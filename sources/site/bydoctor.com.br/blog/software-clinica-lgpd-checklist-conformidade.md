# Source: https://bydoctor.com.br/blog/software-clinica-lgpd-checklist-conformidade

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Software de Clínica em Conformidade com a LGPD: Checklist Completo](https://bydoctor.com.br/_next/image?url=%2Fblog%2Fsoftware-clinica-lgpd-checklist-conformidade%2Ffeatured.png&w=3840&q=75)

![Médica verificando checklist de conformidade LGPD em tablet, com ícones de cadeado e proteção de dados ao fundo](https://bydoctor.com.br/blog/software-clinica-lgpd-checklist-conformidade/featured.png)

Clínicas médicas processam alguns dos dados mais sensíveis que existem: diagnósticos, histórico de saúde, medicamentos em uso, dados genéticos. A [Lei Geral de Proteção de Dados (Lei nº 13.709/2018)](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm) classifica essas informações como dados sensíveis — categoria que exige controles mais rigorosos do que dados pessoais comuns e gera responsabilidade direta para o responsável pela clínica em caso de violação.

O problema é que a maioria das clínicas assume que, por usar um software moderno, está automaticamente em conformidade. Não está. A conformidade com a LGPD depende de como o software foi configurado, quais contratos foram assinados com o fornecedor e como a equipe interna lida com os dados dos pacientes.

Este checklist cobre os 32 pontos que qualquer software de clínica em conformidade com a LGPD precisa atender. Está dividido em quatro blocos: segurança técnica, documentação e contratos, gestão de consentimentos e direitos dos pacientes, e processos internos. Para cada item, há uma indicação do que verificar e o que fazer quando a resposta for não.

## Bloco 1: Segurança técnica (10 itens)

![Interface de painel de segurança digital com indicadores de criptografia, log de acesso e autenticação em dois fatores](https://bydoctor.com.br/blog/software-clinica-lgpd-checklist-conformidade/section_0.png)

A segurança técnica é a camada mais objetiva do checklist. Os itens abaixo podem ser verificados diretamente com o fornecedor ou testados durante o período de trial do software.

### 1\. Criptografia de dados em trânsito

Verifique se o software usa HTTPS com TLS 1.2 ou superior para todas as comunicações entre o navegador/app e os servidores. Na barra de endereço, o cadeado fechado indica que a conexão é criptografada. Softwares que ainda permitem acesso via HTTP sem redirecionamento forçado para HTTPS representam risco real de interceptação.

### 2\. Criptografia de dados em repouso

Além da criptografia em trânsito, os dados armazenados nos servidores do fornecedor precisam estar criptografados — padrão AES-256 é o mais comum e considerado adequado pela ANPD. Pergunte diretamente ao suporte técnico do fornecedor qual algoritmo é usado. Se não souberem responder, é sinal de que a prática não está documentada.

### 3\. Autenticação com senha forte e bloqueio por tentativas

O software precisa exigir senhas com critérios mínimos de complexidade (tamanho mínimo, caracteres especiais) e bloquear o acesso após um número definido de tentativas incorretas. Softwares que aceitam senhas como "123456" sem restrição falham neste item.

### 4\. Autenticação de dois fatores (2FA)

O 2FA reduz drasticamente o risco de acesso não autorizado mesmo quando a senha é comprometida. Verifique se o software oferece 2FA via app autenticador (Google Authenticator, Microsoft Authenticator) ou SMS. Softwares que oferecem 2FA apenas como opcional devem ter esse recurso ativado por política interna da clínica.

### 5\. Controle de acesso por perfil de usuário

Nem toda a equipe precisa acessar o prontuário completo dos pacientes. O software precisa permitir a criação de perfis com permissões distintas: recepcionista acessa agenda e cadastro; médico acessa prontuário e prescrição; administrador acessa financeiro e relatórios. O princípio de menor privilégio (cada usuário acessa apenas o que precisa para seu trabalho) é exigência direta da LGPD para minimização de dados.

### 6\. Log de auditoria de acessos

O sistema precisa registrar quem acessou qual prontuário, quando e de qual dispositivo. Esse log é indispensável para responder a reclamações de pacientes ("quem acessou meu histórico?") e para demonstrar conformidade em caso de fiscalização da [Autoridade Nacional de Proteção de Dados (ANPD)](https://www.gov.br/anpd/pt-br). Verifique se o log é imutável — ou seja, se não pode ser alterado ou excluído por usuários comuns.

### 7\. Backup automático e frequência definida

Backups manuais são backups que não acontecem. O software precisa realizar backup automático dos dados pelo menos diariamente, com retenção por período documentado. Pergunte ao fornecedor: com que frequência o backup é feito? Em quanto tempo é possível restaurar os dados? Onde o backup fica armazenado? As respostas precisam estar no contrato ou no SLA.

### 8\. Localização dos servidores no Brasil

A LGPD permite transferência internacional de dados, mas impõe requisitos adicionais para isso (artigos 33 a 36). Para clínicas que preferem simplicidade regulatória, o ideal é usar softwares cujos servidores estejam localizados no Brasil — preferencialmente em data centers com certificação ISO 27001. Isso não é obrigatório, mas elimina uma camada de complexidade jurídica.

### 9\. Política de retenção e exclusão de dados

O CFM (Conselho Federal de Medicina) exige que prontuários sejam mantidos por pelo menos 20 anos após o último atendimento. Após esse prazo, os dados devem ser descartados de forma segura. Verifique se o software tem uma política documentada de retenção e exclusão — e se o fornecedor garante que os dados são de fato apagados quando o contrato é encerrado.

### 10\. Plano de resposta a incidentes do fornecedor

A LGPD exige que incidentes de segurança (vazamentos, acessos não autorizados) sejam comunicados à ANPD e aos titulares afetados em prazo razoável. Pergunte ao fornecedor: qual é o procedimento em caso de incidente? Em quanto tempo a clínica será notificada? Quem assume a comunicação com a ANPD? Fornecedores sem resposta estruturada para essa pergunta não estão preparados.

## Bloco 2: Documentação e contratos (8 itens)

![Advogado e gestor de clínica revisando contrato DPA em mesa de escritório com documentos de conformidade LGPD](https://bydoctor.com.br/blog/software-clinica-lgpd-checklist-conformidade/section_1.png)

A segurança técnica protege os dados. A documentação protege a clínica juridicamente. Este bloco cobre os documentos que precisam existir — e o que acontece quando não existem.

### 11\. DPA assinado com o fornecedor do software

O DPA (Data Processing Agreement, ou Contrato de Processamento de Dados) é o documento que formaliza a relação entre a clínica (controladora dos dados) e o fornecedor do software (operador). Sem DPA assinado, a clínica pode ser responsabilizada por falhas de segurança causadas pelo fornecedor. Este é o item mais frequentemente ausente em clínicas que acreditam estar em conformidade. Solicite o DPA antes de contratar qualquer software e leia as cláusulas sobre responsabilidade e sub-operadores (fornecedores do fornecedor).

### 12\. Política de privacidade do software publicada e acessível

O fornecedor do software precisa ter uma política de privacidade pública que descreva quais dados coleta, como processa, com quem compartilha e por quanto tempo retém. Verifique se a política está atualizada (data de revisão visível) e se menciona explicitamente os dados de saúde. Políticas genéricas que não tratam especificamente de dados sensíveis são inadequadas para fornecedores de software médico.

### 13\. Termos de uso claros sobre propriedade dos dados

Os dados dos pacientes pertencem à clínica, não ao fornecedor do software. Os termos de uso precisam deixar isso explícito — incluindo o que acontece com os dados quando o contrato é encerrado: prazo para exportação, formato de entrega e garantia de exclusão nos servidores do fornecedor. Contratos que são omissos nesse ponto criam risco real de perda de acesso aos dados históricos.

### 14\. Registro das atividades de tratamento de dados (ROPA)

A LGPD exige que empresas que processam dados sensíveis mantenham um registro documentado das atividades de tratamento. Para clínicas, isso significa mapear: quais dados de pacientes são coletados, com qual finalidade, por quanto tempo são retidos e com quem são compartilhados. Esse documento não precisa ser complexo — uma planilha organizada já é suficiente para clínicas menores — mas precisa existir.

### 15\. Nomeação do Encarregado de Dados (DPO) quando aplicável

A nomeação de um DPO (Data Protection Officer, ou Encarregado de Dados) é obrigatória para organizações que processam dados sensíveis em larga escala. Para a maioria das clínicas pequenas e médias, a ANPD permite que o próprio responsável pela clínica assuma essa função. O que não é permitido é não ter ninguém designado. Formalize por escrito quem é o responsável por decisões relacionadas à proteção de dados.

### 16\. Contrato com suboperadores do fornecedor

Seu fornecedor de software usa infraestrutura de terceiros: provedores de nuvem (AWS, Google Cloud, Azure), serviços de e-mail, plataformas de pagamento. Esses terceiros são sub-operadores. A LGPD exige que o operador (seu fornecedor) garanta que os sub-operadores também estejam em conformidade. Pergunte quais sub-operadores são usados e se há contratos de conformidade com cada um.

### 17\. Política de privacidade da clínica para os pacientes

Além da documentação com o fornecedor, a clínica precisa ter sua própria política de privacidade — o documento que explica aos pacientes quais dados são coletados, para que são usados e quais são seus direitos. Esse documento precisa estar disponível na recepção, no site da clínica e ser entregue ao paciente no primeiro atendimento. Usar a política de privacidade do fornecedor como substituta da sua própria é um erro jurídico comum.

### 18\. Cláusula de confidencialidade nos contratos de trabalho da equipe

A equipe da clínica — recepcionistas, assistentes, médicos — acessa dados de pacientes rotineiramente. Os contratos de trabalho e prestação de serviço precisam ter cláusula explícita de confidencialidade e mencionar as obrigações da LGPD. Em caso de vazamento causado por colaborador, a existência dessa cláusula é parte da demonstração de que a clínica tomou medidas razoáveis de prevenção.

## Bloco 3: Consentimentos e direitos dos pacientes (8 itens)

A LGPD garante direitos aos titulares dos dados — no caso das clínicas, os pacientes. O software precisa ter recursos que permitam à clínica exercer esses direitos na prática.

### 19\. Coleta de consentimento documentada no cadastro do paciente

O consentimento para tratamento de dados sensíveis precisa ser livre, informado, inequívoco e, para dados de saúde, específico (artigo 11 da LGPD). No contexto clínico, isso significa que o paciente deve assinar ou aceitar digitalmente um termo que explique quais dados serão coletados e para quais finalidades. O software precisa registrar esse consentimento com data, hora e versão do termo aceito — não apenas guardar o dado.

### 20\. Finalidade específica para cada tipo de dado coletado

A LGPD proíbe coletar dados sem finalidade definida. O software (e a política da clínica) precisa especificar: o e-mail é coletado para envio de confirmações de consulta; o CPF é coletado para emissão de nota fiscal; o histórico clínico é coletado para continuidade do tratamento. Finalidades vagas como "uso interno" ou "melhoria dos serviços" não são suficientes para dados sensíveis.

### 21\. Recurso para exportação dos dados do paciente

O artigo 18 da LGPD garante ao paciente o direito de portabilidade dos seus dados — ou seja, receber uma cópia dos seus dados em formato estruturado para levar a outro profissional. Verifique se o software permite exportar o prontuário completo do paciente em PDF ou formato aberto. Sistemas que retêm dados em formato não exportável violam esse direito diretamente.

### 22\. Recurso para exclusão de dados mediante solicitação

Pacientes têm o direito de solicitar a exclusão dos seus dados quando o tratamento foi baseado em consentimento e esse consentimento é revogado. Há exceções importantes: dados mantidos para cumprimento de obrigação legal (como o prazo de 20 anos do CFM) não precisam ser excluídos. O software precisa ter um mecanismo para registrar e processar essas solicitações, mesmo que a exclusão seja parcial.

### 23\. Registro de revogação de consentimento

Quando um paciente revoga o consentimento para um determinado uso dos seus dados, esse fato precisa ser registrado no sistema com data e hora. Isso protege a clínica em caso de disputa posterior sobre o que foi ou não autorizado.

### 24\. Mecanismo para correção de dados incorretos

O artigo 18 também garante ao titular o direito de corrigir dados incompletos, inexatos ou desatualizados. O software precisa permitir que a clínica edite o cadastro do paciente mediante solicitação e registre que a edição foi feita a pedido do titular — não por erro operacional da equipe.

### 25\. Informação ao paciente sobre compartilhamento com terceiros

Se a clínica compartilha dados dos pacientes com terceiros — convênios médicos, laboratórios, plataformas de telemedicina — o paciente precisa ser informado disso no momento da coleta. A política de privacidade precisa listar explicitamente quem são esses terceiros e qual dado é compartilhado com cada um.

### 26\. Canal de atendimento para solicitações de titulares

A LGPD exige que os titulares tenham um canal para exercer seus direitos. Para clínicas, isso pode ser tão simples quanto um e-mail dedicado ou um formulário no site. O importante é que o canal exista, seja divulgado e que as solicitações sejam respondidas em prazo razoável — a ANPD considera 15 dias como referência para resposta.

## Bloco 4: Processos internos e treinamento (6 itens)

A conformidade com a LGPD não é apenas uma questão de tecnologia. A maioria dos incidentes de segurança em saúde envolve erro humano — compartilhamento inadvertido de dados, envio de prontuário para número errado no WhatsApp, acesso de ex-funcionários que não tiveram o acesso revogado.

### 27\. Treinamento da equipe sobre LGPD e boas práticas de dados

Toda a equipe que acessa dados de pacientes — recepcionistas, auxiliares, médicos — precisa ser treinada sobre o que pode e o que não pode ser feito com esses dados. Não precisa ser um curso formal: um treinamento de uma hora com exemplos práticos (o que fazer quando um paciente pergunta pelo seu prontuário; como lidar com uma solicitação de exclusão de dados; o que fazer se suspeitar de acesso não autorizado) já é suficiente para clínicas menores.

### 28\. Procedimento para revogação de acesso de ex-colaboradores

O acesso ao software precisa ser desativado no mesmo dia em que um colaborador sai da clínica. Isso parece óbvio, mas a auditoria de acessos frequentemente revela contas de ex-funcionários ainda ativas meses depois do desligamento. Crie um checklist de offboarding que inclua explicitamente a desativação do acesso ao sistema.

### 29\. Política de uso de dispositivos móveis para acesso ao sistema

Médicos que acessam o prontuário pelo celular pessoal representam um vetor de risco. Se o celular for roubado ou perdido sem bloqueio de tela, o acesso ao sistema fica exposto. Defina por escrito uma política mínima: uso de PIN ou biometria no dispositivo, obrigatoriedade de logout após o uso, proibição de salvar dados de pacientes na galeria de fotos do celular.

### 30\. Procedimento documentado para resposta a violações de dados

Em caso de incidente — vazamento, acesso não autorizado, perda de dados —, a clínica tem prazo definido para notificar a ANPD (a regulamentação atual referencia "prazo razoável"). Sem um procedimento documentado, o tempo será perdido discutindo o que fazer em vez de agir. O plano não precisa ser sofisticado: quem é notificado internamente, quem contata o fornecedor, quem redige a comunicação para a ANPD e quem fala com os pacientes afetados.

### 31\. Revisão periódica dos acessos concedidos

Colaboradores mudam de função. A recepcionista que foi promovida a gerente pode ter acumulado permissões de ambos os perfis. Revise trimestralmente quais usuários têm acesso ao sistema, quais permissões cada um tem e se essas permissões ainda fazem sentido para a função atual. Essa revisão leva menos de 30 minutos e elimina uma das principais causas de acesso indevido.

### 32\. Registro das revisões e adequações realizadas

Documentar as ações de conformidade é tão importante quanto realizá-las. Mantenha um registro simples das revisões feitas: data, o que foi verificado, o que foi ajustado e quem realizou. Esse histórico demonstra boa-fé e esforço contínuo de adequação — critérios que a ANPD considera ao aplicar sanções.

## Como interpretar seu resultado

Após percorrer os 32 itens, some quantos você marcou como "sim" e use a tabela abaixo para avaliar o nível de conformidade atual:

| Itens marcados | Situação | O que fazer agora |
| --- | --- | --- |
| 28 a 32 | ✅ Conformidade avançada | Mantenha revisões periódicas e monitore atualizações da ANPD |
| 20 a 27 | ⚠️ Conformidade parcial | Identifique os blocos com mais lacunas e priorize a regularização |
| 12 a 19 | 🔴 Risco moderado | Solicite o DPA ao fornecedor e implante controles básicos com urgência |
| Até 11 | 🚨 Exposição significativa | Consulte um especialista em LGPD e inicie adequação imediata |

Os itens com maior peso jurídico — e que devem ser priorizados em qualquer cenário — são o DPA com o fornecedor (item 11), o log de auditoria (item 6), o consentimento documentado dos pacientes (item 19) e o procedimento de resposta a incidentes (item 30). São os quatro pontos que aparecem com mais frequência nas fiscalizações da ANPD no setor de saúde.

Se o seu software atual não atende a maioria dos itens do Bloco 1 (segurança técnica), o problema provavelmente está no fornecedor — e a troca de sistema precisa entrar na pauta. Adequação de processos internos não resolve lacunas técnicas que o software deveria cobrir.

## Perguntas frequentes sobre conformidade LGPD em software de clínica

### O software da minha clínica precisa assinar um DPA para estar em conformidade com a LGPD?

**Sim.** O DPA (Data Processing Agreement) formaliza as responsabilidades do fornecedor como operador de dados. Sem esse documento, a clínica pode ser responsabilizada por violações causadas pelo fornecedor. A ausência de DPA é um sinal vermelho durante qualquer auditoria da [ANPD](https://www.gov.br/anpd/pt-br).

### Qual é a multa por descumprir a LGPD em uma clínica que usa software inadequado?

**As sanções** previstas no artigo 52 da Lei nº 13.709/2018 vão de advertência até multa de 2% do faturamento anual do grupo econômico, limitada a R$ 50 milhões por infração. A ANPD pode ainda determinar o bloqueio ou eliminação de dados e a suspensão parcial do banco de dados.

### Prontuário eletrônico em nuvem é mais seguro do que servidor local para fins de LGPD?

**Depende do fornecedor, não do modelo.** Sistemas SaaS com certificações ISO 27001, criptografia AES-256 e backups automáticos costumam ser mais seguros do que servidores locais que dependem de manutenção interna. O ponto crítico é verificar onde os dados ficam — prefira fornecedores com servidores no Brasil.

### Com que frequência devo revisar a conformidade LGPD do software da minha clínica?

**Pelo menos uma vez por ano**, e sempre que houver mudança de fornecedor, atualização significativa do software ou alteração da equipe que acessa dados sensíveis. A ANPD recomenda que as organizações mantenham um programa de conformidade contínuo, não apenas uma adequação pontual.

### Clínica com apenas um médico precisa se adequar à LGPD?

**Sim.** A LGPD não distingue porte da organização. Todo profissional que coleta, armazena ou processa dados de pacientes está sujeito à lei. O que muda é a escala — um consultório solo precisa de DPA, política de privacidade e controles básicos de acesso, mas não necessariamente de um DPO dedicado.

## Resumo

A conformidade com a LGPD em software de clínica passa por quatro frentes: segurança técnica (criptografia, log, backup, 2FA), documentação e contratos (DPA, política de privacidade, registro de atividades), gestão de consentimentos e direitos dos pacientes (portabilidade, exclusão, correção), e processos internos (treinamento, revogação de acesso, resposta a incidentes).

Dos 32 itens deste checklist, os mais críticos são o DPA com o fornecedor, o log de auditoria de acessos, o consentimento documentado dos pacientes e o plano de resposta a incidentes. Clínicas que ainda não têm esses quatro pontos cobertos devem priorizá-los antes de qualquer outra adequação.

O [ByDoctor](https://bydoctor.com.br/) foi desenvolvido com conformidade LGPD nativa: criptografia AES-256, log de auditoria imutável, DPA disponível para assinatura, controle de acesso por perfil e servidores localizados no Brasil. Para ver como o sistema lida com cada item deste checklist na prática, [solicite um teste gratuito](https://bydoctor.com.br).

## Artigos relacionados

- [Software de Clínica e LGPD: Perguntas que Médicos Fazem à ANPD](https://bydoctor.com.br/blog/software-clinica-lgpd-perguntas-medicos-anpd)
- [Como Excluir Dados de Pacientes em Conformidade com a LGPD](https://bydoctor.com.br/blog/como-excluir-dados-pacientes-lgpd)
- [Portal do Paciente Online e LGPD: Proteção de Dados](https://bydoctor.com.br/blog/portal-do-paciente-online-lgpd-protecao-de-dados)