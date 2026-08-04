# Source: https://bydoctor.com.br/blog/faturamento-tiss-clinica-o-que-e-guia-completo

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Faturamento TISS: O que é e Por que é Essencial para sua Clínica](https://bydoctor.com.br/_next/image?url=%2Fblog%2Ffaturamento-tiss-clinica-o-que-e-guia-completo%2Ffeatured.png&w=3840&q=75)

Faturamento TISS é o processo pelo qual clínicas e consultórios registram e enviam eletronicamente os atendimentos às operadoras de planos de saúde, seguindo o padrão obrigatório da [ANS](https://www.gov.br/ans/pt-br) (atual Resolução Normativa nº 501/2022). Feito com erros, gera glosas: recusas de pagamento que, segundo a [Associação Nacional de Hospitais Privados (Anahp)](https://www.anahp.com.br/noticias/indicadores-financeiros-dos-hospitais-desajustes-na-saude/), alcançaram 11,89% da receita de convênios em 2023.

**TISS** — Troca de Informações na Saúde Suplementar — é o padrão eletrônico criado pela ANS em 2007 e tornado obrigatório a partir de 2008 para toda troca de dados entre prestadores de serviços de saúde e operadoras de planos. Ele define a estrutura, o formato e o conteúdo de cada guia de faturamento, do código de procedimento ao diagnóstico CID-10. Sem seguir esse padrão, a operadora simplesmente rejeita o lote.

Clínicas que dominam o faturamento TISS, com tabelas atualizadas, autorizações conferidas e guias sem erro, recebem mais rápido e contestam menos. A própria Anahp aponta que, dos 11,89% inicialmente glosados em 2023, apenas 1,17% se confirmam como glosa devida na contabilidade. A maior parte é recusa indevida, evitável com processo estruturado e validação antes do envio.

![Recepcionista de clínica revisando guias TISS em sistema digital de faturamento](https://bydoctor.com.br/blog/faturamento-tiss-clinica-o-que-e-guia-completo/featured.png)

## O que é TISS e quem precisa usar?

**TISS (Troca de Informações na Saúde Suplementar)** é o componente do Padrão TISS que estabelece as regras para troca eletrônica de dados clínicos e administrativos entre prestadores (clínicas, laboratórios, hospitais) e operadoras de planos de saúde. Regido atualmente pela [Resolução Normativa ANS nº 501/2022](https://www.gov.br/ans/pt-br/acesso-a-informacao/perfis-de-interesse/prestadores/tiss-troca-de-informacoes-na-saude-suplementar) (que substituiu a antiga RN nº 305/2012), alterada pela RN nº 631/2025, o TISS é obrigatório para qualquer prestador que realize atendimentos custeados por planos de saúde no Brasil.

Na prática, isso inclui desde consultórios médicos individuais com um único convênio até clínicas multiprofissionais com dezenas de operadoras. Quem fatura manualmente, em papel ou em formatos fora do padrão, recebe glosa automática. A ANS atualiza o componente periodicamente — ignorar a versão vigente é garantia de rejeição em lote.

O padrão TISS organiza as informações em três grupos principais: mensagens de elegibilidade (verificação do beneficiário antes do atendimento), mensagens de autorização prévia e mensagens de cobrança — as guias propriamente ditas. Para clínicas de atenção primária, o contato mais frequente é com as mensagens de cobrança, especialmente a Guia de Consulta e a Guia SP/SADT.

## Como funciona o faturamento TISS na prática?

O ciclo começa antes do atendimento. A clínica verifica a elegibilidade do beneficiário — se o plano está ativo e cobre o procedimento solicitado. Depois do atendimento, preenche a guia correspondente com os dados do paciente, os códigos TUSS dos procedimentos realizados, o CID-10 do diagnóstico e a assinatura digital do profissional. Em seguida, agrupa essas guias em um lote XML e envia eletronicamente à operadora.

A operadora processa o lote, valida os dados e devolve um arquivo de retorno informando quais guias foram aceitas, quais estão em análise e quais sofreram glosa (recusa). O prazo de pagamento é definido em contrato entre operadora e prestador, conforme a [Lei nº 13.003/2014 e a RN ANS nº 363/2014](https://www.gov.br/ans/pt-br); para muitos atendimentos ambulatoriais fica em torno de 30 dias após a entrega do lote, mas atrasos por glosas podem estender esse prazo indefinidamente.

![Diagrama do ciclo de faturamento TISS desde atendimento até recebimento em clínica](https://bydoctor.com.br/blog/faturamento-tiss-clinica-o-que-e-guia-completo/section_0.png)

Para clínicas que atendem múltiplos convênios, o desafio aumenta: cada operadora tem prazos de faturamento, tabelas de procedimentos e regras de autorização diferentes dentro do mesmo padrão TISS. Ferramentas como o [módulo financeiro do ByDoctor](https://bydoctor.com.br/#funcionalidades) centralizam esses fluxos, reduzindo o tempo de fechamento de lote de dias para horas.

### Tabela: principais operadoras e especificidades de faturamento

| Operadora | Prazo de envio de lote | Exige autorização prévia (consultas)? | Tabela de referência |
| --- | --- | --- | --- |
| Unimed | Até o 5º dia útil do mês seguinte | Depende da cobertura contratada | CBHPM + TUSS |
| Bradesco Saúde | Até o 10º dia útil do mês seguinte | Sim, para procedimentos cirúrgicos | TUSS |
| SulAmérica | Até o 15º dia corrido do mês seguinte | Não para consultas simples | TUSS + AMB |
| Amil | Até o 5º dia útil do mês seguinte | Sim, via portal próprio | TUSS |
| Hapvida/NotreDame | Fechamento mensal por contrato | Sim, sistema integrado | TUSS |

Os prazos e exigências acima são referências gerais — cada contrato pode ter especificidades. Sempre confirme com o seu gestor de relacionamento na operadora.

## Quais são as principais guias TISS e quando usar cada uma?

Cada tipo de atendimento tem uma guia correspondente no TISS. Usar a guia errada é uma das principais causas de glosa técnica — a operadora rejeita sem análise de mérito.

1. **Guia de Consulta**: usada para consultas médicas e de outros profissionais de nível superior (psicólogos, nutricionistas, fisioterapeutas). Campos obrigatórios incluem carteirinha do beneficiário, CRM/CRO/CRN do profissional, CID-10 e código TUSS do tipo de consulta.
2. **Guia SP/SADT (Serviços Profissionais e Serviços Auxiliares de Diagnose e Terapia)**: para exames laboratoriais, de imagem, fisioterapia e outros procedimentos ambulatoriais. É a guia mais complexa: exige detalhamento de cada procedimento com código TUSS, quantidade, grau de participação e, em muitos casos, autorização prévia.
3. **Guia de Internação**: registra admissões hospitalares. Inclui dados de CID de internação, previsão de permanência e plano de tratamento. Obrigatória sempre que há internação, mesmo de curta duração.
4. **Guia de Honorários Individuais**: usada por profissionais que participam de equipes cirúrgicas ou procedimentos em ambiente hospitalar. Cada médico (cirurgião, anestesista, auxiliar) emite sua própria guia.
5. **Guia de Resumo de Internação (GRI)**: fecha o ciclo hospitalar, consolidando todos os serviços prestados durante a internação. Enviada após a alta do paciente.

Para clínicas ambulatoriais sem internação, as guias mais usadas no dia a dia são Consulta e SP/SADT. Conhecer a fundo essas duas já resolve 80% do faturamento conveniado da maioria dos consultórios.

## Por que o faturamento incorreto gera glosas — e quanto isso custa?

Glosa é a recusa, total ou parcial, de pagamento pela operadora. Ela pode ser técnica (erro de preenchimento, código inválido, falta de autorização) ou clínica (procedimento não coberto, divergência entre diagnóstico e procedimento). As técnicas são as mais evitáveis — e as mais comuns em clínicas sem processo estruturado.

As principais causas de glosa técnica — as mais evitáveis — são:

- **Código TUSS incorreto ou desatualizado** — tabela TUSS tem atualizações periódicas; usar um código descontinuado gera rejeição automática;
- **Ausência de autorização prévia** — procedimentos que exigem guia de autorização enviados sem esse campo preenchido são devolvidos sem análise;
- **Dados do beneficiário divergentes** — nome, número de carteirinha ou data de nascimento diferente do cadastro da operadora;
- **CID-10 incompatível com o procedimento** — diagnóstico que não justifica o procedimento realizado, do ponto de vista clínico ou regulatório;
- **Prazo de envio extrapolado** — lotes enviados após o prazo contratual são glosados integralmente, sem direito a recurso na maioria dos contratos.

O impacto financeiro é direto. Uma clínica que fatura R$ 50.000/mês em convênios e tem 10% de glosa perde R$ 5.000 por mês — R$ 60.000 por ano. Parte desse valor pode ser recuperada via recurso de glosa, mas o processo é demorado e trabalhoso, consumindo tempo da equipe administrativa. Clínicas com [controle financeiro estruturado](https://bydoctor.com.br/blog/controle-financeiro-consultorios-2026) monitoram a taxa de glosa mensalmente como KPI de gestão.

![Gráfico de barras mostrando impacto financeiro de glosas no faturamento mensal de clínica médica](https://bydoctor.com.br/blog/faturamento-tiss-clinica-o-que-e-guia-completo/section_1.png)

## Como reduzir glosas e otimizar o faturamento TISS?

Reduzir glosas passa por três frentes: padronizar o processo de preenchimento, manter o cadastro atualizado e automatizar a validação antes do envio.

### 1\. Use sempre a tabela TUSS vigente

A Tabela TUSS (Terminologia Unificada da Saúde Suplementar) é o dicionário de procedimentos do sistema TISS, publicado pela [ANS](https://www.gov.br/ans/pt-br) com atualizações periódicas. Usar um código descontinuado — mesmo que tenha funcionado no mês anterior — resulta em rejeição automática. Veja [como usar as tabelas TISS/TUSS corretamente](https://bydoctor.com.br/blog/faturamento-tiss-tuss-como-usar-as-tabelas-corretamente); sistemas integrados ao prontuário atualizam essa tabela automaticamente, eliminando o risco.

### 2\. Verifique elegibilidade antes do atendimento

Confirmar que o plano está ativo e que o procedimento está coberto antes de atender evita um dos cenários mais frustrantes: realizar o atendimento, faturar e receber glosa por carência ou por cobertura não prevista em contrato. A verificação de elegibilidade pode ser feita via sistema TISS, por telefone ou pelo portal da operadora. Com [agendamento online integrado ao sistema de gestão](https://bydoctor.com.br/blog/agendamento-online-clinicas-beneficios-dicas), é possível automatizar essa checagem no momento do agendamento.

### 3\. Implemente revisão de lote antes do envio

Antes de fechar e enviar o lote mensal, reserve 30 a 60 minutos para revisar uma amostra das guias — especialmente as de procedimentos de maior valor. Erros de digitação em campos críticos como CID-10 e código TUSS são os mais comuns e os mais fáceis de corrigir antes da rejeição. Softwares como o ByDoctor validam automaticamente as guias contra as regras da operadora antes do envio, apontando erros em tempo real.

### 4\. Treine a equipe administrativa continuamente

A maioria das glosas técnicas começa no preenchimento da recepção ou do faturamento. Uma capacitação de 4 horas por semestre sobre TISS, focada nos erros mais comuns da clínica, tem ROI imediato. O relatório de glosas do mês anterior é o melhor material de treinamento: mostra exatamente onde a equipe erra com mais frequência.

## Perguntas frequentes sobre faturamento TISS

### O que é TISS em saúde?

TISS (Troca de Informações na Saúde Suplementar) é o padrão obrigatório da ANS que regula a troca eletrônica de dados entre prestadores e operadoras de planos de saúde. Em vigor desde 2008 e hoje regido pela Resolução Normativa nº 501/2022, define a estrutura, o formato e o conteúdo de cada guia de faturamento.

### O que é glosa no faturamento TISS?

Glosa é a recusa total ou parcial de pagamento pela operadora. Pode ser técnica (código TUSS incorreto, falta de autorização, dados divergentes) ou clínica (procedimento não coberto). Segundo a Anahp, a glosa inicial chegou a 11,89% da receita de convênios em 2023, mas apenas 1,17% se confirmam como devidas na contabilidade.

### Quais são as principais guias TISS?

As cinco guias principais são: Guia de Consulta (atendimentos ambulatoriais), Guia SP/SADT (exames e procedimentos), Guia de Internação (admissões hospitalares), Guia de Honorários Individuais (equipe cirúrgica) e Guia de Resumo de Internação (fechamento hospitalar). Para consultórios e clínicas ambulatoriais, Consulta e SP/SADT representam a maior parte do volume de faturamento.

### Como evitar glosas no faturamento TISS?

Para reduzir glosas: mantenha o cadastro dos beneficiários atualizado, use sempre a versão vigente da tabela TUSS, confira a autorização prévia quando exigida e valide as guias eletronicamente antes de fechar o lote. Padronizar o preenchimento e revisar as guias de maior valor antes do envio corta a maioria das rejeições técnicas.

### Qual é a versão vigente do padrão TISS em 2026?

O padrão TISS é regido pela Resolução Normativa ANS nº 501/2022, alterada pela RN nº 631/2025. A ANS publica novas versões periodicamente e divulgou atualização em setembro de 2025, com mudanças nas tabelas de materiais e medicamentos. Usar a versão e a tabela TUSS vigentes evita rejeição automática do lote.

## Em resumo

Faturamento TISS correto é pré-requisito para qualquer clínica conveniada manter o caixa saudável. O padrão da ANS (RN nº 501/2022) define uma guia para cada tipo de atendimento, e erros geram glosas que pressionam a receita. Equipe treinada, tabela TUSS vigente e validação automática das guias são o caminho mais direto para receber no prazo.

Para colocar isso em prática, o primeiro passo é mapear a taxa de glosa atual da sua clínica — número de guias rejeitadas dividido pelo total enviado no mês. Se esse índice for superior a 5%, há ganho imediato em revisar o processo de faturamento. O ByDoctor integra [prontuário eletrônico](https://bydoctor.com.br/#funcionalidades), faturamento TISS e gestão financeira em um único sistema, eliminando a dupla digitação e validando as guias automaticamente antes do envio.

## Artigos relacionados

- [Treinamento da Equipe de Faturamento TISS: Guia Prático](https://bydoctor.com.br/blog/faturamento-tiss-treinamento-equipe-faturamento)
- [Faturamento TISS: Quanto Tempo Demora para Receber dos Convênios?](https://bydoctor.com.br/blog/faturamento-tiss-quanto-tempo-demora-receber-convenios)
- [Faturamento TISS e TUSS: Como Usar as Tabelas Corretamente](https://bydoctor.com.br/blog/faturamento-tiss-tuss-como-usar-as-tabelas-corretamente)