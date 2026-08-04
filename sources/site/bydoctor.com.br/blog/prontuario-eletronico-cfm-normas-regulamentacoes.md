# Source: https://bydoctor.com.br/blog/prontuario-eletronico-cfm-normas-regulamentacoes

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Prontuário Eletrônico e CFM: Tudo sobre as Normas e Regulamentações](https://bydoctor.com.br/_next/image?url=%2Fblog%2Fprontuario-eletronico-cfm-normas-regulamentacoes%2Ffeatured.png&w=3840&q=75)

O prontuário eletrônico é regulamentado no Brasil principalmente pela **Resolução CFM nº 1821/2007**, que define os requisitos técnicos para sua validade legal: certificação digital ICP-Brasil, controle de acesso por usuário, rastreabilidade de alterações e guarda mínima de 20 anos. Clínicas que usam sistemas sem esses requisitos correm risco jurídico — o prontuário pode não ter valor como prova em processos éticos ou judiciais.

**Prontuário eletrônico**, na definição do próprio CFM, é o documento único constituído por um conjunto de informações, sinais e imagens registradas, geradas a partir de fatos, acontecimentos e situações sobre a saúde do paciente e a assistência a ele prestada, de caráter legal, sigiloso e científico, que possibilita a comunicação entre membros da equipe multiprofissional e a continuidade da assistência prestada ao indivíduo — em formato digital, gerado e armazenado por sistema informatizado.

Este guia reúne o que todo médico e gestor de clínica precisa saber sobre as exigências do CFM: quais resoluções se aplicam, o que é obrigatório do ponto de vista técnico, como funciona a assinatura digital, quanto tempo os registros precisam ser mantidos e como a LGPD se articula com essas obrigações.

![Médica revisando prontuário eletrônico em laptop em consultório moderno](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-normas-regulamentacoes/featured.png)

## A Resolução CFM 1821/2007: a base de tudo

A Resolução CFM nº 1821, aprovada em 23 de novembro de 2007, é o marco regulatório central do prontuário eletrônico no Brasil. Antes dela, o uso de prontuários digitais era juridicamente incerto — não havia norma que autorizasse a eliminação do papel ou definisse critérios de validade para registros eletrônicos.

A resolução aprova as normas técnicas concernentes à digitalização e ao uso dos sistemas informatizados para a guarda e manuseio dos documentos dos prontuários dos pacientes, autorizando a eliminação do papel. O ponto central: ela **não torna o prontuário eletrônico obrigatório**, mas estabelece as condições sob as quais ele tem validade legal equivalente ao documento em papel.

Para que o prontuário eletrônico tenha essa validade, a Resolução 1821/2007 exige:

**1\. Certificação digital ICP-Brasil.** Toda entrada no prontuário precisa ser assinada digitalmente com certificado emitido por autoridade certificadora credenciada pela Infraestrutura de Chaves Públicas Brasileira (ICP-Brasil). Isso garante autoria (quem escreveu) e integridade (o conteúdo não foi alterado depois da assinatura).

**2\. Controle de acesso individualizado.** Cada profissional que acessa o sistema deve ter login próprio com senha. O acesso coletivo — uma senha compartilhada pela equipe — não é aceito porque impossibilita rastrear quem fez cada registro.

**3\. Registro de auditoria (log de acesso).** O sistema deve manter trilha de auditoria com data, hora, identificação do usuário e tipo de operação para cada acesso ou modificação nos dados. Esses logs não podem ser apagados ou editados pelos próprios usuários.

**4\. Backup periódico e recuperação de desastres.** A norma exige política de cópias de segurança documentada. Na prática, isso significa backup automático com frequência mínima diária e capacidade de restauração comprovada.

**5\. Migração de formato para preservação de longo prazo.** Durante os 20 anos de guarda obrigatória, o sistema deve garantir que os documentos permaneçam legíveis mesmo que o software original seja descontinuado. Formatos abertos (PDF/A, por exemplo) são preferíveis a formatos proprietários.

## Outras resoluções que afetam o prontuário eletrônico

A Resolução 1821/2007 é a base, mas não está sozinha. Dois outros instrumentos normativos impactam diretamente como o prontuário eletrônico deve funcionar na prática:

**Resolução CFM 2314/2022 — Telemedicina.** Com a regulamentação definitiva da telemedicina pelo CFM em 2022, ficou claro que consultas realizadas à distância geram prontuários com os mesmos requisitos das consultas presenciais. O registro do encontro clínico, o conteúdo da anamnese, as prescrições e as orientações terapêuticas precisam ser documentados com a mesma completude. A diferença está na possibilidade de usar imagens e vídeos como parte do registro clínico, desde que o sistema suporte seu armazenamento seguro.

**Resolução CFM 2056/2013 — Conselho de Ética Médica.** Esta resolução reforça que o prontuário é documento indispensável em processos ético-disciplinares. Em qualquer investigação pelo CFM ou pelos Conselhos Regionais de Medicina (CRM), o médico pode ser solicitado a apresentar os registros do atendimento em questão. Prontuários incompletos, ilegíveis ou indisponíveis dentro do prazo de guarda são considerados infração ética grave.

**Código de Ética Médica (CEM) — artigo 87.** O médico é obrigado a elaborar prontuário para cada paciente que atende. O prontuário precisa conter dados mínimos: identificação do paciente, anamnese, exame físico, hipóteses diagnósticas, diagnóstico, conduta e evolução. Deixar de registrar esses dados — seja em papel ou digital — é infração ética independente do formato.

![Profissional de saúde preenchendo prontuário eletrônico em tablet em consultório](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-normas-regulamentacoes/section_0.png)

## Assinatura digital no prontuário eletrônico: como funciona na prática

A exigência de assinatura digital é o ponto que mais gera dúvidas — e também o que mais frequentemente está ausente em sistemas mais simples.

**O que é assinatura digital ICP-Brasil.** A ICP-Brasil é a infraestrutura oficial de certificação digital do governo brasileiro. Um certificado ICP-Brasil vincula uma chave criptográfica à identidade do profissional com verificação pelo conselho de classe ou por autoridade certificadora credenciada. Quando o médico assina um registro com esse certificado, fica matematicamente comprovável que aquela pessoa específica fez aquele registro naquele momento — e que o conteúdo não foi modificado depois.

**Token ou certificado em nuvem.** Historicamente, os certificados ICP-Brasil eram emitidos em tokens físicos (pen drives criptografados) ou em cartões com chip. Mais recentemente, os certificados em nuvem (como o e-CPF A3 em nuvem) permitem assinar documentos direto do computador ou celular sem necessidade de hardware adicional. Para uso em sistemas de prontuário eletrônico, os certificados em nuvem têm a mesma validade que os físicos.

**O que acontece quando não há assinatura digital.** Um sistema que permite ao médico digitar registros sem assinatura digital ICP-Brasil produz documentos com valor probatório limitado. Em processos judiciais ou éticos, a parte contrária pode questionar a autenticidade e a integridade do registro. O prontuário pode ser considerado inconsistente como prova, mesmo que o conteúdo seja verdadeiro.

**Como identificar se seu sistema está em conformidade.** Pergunte ao fornecedor: "o sistema integra com certificados ICP-Brasil para assinatura de registros?". A resposta precisa ser afirmativa e específica — não vaga sobre "segurança dos dados". Sistemas que usam apenas login e senha para identificar o profissional não atendem ao requisito de assinatura digital da Resolução 1821/2007. O [guia de implantação do prontuário eletrônico](https://bydoctor.com.br/blog/como-implantar-prontuario-eletronico-clinica-do-zero) detalha como verificar esses aspectos antes de contratar.

## Tempo de guarda: 20 anos e as exceções importantes

O CFM determina guarda mínima de **20 anos a partir do último registro** no prontuário. Na prática, isso significa que um paciente atendido pela última vez em maio de 2026 tem seu prontuário sob obrigação de guarda até maio de 2046.

Há regras específicas para situações fora do padrão:

**Pacientes menores de idade.** Quando o atendimento ocorre enquanto o paciente é menor de 18 anos, o prazo de 20 anos só começa a contar a partir da data em que o paciente completa 18 anos — não do último atendimento. Na prática, isso significa que um atendimento feito quando o paciente tinha 5 anos precisa ser guardado até os 38 anos dele (18 + 20). Para clínicas pediátricas, isso representa um volume significativo de dados mantidos por décadas.

**Pacientes falecidos.** O prontuário deve ser mantido pelos mesmos 20 anos, a contar do último registro. Herdeiros e familiares diretos podem solicitar acesso aos registros por razões legítimas (herança, processo judicial, pesquisa médica familiar), e a clínica tem obrigação de fornecê-los dentro do período de guarda.

**Documentos de imagem (radiografias, tomografias, ultrassonografias).** As imagens de exames têm prazo de guarda específico definido pelo Colégio Brasileiro de Radiologia: mínimo de 5 anos para adultos e até os 28 anos do paciente para menores. Esses prazos são diferentes do prontuário textual — uma razão pela qual sistemas que integram imagens ao prontuário precisam de política de retenção configurável por tipo de documento.

**Documentos físicos já digitalizados.** Quando uma clínica digitaliza prontuários em papel preexistentes, os documentos físicos originais podem ser eliminados desde que a digitalização siga as normas técnicas da Resolução 1821/2007 (resolução mínima, formato, processo de indexação). Mas o prazo de guarda do arquivo digital passa a ser contado a partir da data do último registro no documento original — não da data da digitalização.

## LGPD e prontuário eletrônico: dados sensíveis de saúde

A Lei Geral de Proteção de Dados (Lei 13.709/2018) classifica dados sobre saúde como **dados sensíveis** — a categoria com maior nível de proteção na legislação. Isso impõe obrigações adicionais às clínicas que vão além do que o CFM já exige.

**Base legal para tratamento.** Para tratar dados de saúde, a clínica precisa de base legal explícita. No contexto de prontuário, as bases mais aplicáveis são: tutela da saúde (o tratamento é necessário para a prestação de serviço de saúde pelo profissional) e cumprimento de obrigação legal (as normas do CFM impõem guarda obrigatória). O consentimento do paciente, embora sempre recomendável, não é a única base possível — e na prática do atendimento clínico raramente é a base principal.

![Conceito de segurança de dados médicos com escudo digital protegendo informações de saúde](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-normas-regulamentacoes/section_1.png)

**Direitos do paciente como titular dos dados.** Pela LGPD, o paciente tem direito a: saber quais dados sobre ele estão armazenados, como são usados e com quem são compartilhados; solicitar correção de dados incorretos; solicitar portabilidade do prontuário para outro profissional ou instituição; e, em certos casos, solicitar eliminação dos dados. O prazo de guarda obrigatória do CFM (20 anos) prevalece sobre solicitações de eliminação — um conflito que a LGPD resolve em favor da norma específica de saúde.

**Compartilhamento com terceiros.** O prontuário eletrônico não pode ser compartilhado com planos de saúde, laboratórios, outros médicos ou pesquisadores sem base legal adequada. O compartilhamento para continuidade do tratamento (referência e contrarreferência entre profissionais) tem base legal na tutela da saúde. O compartilhamento para fins de auditoria de convênio tem base no cumprimento de contrato. O compartilhamento para fins comerciais — análise de dados para marketing ou pesquisa de mercado — é ilegal sem consentimento explícito do paciente.

**Encarregado de proteção de dados (DPO).** Clinicas que tratam dados sensíveis de saúde em volume significativo são obrigadas a nomear um Encarregado de Proteção de Dados (DPO), que pode ser um funcionário interno ou um serviço terceirizado. O DPO é o canal de comunicação entre a clínica, a Autoridade Nacional de Proteção de Dados (ANPD) e os pacientes. Para clínicas de pequeno porte, existem serviços de DPO compartilhado com custo acessível.

**Notificação de incidentes.** Em caso de vazamento ou acesso não autorizado a prontuários, a clínica tem 72 horas para comunicar o incidente à ANPD e, se houver risco significativo aos pacientes, notificá-los diretamente. A multa por descumprimento pode chegar a 2% do faturamento da organização, limitado a R$ 50 milhões por infração. Para uma análise mais aprofundada sobre conformidade de software com a LGPD, veja o artigo sobre [prontuário eletrônico e LGPD: armazenamento seguro de dados do paciente](https://bydoctor.com.br/blog/prontuario-eletronico-lgpd-armazenamento-seguro-dados-paciente).

## O que verificar no software antes de assinar o contrato

Conhecer a regulação é o primeiro passo. O segundo é garantir que o sistema escolhido realmente a cumpre. Estas são as perguntas que todo médico ou gestor deve fazer ao fornecedor antes de contratar:

**Sobre certificação digital e assinatura.** O sistema suporta assinatura digital com certificado ICP-Brasil? Quais tipos de certificado (A1, A3, nuvem)? O médico precisa instalar algum software adicional para assinar os registros?

**Sobre controle de acesso e logs.** Cada usuário tem login individual? O sistema gera logs de auditoria automáticos? Os logs podem ser exportados para fins de perícia? O gestor consegue ver quem acessou o prontuário de um paciente específico e quando?

**Sobre backup e continuidade.** Com que frequência o backup é realizado? Onde os dados são armazenados (servidores no Brasil ou fora)? Qual é o tempo de recuperação garantido em contrato em caso de falha do sistema?

**Sobre guarda de longo prazo.** O contrato prevê o que acontece com os dados se a clínica cancelar o serviço? Os dados são exportáveis em formato aberto (PDF/A, HL7 FHIR)? O fornecedor garante migração assistida para outro sistema?

**Sobre conformidade LGPD.** O fornecedor assina um DPA (Data Processing Agreement) formal? Ele atua como operador de dados ou como controlador? Possui política de resposta a incidentes documentada?

Um fornecedor que responde a essas perguntas com clareza e documentação tem muito mais chance de manter a clínica em conformidade do que um que usa termos vagos como "seguimos todas as normas".

## Perguntas frequentes sobre prontuário eletrônico e CFM

### O prontuário eletrônico é obrigatório no Brasil?

Não existe obrigatoriedade legal de usar prontuário eletrônico. A Resolução CFM 1821/2007 autoriza e regulamenta o uso, mas não impõe. Clínicas que preferem continuar com papel podem fazê-lo. Na prática, porém, a adoção cresce ano a ano porque os benefícios operacionais e a pressão de convênios por padronização tornam a digitalização inevitável.

### Qual resolução do CFM regulamenta o prontuário eletrônico?

A norma principal é a Resolução CFM nº 1821/2007. Ela aprova os critérios técnicos para validade do prontuário digital e autoriza a eliminação do papel. A Resolução CFM 2314/2022 complementa com diretrizes específicas para a telemedicina. O Código de Ética Médica (especialmente o artigo 87) define as obrigações de registro independentemente do formato.

### Por quanto tempo o prontuário eletrônico deve ser guardado?

O CFM determina guarda mínima de 20 anos a partir do último registro para pacientes adultos. Para pacientes que eram menores de idade durante o atendimento, o prazo se conta a partir dos 18 anos do paciente, o que pode estender significativamente o período de retenção.

### O prontuário eletrônico precisa de assinatura digital?

Sim. A Resolução 1821/2007 exige certificação digital compatível com a ICP-Brasil para que o prontuário eletrônico tenha validade legal equivalente ao documento em papel. Sistemas que usam apenas login e senha não atendem esse requisito e podem gerar problemas em processos judiciais ou éticos.

### O prontuário eletrônico pode ficar armazenado em nuvem?

Sim. O CFM permite armazenamento em nuvem desde que sejam garantidos disponibilidade, integridade, confidencialidade e rastreabilidade. O sistema deve usar criptografia em trânsito e em repouso, e o provedor precisa estar em conformidade com a LGPD — o que inclui manter servidores no Brasil ou garantir adequação para transferências internacionais de dados.

### O que acontece se o médico não mantiver o prontuário pelo prazo exigido?

A ausência do prontuário dentro do prazo de guarda é infração ética grave segundo o Código de Ética Médica. Em processos disciplinares no CFM ou nos CRMs, o médico pode sofrer penalidades que vão de advertência confidencial até cassação do registro. Em processos judiciais, a falta de prontuário pode ser interpretada pelo juiz como elemento desfavorável ao médico (inversão do ônus da prova).

## Resumo

O prontuário eletrônico no Brasil é regulamentado pela Resolução CFM 1821/2007, que exige certificação digital ICP-Brasil, controle de acesso individualizado, logs de auditoria e guarda mínima de 20 anos. A LGPD adiciona uma camada de proteção específica para dados sensíveis de saúde, com direitos aos pacientes e obrigações de notificação em caso de incidente. Escolher um software que atende a esses requisitos não é opcional — é condição para que o prontuário eletrônico tenha validade legal e para que a clínica esteja protegida em situações de auditoria, processo ético ou judicial.

O ByDoctor foi desenvolvido em conformidade com as normas do CFM e da LGPD, com suporte a certificação digital, logs de auditoria completos, armazenamento em nuvem com servidores no Brasil e exportação de dados em formatos abertos. Para ver como funciona na prática, acesse [bydoctor.com.br](https://bydoctor.com.br/) e comece um teste gratuito.

## Artigos relacionados

- [Migração de Prontuários Físicos para o Digital: Passo a Passo](https://bydoctor.com.br/blog/migracao-prontuarios-fisicos-para-digital-passo-a-passo)
- [Modelo de Prontuário Eletrônico: O Que Não Pode Faltar](https://bydoctor.com.br/blog/modelo-prontuario-eletronico-o-que-nao-pode-faltar)
- [Prontuário Eletrônico: Como Reduz Erros Médicos](https://bydoctor.com.br/blog/prontuario-eletronico-reduz-erros-medicos)