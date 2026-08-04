# Source: https://bydoctor.com.br/compliance

[Voltar à home](https://bydoctor.com.br/)

## Resumo de segurança

Hospedagem

AWS (São Paulo) + Google Cloud Storage

Criptografia em trânsito

TLS 1.3 com HSTS forçado

Criptografia em repouso

AES-256 (S3, RDS, GCS)

Autenticação

Clerk (JWT, MFA, SSO, SAML)

Arquitetura

Multi-tenant com isolamento lógico total

Trilha de auditoria

Imutável, por usuário e timestamp

Backups

Automáticos, point-in-time, 30 dias

Monitoramento

Sentry + Datadog APM + OpenTelemetry

Prescrição digital

MEMED (ICP-Brasil, CFM)

Disponibilidade

SLA-alvo de 99,9% mensal

Resposta a incidentes

Notificação à ANPD em até 48h úteis

Última atualização

12 de maio de 2026

## Como protegemos os dados

Seis pilares formam a base de segurança da plataforma. O time de engenharia revisa cada um deles em cada release.

### Criptografia ponta a ponta

Cada requisição entre o navegador e a ByDoctor passa por TLS 1.3 com HSTS forçado. No banco e nos buckets, os dados ficam cifrados em AES-256.

- •TLS 1.3 obrigatório em todas as rotas (sem fallback para HTTP)
- •AES-256 em repouso no PostgreSQL, S3 e Google Cloud Storage
- •URLs assinadas com expiração curta para anexos de prontuário
- •Chaves rotacionadas pelo provedor de nuvem (KMS)

### Arquitetura multi-tenant

Cada clínica vive em um tenant isolado. Toda consulta ao banco filtra por organização antes de retornar — separação garantida na camada de aplicação e revisada por testes automáticos.

- •Isolamento lógico por organization\_id em todas as tabelas
- •Testes de regressão automatizados contra vazamento entre tenants
- •Sem possibilidade de uma clínica enxergar dados de outra
- •Recepcionista de uma clínica nunca aparece em buscas de outra

### Autenticação e controle de acesso

Login centralizado via Clerk com suporte a senha forte, autenticação em dois fatores, SSO corporativo e SAML para clínicas maiores. Três papéis cobrem os fluxos clínicos e administrativos.

- •MFA opcional por usuário; obrigatório para perfis Admin sob política da clínica
- •Sessões com tokens JWT de curta duração e refresh seguro
- •Papéis Admin, Profissional e Colaborador com escopos distintos
- •Recepcionistas não acessam prontuário, evolução ou prescrições

### Trilha de auditoria imutável

Toda mudança em consulta, paciente, prescrição, exame ou documento clínico fica registrada com autor, data, IP e diff do conteúdo — atendendo ao requisito de rastreabilidade da Resolução CFM 1.821/2007.

- •Logs de criação, edição e exclusão por entidade
- •Histórico de acesso a prontuário visível para o Admin
- •Retenção do log alinhada com a vida do prontuário (20 anos)
- •Exportação sob demanda para auditorias internas

### Continuidade e backups

Backups automáticos do banco com restauração point-in-time em janela de 30 dias. Arquivos em buckets com versionamento e replicação multi-AZ.

- •Backups diários completos + WAL contínuo (PostgreSQL)
- •Replicação multi-AZ na AWS São Paulo
- •Plano de Disaster Recovery com RPO ≤ 15 min e RTO ≤ 4 h
- •Testes de restauração executados periodicamente

### Resposta a incidentes

Quando algo sai do esperado, o playbook é claro: contenção em até 4 horas, comunicação ao controlador (clínica) em até 24 horas e notificação à ANPD em até 48 horas úteis, conforme orientação do Art. 48 da LGPD.

- •Canal dedicado: security@bydoctor.com.br
- •Monitoramento contínuo com Sentry e Datadog APM
- •Plano de resposta documentado com papéis e SLA
- •Comunicação ao titular quando houver risco relevante

## Padrões, leis e certificações

### LGPD — Lei 13.709/2018

Em conformidade

Tratamos os dados pessoais e sensíveis de saúde nas bases legais previstas no Art. 7º (II, VI, VIII) e no Art. 11, II, alíneas “a” e “f”. Detalhes completos em /lgpd.

### Resolução CFM 1.821/2007

Plataforma desenhada para atender

A norma do Conselho Federal de Medicina sobre o prontuário eletrônico exige integridade, auditoria, controle de acesso e armazenamento seguro. Cada um desses requisitos está mapeado para um controle técnico na plataforma.

### Resolução CFM 2.314/2022

Suportada

Marco vigente da telemedicina no Brasil. A ByDoctor permite registrar o consentimento informado do paciente, anexar documentos da consulta remota e manter a evolução assinada no prontuário.

### Lei 13.787/2018

Suportada

Lei da digitalização do prontuário. A retenção mínima de 20 anos e a possibilidade de uso exclusivo do meio eletrônico estão refletidas no modelo de retenção e na trilha de auditoria.

### ICP-Brasil (MP 2.200-2/2001)

Disponível via MEMED

Prescrições digitais emitidas pela ByDoctor usam o provedor MEMED, que aplica assinatura digital com certificados ICP-Brasil — equivalente à assinatura manuscrita conforme a Medida Provisória 2.200-2/2001.

### ISO 27001 e ISO 27018

Herdada da infraestrutura (AWS, GCP)

A infraestrutura de nuvem da ByDoctor roda sobre Amazon Web Services e Google Cloud, ambos certificados ISO 27001, ISO 27017 e ISO 27018 (proteção de dados pessoais na nuvem). A ByDoctor opera dentro do modelo de responsabilidade compartilhada.

### SOC 2 (provedores)

Herdada da infraestrutura

Stripe, Clerk, AWS, Google Cloud, MEMED, OpenAI e Sentry — todos os subprocessadores da ByDoctor mantêm relatório SOC 2 Type II vigente.

### NGS2 / SBIS-CFM

Princípios aplicados

Adotamos os princípios do Manual de Certificação SBIS-CFM para Sistema de Registro Eletrônico em Saúde nível NGS2: autenticação forte, controle de acesso, auditoria, integridade e disponibilidade do prontuário.

## Conformidade com normas do CFM e do MS

A maior parte do que uma clínica faz hoje no Brasil — emitir receita, registrar a evolução, atender por telemedicina — está regulada pelo Conselho Federal de Medicina ou por leis federais. Mapeamos cada exigência para um controle concreto na ByDoctor.

Resolução CFM 1.821/2007

### Prontuário eletrônico do paciente

Norma do Conselho Federal de Medicina que estabelece como o prontuário eletrônico deve garantir integridade, autenticidade, confidencialidade e disponibilidade dos dados.

Como a ByDoctor aplica

- ✓Trilha de auditoria com autor, data e conteúdo da alteração
- ✓Controle de acesso por papéis com sigilo profissional preservado
- ✓Armazenamento em nuvem com criptografia e backup periódico
- ✓Possibilidade de impressão e exportação para perícia ou portabilidade

Resolução CFM 2.314/2022

### Telemedicina no Brasil

Marco vigente da telemedicina. Substituiu as Resoluções 2.227/2018 e 2.299/2021. Define teleconsulta, telediagnóstico, telecirurgia, telemonitoramento e exige consentimento informado registrado em prontuário.

Como a ByDoctor aplica

- ✓Registro do consentimento informado no prontuário do paciente
- ✓Anexo de documentos da consulta remota (áudio, vídeo, PDF)
- ✓Evolução assinada e datada após o atendimento à distância
- ✓Possibilidade de emitir receita e atestado a partir do mesmo encontro

Resolução CFM 2.217/2018

### Código de Ética Médica

Reforça o sigilo profissional como um dos pilares do exercício médico. Toda manipulação de dado clínico precisa respeitar a confidencialidade entre médico e paciente.

Como a ByDoctor aplica

- ✓Recepcionistas e Colaboradores não acessam prontuário ou prescrições
- ✓Log de acesso ao prontuário disponível para o Admin
- ✓Compartilhamento de prontuário só por ação explícita do profissional

Lei 13.787/2018

### Digitalização do prontuário do paciente

Permite o uso exclusivo do prontuário eletrônico, define a retenção mínima de 20 anos e exige sistema especializado de gerenciamento eletrônico de documentos.

Como a ByDoctor aplica

- ✓Retenção do prontuário por no mínimo 20 anos a partir do último registro
- ✓Eliminação segura ao fim do prazo, com registro em log
- ✓Backup contínuo durante toda a vida útil do prontuário

Lei 14.510/2022

### Marco legal da telessaúde

Reconhece a telessaúde como modalidade do exercício profissional em todo o território nacional, aplicável a todas as profissões da saúde regulamentadas.

Como a ByDoctor aplica

- ✓Suporte a múltiplos conselhos (CFM, CFP, CFN, COFFITO, CRO)
- ✓Atendimento ambulatorial remoto registrado como tipo de consulta
- ✓Documentos clínicos válidos para psicólogos, nutricionistas, fisioterapeutas e dentistas

## Controle de acesso por papel

| Papel | Agenda e pacientes | Prontuário e prescrição | Financeiro | Configurações |
| --- | --- | --- | --- | --- |
| Admin | Total | Total | Total | Total |
| Profissional | Própria agenda | Próprios pacientes | Visualização das próprias consultas | Não |
| Colaborador | Sim | Não | Não | Não |

A separação entre recepção e clínica evita que informação sensível circule pela equipe administrativa sem necessidade.

## Subprocessadores

Empresas que processam dados em nosso nome para que o produto funcione. Todas operam sob contrato com cláusulas de proteção de dados (DPA) e estão sujeitas aos mesmos compromissos de confidencialidade que a ByDoctor.

| Subprocessador | Função | Jurisdição |
| --- | --- | --- |
| Amazon Web Services (AWS) | Hospedagem da aplicação e do banco PostgreSQL | Brasil (São Paulo) |
| Google Cloud Storage | Armazenamento de arquivos e anexos clínicos | Brasil / EUA |
| Clerk | Autenticação, MFA, SSO e gestão de organização | EUA (cláusulas-padrão) |
| Stripe | Cobrança da assinatura ByDoctor (não processa pagamento de paciente) | EUA / Irlanda |
| MEMED | Prescrição digital com assinatura ICP-Brasil | Brasil |
| Meta — WhatsApp Business API | Mensagens automatizadas para o paciente | Brasil / EUA |
| OpenAI | Transcrição opcional de áudio da consulta (ativada por profissional) | EUA (com cláusulas-padrão e DPA) |
| Sentry + Datadog | Observabilidade técnica (sem PII clínica no payload) | EUA |
| PostHog | Analytics de produto com dados pseudonimizados | EUA / UE |
| Resend | Envio de e-mails transacionais | EUA |

## Resposta a incidentes e canal de segurança

Suspeita de vulnerabilidade, acesso indevido ou comportamento estranho na sua conta? Fale com o time de segurança diretamente:

[security@bydoctor.com.br](mailto:security@bydoctor.com.br)

Contenção

Em até 4 horas após detecção interna ou comunicação externa.

Comunicação ao controlador

Em até 24 horas, com detalhes do escopo e recomendações.

Notificação à ANPD

Em até 48 horas úteis quando houver risco relevante (Art. 48, LGPD).

## Direitos do titular dos dados

O paciente é titular dos próprios dados clínicos. O Art. 18 da LGPD garante a ele nove direitos — confirmação do tratamento, acesso, correção, anonimização, portabilidade, eliminação, informação sobre compartilhamentos, revogação de consentimento e oposição. A ByDoctor atende cada um deles em parceria com a clínica (controlador dos dados).

Veja a página dedicada à LGPD

Bases legais, prazo de retenção, dados do encarregado (DPO), modelo de exercício de direitos e processo de eliminação ficam em [/lgpd](https://bydoctor.com.br/lgpd).

## Perguntas frequentes

A ByDoctor é certificada pela SBIS?

A plataforma foi projetada seguindo os princípios do Manual de Certificação SBIS-CFM para Sistema de Registro Eletrônico em Saúde nível NGS2 — autenticação forte, controle de acesso, trilha de auditoria, integridade e disponibilidade. A certificação formal SBIS está no roadmap de 2026. Hoje, todos os controles técnicos exigidos pelo NGS2 já estão implementados.

Onde os dados clínicos ficam armazenados?

Os dados ficam em servidores da Amazon Web Services na região de São Paulo (Brasil) e em buckets de Google Cloud Storage. Os arquivos são cifrados em AES-256 em repouso e em TLS 1.3 em trânsito. Não há transferência rotineira de prontuário para fora do Brasil.

A ByDoctor segue a LGPD?

Sim. A ByDoctor é operadora dos dados, e a clínica ou o profissional contratante é o controlador, conforme definição do Art. 5º da Lei 13.709/2018. Aplicamos as bases legais do Art. 7º (II, VI, VIII) e do Art. 11, II, “a” e “f” para dados sensíveis de saúde. Detalhes completos, direitos do titular e contato do DPO estão em /lgpd.

Como funciona a trilha de auditoria?

Toda criação, alteração ou exclusão em consulta, paciente, prescrição, exame ou documento clínico fica registrada com autor, data, IP e diff do conteúdo. Apenas o perfil Admin da clínica visualiza o log completo. A retenção do log acompanha a do prontuário — no mínimo 20 anos, conforme a Lei 13.787/2018.

O que acontece em caso de incidente de segurança?

O plano de resposta da ByDoctor segue três fases: contenção em até 4 horas após detecção, comunicação ao controlador (clínica) em até 24 horas e notificação à ANPD em até 48 horas úteis quando houver risco ou dano relevante, conforme orientação do Art. 48 da LGPD. O canal dedicado é security@bydoctor.com.br.

A prescrição emitida pela ByDoctor tem validade legal?

Sim. A prescrição digital é emitida via integração oficial com a MEMED, que aplica assinatura digital com certificados ICP-Brasil. A MP 2.200-2/2001 garante que essa assinatura tem o mesmo efeito jurídico da assinatura manuscrita. A MEMED é reconhecida pelo CFM e pelo Conselho Federal de Farmácia para receituário eletrônico.

Quem pode acessar o prontuário do paciente?

Por padrão, apenas o profissional de saúde responsável pelo atendimento e o Admin da clínica acessam prontuário e prescrições. Colaboradores (recepcionistas) gerenciam agenda e cadastro do paciente, mas não enxergam o conteúdo clínico. Todo acesso fica registrado na trilha de auditoria.

A ByDoctor compartilha dados com terceiros?

Compartilhamos apenas com subprocessadores estritamente necessários para o serviço — listados nesta página. Não vendemos, não cedemos e não usamos dados clínicos para treinar modelos de IA. A transcrição opcional via OpenAI ocorre só quando o profissional ativa o recurso para um atendimento específico.

Como a clínica solicita uma cópia dos dados ou exclui a conta?

O Admin da clínica pode exportar pacientes, consultas e financeiro a qualquer momento dentro do produto. Para exclusão definitiva, basta abrir um chamado em dpo@bydoctor.com.br — a ByDoctor responde no prazo de 15 dias previsto no Art. 19 da LGPD. Os dados são eliminados de forma segura, exceto pelo que a legislação obrigar a manter.

Qual a disponibilidade do serviço?

A meta de SLA é 99,9% de uptime mensal. O status em tempo real, incidentes históricos e janelas de manutenção programada ficam disponíveis em status.bydoctor.com.br. Backups contínuos garantem RPO de até 15 minutos e RTO de até 4 horas em cenários de recuperação.

## Precisa do material para o seu time jurídico?

A ByDoctor envia o resumo de compliance, o DPA e a lista atualizada de subprocessadores para clínicas em avaliação. Basta solicitar por e-mail.

[Solicitar documentação](mailto:dpo@bydoctor.com.br?subject=Solicita%C3%A7%C3%A3o%20de%20documenta%C3%A7%C3%A3o%20de%20compliance) [Ver página de LGPD](https://bydoctor.com.br/lgpd)