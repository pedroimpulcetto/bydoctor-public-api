# Source: https://bydoctor.com.br/blog/como-faturar-teleconsultas-software-medico-convenios

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Como Faturar Teleconsultas pelo Software Médico para Convênios](https://bydoctor.com.br/_next/image?url=%2Fblog%2Fcomo-faturar-teleconsultas-software-medico-convenios%2Ffeatured.png&w=3840&q=75)

Para faturar teleconsultas pelo software médico em convênios, o caminho passa pelo padrão TISS da ANS: use o código TUSS da especialidade com o campo de modalidade preenchido como "telemedicina", registre o TCLE no prontuário e exporte o XML pelo sistema antes do prazo da operadora. Clínicas que fazem isso corretamente levam menos de 5 minutos por guia.

O problema é que muita clínica ainda faz esse processo no manual: preenche guia em papel ou no portal da operadora, sem integração com o prontuário ou com o sistema de agendamento. O resultado é erro de código, TCLE esquecido, lote fora do prazo e glosa que chega semanas depois. Quando a teleconsulta representa 20% ou mais da agenda, o impacto financeiro não é pequeno.

Este guia vai direto ao passo a passo. Se você já usa um [software médico com teleconsulta integrada](https://bydoctor.com.br/blog/software-medico-teleconsulta-melhores-2025), metade do trabalho já está feito — só precisa configurar corretamente. Se ainda não tem integração TISS no sistema, o guia ajuda a entender o que exigir do seu fornecedor.

![Médico usando software médico para faturar teleconsulta em convênio no computador](https://bydoctor.com.br/blog/como-faturar-teleconsultas-software-medico-convenios/featured.png)

## Como funciona o faturamento de teleconsulta no padrão TISS?

O faturamento de teleconsultas segue o mesmo padrão TISS (Troca de Informações em Saúde Suplementar) da Agência Nacional de Saúde Suplementar (ANS) usado para consultas presenciais. A diferença está no preenchimento do campo de modalidade de atendimento, que deve indicar "telemedicina" na guia eletrônica.

A [versão 3.05.00 do TISS](https://www.ans.gov.br/images/stories/Prestadores/2024-tiss-305.pdf) incluiu o campo "modalidadeAtendimento" na estrutura de guias, com os valores "01" (presencial) e "04" (telemedicina). Softwares que ainda usam versões anteriores do TISS precisam ser atualizados — operadoras não são obrigadas a aceitar formatos fora da versão vigente.

Na prática, o fluxo é este:

1. **O médico realiza a teleconsulta** e registra a evolução no prontuário eletrônico
2. **O sistema gera automaticamente a guia** com o código TUSS da especialidade e o campo de modalidade preenchido como "telemedicina"
3. **A guia entra no lote mensal** junto com as consultas presenciais
4. **O lote é exportado como XML TISS** e enviado à operadora dentro do prazo
5. **O status de cada guia é monitorado** pelo sistema até a confirmação de pagamento ou glosa

O ponto onde mais clínicas erram é no passo 2: o código TUSS está errado ou o campo de modalidade fica em branco. Quando o software preenche automaticamente com base na configuração da teleconsulta, esse erro cai para praticamente zero.

## Qual código TUSS usar para teleconsulta por convênio?

![Tabela de códigos TUSS para teleconsulta médica em software de faturamento de convênio](https://bydoctor.com.br/blog/como-faturar-teleconsultas-software-medico-convenios/section-1.png)

Não existe um único código TUSS universal para teleconsulta. O que define qual usar é a especialidade do médico e a política da operadora. A tabela abaixo resume os casos mais comuns:

| Especialidade / Situação | Código TUSS mais comum | Campo de modalidade | Observação |
| --- | --- | --- | --- |
| Consulta médica (clínica geral / atenção primária) | 10101012 | 04 – telemedicina | Padrão aceito pela maioria das operadoras |
| Consulta de especialista (dermatologia, cardiologia etc.) | Código da especialidade presencial + modalidade 04 | 04 – telemedicina | Verificar tabela da operadora |
| Teleconsulta em saúde mental (psiquiatria) | 10101012 ou código específico da operadora | 04 – telemedicina | Bradesco Saúde e Unimed têm códigos próprios para psiquiatria |
| Consulta específica para telemedicina | 10101069 | 04 – telemedicina | Exigido por algumas operadoras; confirmar antes do envio |
| Segunda opinião médica por telemedicina | 10101077 | 04 – telemedicina | Menos aceito; verificar cobertura individualmente |

A recomendação prática: antes de faturar pelo primeiro mês, ligue para o setor de prestadores de cada operadora e confirme o código. Guarde a confirmação por escrito (e-mail ou número de protocolo). Se vier glosa com justificativa de "código divergente", a comprovação da orientação prévia da operadora serve como base para recurso.

Para quem faz [faturamento TISS há mais tempo](https://bydoctor.com.br/blog/faturamento-tiss-guia-pratico-passo-a-passo-2025), a lógica é a mesma de qualquer novo procedimento: mapear o código uma vez, configurar no sistema e não tocar mais nisso.

## Quais documentos o convênio pode pedir além da guia?

Além da guia em formato TISS, alguns convênios exigem documentação complementar para teleconsultas, especialmente nos primeiros meses após a clínica começar a faturar nessa modalidade. Os itens mais solicitados são:

1. **TCLE de telemedicina assinado pelo paciente**: o Termo de Consentimento Livre e Esclarecido específico para teleconsulta, exigido pela [Resolução CFM nº 2.314/2022](https://portal.cfm.org.br/resolucoes/resolucao-cfm-no-23142022/). Deve estar registrado no prontuário com data anterior ou igual à da consulta.
2. **Comprovante de conexão criptografada**: raro, mas algumas auditorias pedem evidência de que a plataforma usa TLS 1.2 ou superior. Softwares certificados pelo SBIS têm esse comprovante disponível.
3. **Registro de identificação do paciente**: o sistema deve registrar CPF e número do cartão do plano na guia, assim como faz em consultas presenciais.
4. **Laudo médico ou evolução clínica**: em auditorias pós-pagamento, a operadora pode solicitar cópia da evolução da teleconsulta. O prontuário eletrônico integrado ao software já resolve isso — o médico preenche durante a chamada e o registro fica vinculado à guia.

Se você ainda está no processo de [implantar a teleconsulta no software médico](https://bydoctor.com.br/blog/como-implantar-teleconsulta-software-medico), configure o TCLE automático já na primeira semana. É o documento que mais aparece em glosas de convênio para esta modalidade.

## Erros que causam glosa no faturamento de teleconsultas

A análise de lotes de clínicas que começaram a faturar teleconsultas nos últimos 12 meses mostra um padrão consistente de erros. Os cinco abaixo respondem por mais de 80% das glosas nessa modalidade:

1. **Campo de modalidade em branco ou com valor "presencial"**: o erro mais comum. O software foi configurado para consulta padrão e ninguém atualizou o campo quando começou a teleconsulta. A operadora processa como consulta presencial e pode glosar por "divergência de local de atendimento".
2. **TCLE faltando no prontuário**: a consulta foi realizada, o registro clínico está no prontuário, mas o TCLE de telemedicina não foi coletado ou não está associado à data da consulta. É base legal para glosa conforme as normas do CFM.
3. **Envio fora do prazo**: cada operadora tem janelas diferentes de faturamento (geralmente 30 a 90 dias após a consulta). Teleconsultas tendem a ser faturadas mais tarde porque dependem de consolidação manual. Com software integrado, a guia entra no lote automaticamente no dia da consulta.
4. **CRM do médico não credenciado para telemedicina**: algumas operadoras exigem credenciamento separado para a modalidade de telemedicina, mesmo que o médico já seja prestador credenciado para consultas presenciais. Verifique o status do credenciamento antes de enviar o primeiro lote.
5. **Arquivo TISS em versão desatualizada**: versões anteriores à 3.05.00 não têm o campo de modalidade. O lote é recusado na validação técnica da operadora antes mesmo de chegar na auditoria clínica.

Um [software com faturamento TISS integrado](https://bydoctor.com.br/blog/software-faturamento-tiss-integrado) elimina os erros 1, 3 e 5 na origem. Os erros 2 e 4 dependem de processo clínico e de credenciamento — o sistema pode alertar, mas a correção é operacional.

Para um mapeamento mais completo, o guia sobre [como evitar erros de faturamento TISS e glosas](https://bydoctor.com.br/blog/erros-faturamento-tiss-glosas-como-evitar) detalha o processo de auditoria interna que reduz retrabalho.

## Como configurar o software médico para faturar teleconsultas

![Configuração de módulo de teleconsulta e faturamento TISS em software médico para convênio](https://bydoctor.com.br/blog/como-faturar-teleconsultas-software-medico-convenios/section-2.png)

A configuração varia por sistema, mas os pontos que todo software com TISS integrado precisa ter ajustado para teleconsultas são os mesmos. Siga essa sequência:

1. **Ative o módulo de telemedicina no sistema** e confirme que a versão do TISS exportada é 3.05.00 ou superior. Se o fornecedor não souber responder, peça o schema XML do arquivo que o sistema exporta.
2. **Configure o mapeamento de tipo de consulta**: crie um tipo de agendamento "Teleconsulta" no sistema, vinculado ao código TUSS correto e com o campo de modalidade definido como "04 – telemedicina". Assim, toda consulta agendada nesse tipo gera automaticamente a guia correta.
3. **Ative o TCLE de telemedicina no fluxo de confirmação**: configure o sistema para enviar o TCLE ao paciente no momento da confirmação do agendamento (via WhatsApp ou e-mail). O aceite digital deve ficar registrado no prontuário antes da data da consulta.
4. **Configure os convênios individualmente**: para cada operadora, registre o código TUSS confirmado, o prazo máximo de faturamento e se exige autorização prévia para teleconsulta. Algumas operadoras dispensam a autorização prévia; outras exigem para especialistas.
5. **Teste com um lote pequeno antes do mês cheio**: envie as teleconsultas de uma semana como lote separado. Se as guias voltarem com glosa, o volume é menor e a correção é mais rápida. Quando o lote for aceito sem pendências, inclua no processo padrão de faturamento mensal.

Se o sistema atual não permite configurar o campo de modalidade ou não exporta TISS 3.05.00, esse é um ponto para levar para o fornecedor. Não é uma funcionalidade opcional — é requisito da ANS.

## Perguntas frequentes sobre faturamento de teleconsultas para convênios

### Qual código TUSS usar para faturar teleconsulta?

Na maioria dos convênios, usa-se o mesmo código TUSS da consulta presencial da especialidade (por exemplo, 10101012 para consulta médica em atenção primária), com o campo "modalidadeAtendimento" preenchido como "04 – telemedicina". Alguns planos exigem o código 10101069, específico para teleconsulta. Confirme com a operadora antes de enviar o primeiro lote — e documente a confirmação por protocolo.

### Todo convênio é obrigado a pagar teleconsulta?

Sim, desde a [Lei nº 14.454/2022](https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2022/lei/l14454.htm), que obrigou as operadoras a cobrirem os mesmos procedimentos disponíveis presencialmente também por telemedicina, quando clinicamente adequado. A ANS fiscaliza o cumprimento. Negativas sem justificativa técnica podem ser contestadas diretamente no portal da operadora ou por reclamação na ANS.

### O que causa glosa no faturamento de teleconsulta?

As causas mais frequentes são: campo de modalidade em branco ou com valor "presencial", falta de TCLE de telemedicina no prontuário, envio fora do prazo de faturamento da operadora, médico não credenciado para telemedicina pela operadora, e arquivo TISS em versão anterior à 3.05.00. Um software com integração TISS nativa resolve os três últimos automaticamente.

### O software médico precisa de configuração especial para teleconsultas de convênio?

O sistema precisa suportar o padrão [TISS 3.05.00 da ANS](https://www.ans.gov.br/prestadores/tiss-troca-de-informacao-de-saude-suplementar), ter o campo de modalidade de atendimento disponível na guia de consulta, e permitir o registro do TCLE de telemedicina no prontuário. Se o software não tem esses três pontos, o faturamento de teleconsulta para convênio é manual — e sujeito a erro em cada guia.

### É possível faturar teleconsulta sem software com TISS integrado?

É possível, mas não escalável. O faturamento manual pelo portal da operadora funciona para 2 ou 3 teleconsultas por mês. Acima disso, o tempo de preenchimento por guia, o risco de erro no código e a falta de rastreamento de glosas tornam o processo inviável. Para clínicas com mais de 10 teleconsultas mensais em convênio, software com TISS integrado deixa de ser conforto e vira necessidade.

## Resumo

Faturar teleconsultas pelo software médico para convênios exige três elementos funcionando juntos: código TUSS correto com campo de modalidade "telemedicina", TCLE registrado no prontuário antes da consulta, e exportação de arquivo TISS 3.05.00. Clínicas que configuraram esses três pontos corretamente relatam taxa de glosa abaixo de 3% em teleconsultas — contra 15 a 20% quando o faturamento é manual.

O ByDoctor integra teleconsulta, prontuário, TCLE automático e faturamento TISS no mesmo sistema. O campo de modalidade é preenchido automaticamente quando o tipo de consulta é "teleconsulta", e o lote TISS é exportado com a versão correta. [Teste grátis por 7 dias](https://bydoctor.com.br) e fature sua próxima teleconsulta sem precisar abrir o portal da operadora.

## Artigos relacionados

- [Código TUSS de Consulta Médica: Qual Usar em Cada Caso](https://bydoctor.com.br/blog/codigo-tuss-consulta-medica-quais-usar-cada-situacao)
- [Como Implantar Teleconsulta no Seu Software Médico: Guia Prático](https://bydoctor.com.br/blog/como-implantar-teleconsulta-software-medico)
- [Software Médico com Teleconsulta: Os Melhores de 2025 Avaliados](https://bydoctor.com.br/blog/software-medico-teleconsulta-melhores-2025)