# Source: https://bydoctor.com.br/blog/como-excluir-dados-pacientes-lgpd

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Como Excluir Dados de Pacientes em Conformidade com a LGPD](https://bydoctor.com.br/_next/image?url=%2Fblog%2Fcomo-excluir-dados-pacientes-lgpd%2Ffeatured.png&w=3840&q=75)

Excluir dados de pacientes em conformidade com a LGPD exige verificar três coisas antes de apertar qualquer botão: a identidade do solicitante, a base legal que justificou o tratamento original e se existe obrigação de guarda que supere o pedido. Dados de saúde têm prazo mínimo de retenção definido pelo [Conselho Federal de Medicina (CFM)](https://portal.cfm.org.br) — e ignorar esse prazo gera risco regulatório tão sério quanto ignorar a LGPD.

**Software clínica LGPD** é qualquer sistema de gestão clínica que trata dados pessoais de pacientes em conformidade com a [Lei Geral de Proteção de Dados (Lei nº 13.709/2018)](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm). Isso inclui mecanismos de controle de acesso, registro de consentimento, logs de auditoria e — ponto central deste guia — procedimentos documentados para exclusão ou anonimização de dados quando o titular solicita.

A [Autoridade Nacional de Proteção de Dados (ANPD)](https://www.gov.br/anpd/pt-br) já aplicou sanções a organizações do setor de saúde por ausência de procedimentos claros de resposta a direitos dos titulares. Clínicas que não têm um fluxo definido para lidar com pedidos de exclusão ficam expostas a multas de até 2% do faturamento, limitadas a R$ 50 milhões por infração. Para entender o quadro completo de penalidades, o post sobre [penalidades da LGPD para software de clínica](https://bydoctor.com.br/blog/lgpd-software-clinica-penalidades) detalha os casos já autuados.

![Médica revisando política de privacidade em tablet em consultório moderno](https://bydoctor.com.br/blog/como-excluir-dados-pacientes-lgpd/featured.png)

## Quando a clínica pode — e quando não pode — excluir dados de pacientes

A LGPD garante o direito à exclusão no artigo 18, mas o mesmo artigo prevê exceções. Para clínicas, a exceção mais relevante é a obrigação legal de guardar o prontuário. A Resolução CFM nº 1.821/2007 estabelece os prazos mínimos de guarda:

| Tipo de paciente | Prazo mínimo de guarda | Contagem |
| --- | --- | --- |
| Adulto (18+ anos) | 20 anos | A partir do último atendimento registrado |
| Menor de idade | Até 5 anos após atingir 18 anos | Ou seja, mínimo de 23 anos a partir do nascimento |
| Paciente falecido | 10 anos | A partir da data do óbito |
| Microfilmagem ou digitalização | Permanente (sem prazo de descarte) | Conforme legislação de arquivos públicos |

Isso significa que um paciente adulto que foi atendido uma única vez em 2024 tem o prontuário protegido de exclusão até, no mínimo, 2044 — independentemente do que ele solicite. A clínica pode e deve informar isso ao titular, com referência à norma, em até 15 dias após o pedido.

Fora do prazo de guarda obrigatória, a exclusão precisa acontecer quando: o paciente revoga o consentimento (se consentimento era a única base legal), o dado não é mais necessário para a finalidade original, ou o tratamento foi realizado em desconformidade com a lei. Para cada situação, o fluxo de resposta é diferente — o [checklist de conformidade LGPD para software de clínica](https://bydoctor.com.br/blog/software-clinica-lgpd-checklist-conformidade) mapeia cada cenário com ação correspondente.

## Como processar um pedido de exclusão em 5 passos

### Passo 1: Verificar a identidade do solicitante

Antes de qualquer ação, confirme que a pessoa que está pedindo é de fato o titular dos dados. Para pedidos digitais (e-mail, formulário), exija CPF e um dado de confronto — data de nascimento ou número do prontuário. Para pedidos presenciais, valide documento com foto.

Menores de 16 anos precisam do representante legal. Para dados de paciente falecido, o pedido pode vir de sucessores — avalie caso a caso com base no artigo 18, §6º da LGPD.

### Passo 2: Checar os prazos de guarda e a base legal original

Com a identidade confirmada, acesse o histórico do paciente no seu [prontuário eletrônico](https://bydoctor.com.br/blog/prontuario-eletronico-guia-definitivo-medicos-clinicas) e verifique:

- Data do último atendimento registrado
- Se o paciente é maior de idade (ou era menor na época dos atendimentos)
- Quais dados estão dentro do prazo de guarda obrigatória
- Quais dados foram coletados com base em consentimento vs. obrigação legal

Dados coletados com base em obrigação legal — como o prontuário clínico — não podem ser excluídos enquanto o prazo de guarda vigir. Dados acessórios coletados com base em consentimento e que não fazem parte do prontuário (como e-mails de marketing, preferências de comunicação) podem ser excluídos independentemente.

### Passo 3: Documentar o pedido e a decisão

Todo pedido de exclusão precisa de registro formal. Crie um protocolo de atendimento com:

- Data e hora do recebimento
- Canal (e-mail, formulário, presencial)
- Dados do solicitante e relação com o titular
- Escopo do pedido (quais dados, qual finalidade de exclusão)
- Decisão tomada (deferir, deferir parcialmente, indeferir) e justificativa com referência legal
- Data de resposta ao titular

Esse registro é sua prova em caso de auditoria da ANPD. Guarde por, no mínimo, 5 anos. Sistemas como o ByDoctor permitem registrar anotações administrativas vinculadas ao cadastro do paciente sem que essas anotações façam parte do prontuário clínico — útil exatamente para esse tipo de documentação interna.

![Profissional de saúde verificando documentos de conformidade em laptop com café ao lado](https://bydoctor.com.br/blog/como-excluir-dados-pacientes-lgpd/section_0.png)

### Passo 4: Executar a exclusão ou anonimização

Se a exclusão for possível (dados fora do prazo de guarda ou dados baseados exclusivamente em consentimento revogado), execute em quatro camadas:

1. **Banco de dados principal do sistema**: use a funcionalidade de exclusão do seu software clínica LGPD. Softwares conformes registram log da operação com usuário, data e hora.
2. **Backups automáticos**: verifique a política de retenção de backups do fornecedor. Se os backups são criptografados e inacessíveis individualmente, a exclusão propagada pode ocorrer no próximo ciclo de rotação — documente isso.
3. **Planilhas e exportações locais**: é aqui que a maioria das clínicas tem o maior risco. Dados exportados para Excel, Google Sheets ou enviados por e-mail para a equipe criam cópias fora do controle do sistema. Mapeie onde esses dados foram parar.
4. **Arquivos físicos digitalizados**: documentos escaneados e salvos em pastas locais ou Google Drive precisam ser identificados e excluídos manualmente.

Quando a exclusão total não é possível (dados dentro do prazo de guarda), use anonimização. **Anonimização** é o processo de modificar o dado de forma que seja tecnicamente impossível reidentificar o titular — mesmo com cruzamento de outras bases. Pseudonimização (trocar nome por código) não basta: o código ainda permite reidentificação e o dado continua no escopo da LGPD. Para entender a diferença técnica, o guia de [LGPD para software de clínica médica](https://bydoctor.com.br/blog/lgpd-software-clinica-medica-o-que-e-como-impacta) detalha os conceitos com exemplos práticos.

### Passo 5: Comunicar o resultado ao paciente em até 15 dias

A resposta ao titular precisa ser formal — por escrito, pelo mesmo canal que o pedido chegou. Se deferir a exclusão, confirme quais dados foram eliminados e em quais sistemas. Se indeferir (total ou parcialmente), cite a norma que justifica a retenção e informe quando os dados serão excluídos após o prazo de guarda.

O prazo de 15 dias é contado em dias corridos a partir do recebimento do pedido. Pedidos complexos que envolvem múltiplos prontuários ou diversas categorias de dados podem ter prazo estendido com comunicação prévia ao titular — mas o silêncio nunca é uma opção segura.

## O que verificar no seu software clínica LGPD

Nem todo sistema de gestão clínica está preparado para processar pedidos de exclusão de forma rastreável. Antes de receber o primeiro pedido, verifique se o seu software oferece:

| Funcionalidade | O que procurar | Risco se ausente |
| --- | --- | --- |
| Log de auditoria por usuário | Registro de quem acessou, editou ou excluiu cada dado, com data e hora | Impossível provar conformidade em auditoria da ANPD |
| Controle granular de permissões | Acesso por função: recepcionista não acessa prontuário; financeiro não acessa dados clínicos | Violação de dados internos e infração do princípio da necessidade (LGPD, art. 6º) |
| Exclusão ou anonimização de cadastro | Função dedicada para remover ou despersonalizar dados de paciente específico | Exclusão manual gera inconsistências e não é auditável |
| Política de retenção de backups documentada | Ciclo de rotação dos backups, prazo máximo de retenção, criptografia em repouso | Dados "excluídos" do sistema podem persistir em backups por anos |
| Relatório de mapeamento de dados | Onde cada categoria de dado é armazenada, por quanto tempo e com qual finalidade | Impossível responder ao titular quais dados existem e onde estão |
| Contrato de operador (DPA) | Documento que define responsabilidades do fornecedor de software como operador de dados | A clínica responde sozinha por violações causadas pelo software |

Se o seu sistema atual não oferece log de auditoria ou função de exclusão rastreável, você está operando com risco. A [verificação de conformidade LGPD do seu software de clínica](https://bydoctor.com.br/blog/como-verificar-conformidade-lgpd-software-clinica) pode ser feita com um processo estruturado — e é o primeiro passo antes de qualquer pedido de exclusão chegar.

## Quais dados de pacientes podem ser anonimizados em vez de excluídos?

Quando a exclusão total conflita com a obrigação de guarda, a anonimização permite cumprir ambas as exigências. A lógica: o dado clínico permanece para fins de guarda legal, mas o vínculo com o titular é desfeito de forma irreversível.

Na prática, uma clínica pode anonimizar dados de paciente mantendo registros clínicos para fins epidemiológicos ou de auditoria interna — desde que não seja mais possível identificar a pessoa. O processo técnico envolve:

- **Substituição de identificadores diretos**: nome, CPF, RG, data de nascimento completa, endereço, telefone e e-mail são removidos ou substituídos por valores sintéticos sem correspondência real
- **Generalização de quase-identificadores**: dados como faixa etária (em vez de data exata), cidade (em vez de endereço completo) e especialidade atendida (em vez de diagnóstico específico) reduzem o risco de reidentificação por cruzamento
- **Verificação de reidentificabilidade**: após a anonimização, teste se o registro ainda permite identificar o titular com outras bases de dados acessíveis — um prontuário de paciente com doença rara em cidade pequena pode ser reidentificável mesmo sem nome

A anonimização precisa ser documentada: quais campos foram alterados, qual técnica foi usada, quem executou e quando. Esse registro é o que diferencia anonimização real de pseudonimização — e o que a ANPD vai pedir em caso de contestação.

![Tela de sistema de gestão clínica mostrando configurações de privacidade e proteção de dados](https://bydoctor.com.br/blog/como-excluir-dados-pacientes-lgpd/section_1.png)

## Perguntas frequentes sobre exclusão de dados de pacientes e LGPD

### Clínica é obrigada a excluir dados de pacientes quando solicitado?

Depende do prazo de guarda. A LGPD garante o direito à exclusão, mas dados de saúde têm retenção mínima definida pelo CFM: 20 anos após o último atendimento para adultos. Enquanto esse prazo vigir, a clínica pode indeferir o pedido e deve comunicar o motivo ao paciente em até 15 dias, com referência à norma.

### Qual o prazo para responder um pedido de exclusão de dados?

15 dias corridos a partir do recebimento do pedido, conforme o artigo 18 da LGPD. Esse prazo vale tanto para confirmação de exclusão quanto para justificativa de negativa. Silêncio no prazo pode ser interpretado como infração administrativa pela ANPD. Documente cada etapa do processo de resposta.

### O que é anonimização e quando usar no lugar da exclusão?

Anonimização é o processo de desassociar o dado do titular de forma tecnicamente irreversível. É a alternativa legal quando a exclusão total não é possível por obrigação de guarda. Dados corretamente anonimizados saem do escopo da LGPD — mas o processo precisa ser robusto o suficiente para resistir a tentativas de reidentificação por cruzamento de bases.

### Como garantir que o backup também exclua os dados do paciente?

Mapeie todos os repositórios onde o dado existe: banco de dados principal, backups automáticos, planilhas locais e arquivos exportados. Verifique a política de retenção de backups do seu fornecedor de software clínica LGPD — backups com ciclo de rotação curto (7 a 30 dias) reduzem o risco de persistência. Para backups de longa retenção, a exclusão propagada precisa ser explicitamente confirmada pelo fornecedor no contrato de operador (DPA).

### O paciente pode pedir exclusão de dados de prontuário digital?

Pode solicitar, mas a clínica pode indeferir enquanto o prazo de guarda do CFM (mínimo 20 anos para adultos) não tiver expirado. A obrigação legal de retenção prevalece sobre o direito de exclusão da LGPD. Após o prazo de guarda, a exclusão torna-se obrigatória se solicitada — ou pode ser feita proativamente pela clínica como boa prática de gestão de dados.

## Resumo

Excluir dados de pacientes em conformidade com a LGPD significa verificar prazos de guarda (mínimo 20 anos para adultos, conforme CFM 1.821/2007), documentar cada pedido e decisão, executar a exclusão em todas as camadas do sistema — incluindo backups e cópias locais — e comunicar o resultado em até 15 dias. Quando a exclusão não é possível, anonimização irreversível é a alternativa legal.

O ByDoctor oferece controle de acesso por função, log de auditoria e suporte para mapeamento de dados — recursos essenciais para qualquer clínica que precisa responder a pedidos de titulares com segurança e rastreabilidade. Para verificar se sua operação atual está preparada, acesse o [checklist de conformidade LGPD para software de clínica](https://bydoctor.com.br/blog/software-clinica-lgpd-checklist-conformidade) ou conheça as [funcionalidades do ByDoctor](https://bydoctor.com.br/#funcionalidades) voltadas à proteção de dados.

## Artigos relacionados

- [Software de Clínica e LGPD: Perguntas que Médicos Fazem à ANPD](https://bydoctor.com.br/blog/software-clinica-lgpd-perguntas-medicos-anpd)
- [Como Verificar se o Software da Sua Clínica está em Conformidade com LGPD](https://bydoctor.com.br/blog/como-verificar-conformidade-lgpd-software-clinica)
- [LGPD e Software de Clínica: Penalidades para Quem Não se Adequar](https://bydoctor.com.br/blog/lgpd-software-clinica-penalidades)