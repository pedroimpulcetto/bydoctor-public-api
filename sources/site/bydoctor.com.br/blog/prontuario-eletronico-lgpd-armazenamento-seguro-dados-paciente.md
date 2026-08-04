# Source: https://bydoctor.com.br/blog/prontuario-eletronico-lgpd-armazenamento-seguro-dados-paciente

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Prontuário Eletrônico e LGPD: Armazenamento Seguro de Dados do Paciente](https://bydoctor.com.br/_next/image?url=%2Fblog%2Fprontuario-eletronico-lgpd-armazenamento-seguro-dados-paciente%2Ffeatured.png&w=3840&q=75)

O prontuário eletrônico armazena dados de saúde — e a LGPD classifica esses dados como **sensíveis**, o que exige atenção redobrada de qualquer clínica ou consultório. Segundo a [Autoridade Nacional de Proteção de Dados (ANPD)](https://www.gov.br/anpd/pt-br), descumprimentos envolvendo dados sensíveis têm prioridade de fiscalização, com multas que podem chegar a 2% do faturamento anual. Saber o que a lei pede — e como um bom sistema ajuda a cumprir — é parte da gestão clínica responsável.

![Médica verificando conformidade de prontuário eletrônico com exigências da LGPD em tablet](https://bydoctor.com.br/blog/prontuario-eletronico-lgpd-armazenamento-seguro-dados-paciente/featured.png)

## O que a LGPD diz especificamente sobre dados de saúde?

**Dados de saúde são dados pessoais sensíveis** pela definição do art. 5º, inciso II da [Lei nº 13.709/2018 (LGPD)](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm). Isso não é detalhe burocrático. Na prática, significa que prontuários eletrônicos, histórico de diagnósticos, resultados de exames e quaisquer registros que revelem condição de saúde do paciente recebem um nível de proteção maior do que outros dados pessoais comuns.

Para tratar dados sensíveis, a clínica precisa de uma **base legal específica do art. 11** — não é possível usar as mesmas hipóteses do art. 7º que valem para dados comuns. As bases mais relevantes para clínicas são:

- **Consentimento explícito do titular** para finalidade específica: o paciente deve saber o que está autorizando, com linguagem clara
- **Tutela da saúde por profissional habilitado** ou por entidade sanitária: ampara o tratamento durante o atendimento clínico
- **Cumprimento de obrigação legal ou regulatória**: como guardar o prontuário pelo prazo mínimo do CFM
- **Proteção da vida ou da incolumidade física**: situações de emergência médica

Na rotina de consultório, a combinação mais comum é tutela da saúde (para o tratamento em si) mais consentimento documentado no cadastro inicial (para finalidades como envio de lembretes e comunicação de resultados). O ideal é ter esse consentimento registrado no prontuário eletrônico desde o primeiro atendimento — e o [guia completo de prontuário eletrônico](https://bydoctor.com.br/blog/prontuario-eletronico-guia-definitivo-medicos-clinicas) detalha como estruturar esse processo.

## Como armazenar prontuários eletrônicos de forma segura?

Armazenamento seguro de dados de saúde não é só questão de backup. A LGPD, combinada com as exigências técnicas do [Conselho Federal de Medicina (CFM)](https://portal.cfm.org.br), define um conjunto de controles mínimos que qualquer sistema de prontuário eletrônico precisa oferecer.

![Interface de sistema de prontuário eletrônico mostrando níveis de acesso e controle de permissões por usuário](https://bydoctor.com.br/blog/prontuario-eletronico-lgpd-armazenamento-seguro-dados-paciente/section_0.png)

| Controle de Segurança | O que exige na prática | Risco sem adoção |
| --- | --- | --- |
| Criptografia de dados em trânsito e em repouso | TLS 1.2+ para transmissão; AES-256 para armazenamento | Dados legíveis em caso de interceptação ou invasão |
| Controle de acesso por perfil | Médico acessa prontuário; recepcionista acessa agenda sem ver diagnóstico | Exposição de dados clínicos a quem não precisa deles |
| Log de auditoria imutável | Registro de quem acessou, alterou ou exportou cada prontuário, com data e hora | Impossibilidade de apurar responsabilidade em incidente |
| Backup automático com retenção definida | Cópias diárias, testadas periodicamente, armazenadas em local separado | Perda irreversível de histórico clínico em falha de hardware |
| Autenticação forte | Senha robusta + autenticação de dois fatores para acessar dados de pacientes | Acesso não autorizado por credencial comprometida |

O CFM, pela [Resolução nº 1.821/2007](https://portal.cfm.org.br/images/PDF/resolucao182107.pdf), exige que sistemas de prontuário eletrônico sejam certificados digitalmente para eliminar o papel — o que pressupõe infraestrutura de segurança compatível. Clínicas que usam planilhas ou documentos em nuvem sem controles adequados não atendem nem ao CFM nem à LGPD.

Para quem já usa software de gestão e quer verificar a conformidade técnica, o [checklist de conformidade LGPD para software de clínica](https://bydoctor.com.br/blog/software-clinica-lgpd-checklist-conformidade) é um ponto de partida direto.

## Por quanto tempo guardar os dados do prontuário eletrônico?

O prazo de retenção de prontuários tem resposta direta: **mínimo de 20 anos** a partir da data do último registro, para pacientes adultos, conforme a Resolução CFM nº 1.821/2007. Para menores de idade, o prazo de 20 anos começa a contar a partir da data em que o paciente completar 18 anos.

Isso cria uma situação que confunde muitos gestores: o paciente pode pedir a exclusão dos dados com base na LGPD (art. 18, IV), mas a clínica tem o direito — e a obrigação — de manter o prontuário enquanto o prazo legal não expirar. O fundamento está no art. 16 da LGPD, que permite manter dados mesmo após o fim da relação com o titular quando houver obrigação legal de guarda.

O que a clínica _não_ pode fazer é manter os dados indefinidamente após o vencimento do prazo sem razão documentada. Um bom sistema de prontuário eletrônico deve permitir configurar alertas de vencimento e executar exclusão verificável — isso é parte do que a [exclusão de dados de pacientes pela LGPD](https://bydoctor.com.br/blog/como-excluir-dados-pacientes-lgpd) exige na prática.

Para clínicas que ainda mantêm parte do arquivo em papel, a transição para o digital não elimina automaticamente o físico — o descarte de documentos de saúde tem rito próprio, incluindo destruição segura (trituração ou incineração) com registro em termo. O post sobre [prontuário eletrônico versus papel](https://bydoctor.com.br/blog/prontuario-eletronico-vs-prontuario-em-papel) detalha esse processo.

## Quais são os direitos do paciente sobre seus dados de saúde?

**O paciente tem direitos garantidos pela LGPD sobre seus dados pessoais de saúde**, e a clínica precisa ter mecanismo para atender a esses pedidos dentro do prazo. A lei não define prazo exato para resposta, mas a ANPD considera razoável entre 15 e 30 dias.

Os principais direitos que afetam a rotina de clínicas incluem:

1. **Acesso aos dados**: o paciente pode solicitar quais informações a clínica tem sobre ele. Isso inclui diagnósticos, medicamentos prescritos, histórico de consultas e dados cadastrais.
2. **Correção de dados incompletos ou incorretos**: erros em nome, data de nascimento ou contato devem ser corrigidos sem burocracia.
3. **Portabilidade**: o paciente pode pedir seus dados em formato estruturado para levar a outro serviço — o que, na prática, significa exportar o prontuário em PDF ou formato interoperável.
4. **Revogação de consentimento**: se o tratamento se basear em consentimento, o paciente pode revogar a qualquer momento — com efeito para comunicações futuras, não para o histórico já registrado.
5. **Oposição**: o paciente pode se opor a tratamentos que não atendam as bases legais aplicáveis.

Ter um fluxo documentado para receber e responder a esses pedidos não é só boa prática — é o que a ANPD verifica em casos de fiscalização. Clínicas que não conseguem demonstrar como atendem direitos de titulares enfrentam penalidades independentemente de ter sofrido vazamento ou não.

## O que é necessário em caso de vazamento de dados de prontuário?

Vazamentos envolvendo dados de saúde são classificados como incidentes de alto risco pela LGPD, o que ativa obrigações imediatas. O fluxo que a clínica precisa seguir — respaldado pelo art. 48 da LGPD e pela [Resolução CD/ANPD nº 15/2024](https://www.gov.br/anpd/pt-br/assuntos/noticias/anpd-regulamenta-a-comunicacao-de-incidente-de-seguranca) — é:

1. **Identificar o incidente**: acesso não autorizado, exposição acidental, ransomware, phishing com extração de dados — qualquer evento que comprometa dados de pacientes.
2. **Avaliar o risco em até 72 horas**: verificar a extensão do incidente e determinar se há risco ou dano relevante aos titulares.
3. **Notificar a ANPD**: pelo portal da ANPD, com descrição do incidente, categorias de dados afetados, número estimado de titulares e medidas adotadas.
4. **Comunicar os pacientes afetados**: de forma direta, clara e individualizada, quando possível. A comunicação deve descrever o que aconteceu e quais providências foram tomadas.
5. **Documentar tudo**: o registro interno do incidente deve ser mantido, incluindo linha do tempo, decisões e evidências das medidas corretivas.

![Equipe clínica reunida revisando protocolo de segurança e resposta a incidentes de dados de pacientes](https://bydoctor.com.br/blog/prontuario-eletronico-lgpd-armazenamento-seguro-dados-paciente/section_1.png)

A multa máxima por infração à LGPD é de 2% do faturamento do grupo econômico no Brasil no último exercício, limitada a R$ 50 milhões por infração. Mas além da multa, o impacto reputacional de um vazamento de dados de saúde tende a ser mais duradouro — pacientes não esquecem quando informações médicas são expostas.

Usar um software de gestão com infraestrutura segura e certificada — como o que o [ByDoctor oferece para prontuário eletrônico com requisitos CFM](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-requisitos-seguranca-certificacao) — reduz significativamente a probabilidade de incidentes e facilita a apuração quando algo acontece, graças ao log de auditoria.

## Perguntas frequentes sobre prontuário eletrônico e LGPD

### Prontuário eletrônico é dado sensível pela LGPD?

**Sim.** A LGPD (Lei nº 13.709/2018) classifica dados de saúde como dados pessoais sensíveis no art. 5º, inciso II. Isso significa que prontuários eletrônicos exigem bases legais específicas para tratamento (art. 11), maior cuidado com segurança e obrigações adicionais em caso de incidente. A ANPD pode aplicar multas de até 2% do faturamento por descumprimento.

### Por quanto tempo a clínica deve guardar o prontuário eletrônico?

O Conselho Federal de Medicina (CFM), pela Resolução nº 1.821/2007, determina prazo mínimo de **20 anos** para guarda de prontuários de adultos a partir da data do último atendimento. Para menores de idade, o prazo é de 20 anos após a maioridade. Após esse período, a clínica pode excluir os dados, documentando o processo conforme a LGPD.

### Paciente pode pedir exclusão do prontuário pela LGPD?

Não de forma irrestrita. A LGPD garante o direito à exclusão (art. 18), mas o prontuário médico é um documento legal com prazo mínimo de guarda definido pelo CFM. Enquanto o prazo de 20 anos não expirar, a clínica pode recusar a exclusão com base no cumprimento de obrigação legal — mas deve explicar isso ao paciente de forma transparente e documentada.

### Qual a base legal para armazenar dados de saúde no prontuário eletrônico?

Para dados de saúde (sensíveis), as bases legais disponíveis pelo art. 11 da LGPD incluem: consentimento explícito do titular, tutela da saúde por profissional habilitado, cumprimento de obrigação legal ou regulatória, e proteção da vida. Na prática, clínicas costumam combinar tutela da saúde com consentimento documentado no cadastro do paciente.

### O que acontece se a clínica sofrer um vazamento de dados de prontuários?

A clínica deve notificar a ANPD em até 72 horas após tomar conhecimento do incidente — exigência prevista no art. 48 da LGPD e reforçada pela Resolução CD/ANPD nº 15/2024. Também deve comunicar os pacientes afetados. Multas por descumprimento chegam a 2% do faturamento (limitadas a R$ 50 milhões por infração). Dados de saúde recebem atenção prioritária por serem sensíveis.

## Resumo

Em resumo: prontuários eletrônicos contêm dados sensíveis pela LGPD, o que exige base legal específica (art. 11), controles técnicos de segurança (criptografia, log de auditoria, acesso por perfil), prazo mínimo de guarda de 20 anos conforme o CFM, e protocolo de notificação em até 72 horas em caso de incidente. Nenhum desses requisitos é cumprido com planilhas ou soluções improvisadas.

Para colocar isso em prática, o caminho mais direto é usar um software de prontuário eletrônico que já nasce com esses controles embutidos. O ByDoctor oferece [prontuário eletrônico integrado](https://bydoctor.com.br/#funcionalidades) com controle de acesso por perfil, log de auditoria e infraestrutura em nuvem segura — o que significa que sua clínica cumpre os requisitos técnicos da LGPD sem precisar construir nada do zero. Conheça as funcionalidades e veja como funciona na prática.

## Artigos relacionados

- [Prontuário Eletrônico CFM: Mudanças na Regulamentação em 2025](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-mudancas-regulamentacao-2025)
- [Software de Clínica e LGPD: Perguntas que Médicos Fazem à ANPD](https://bydoctor.com.br/blog/software-clinica-lgpd-perguntas-medicos-anpd)