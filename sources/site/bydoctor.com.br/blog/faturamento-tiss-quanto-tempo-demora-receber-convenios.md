# Source: https://bydoctor.com.br/blog/faturamento-tiss-quanto-tempo-demora-receber-convenios

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Faturamento TISS: Quanto Tempo Demora para Receber dos Convênios?](https://bydoctor.com.br/_next/image?url=%2Fblog%2Ffaturamento-tiss-quanto-tempo-demora-receber-convenios%2Ffeatured.png&w=3840&q=75)

O convênio tem até **30 dias corridos** para pagar após aceitar o lote TISS — esse é o prazo estabelecido pela [Agência Nacional de Saúde Suplementar (ANS)](https://www.gov.br/ans/pt-br). Na prática, porém, o ciclo completo entre o envio do faturamento e o crédito na conta costuma levar de 45 a 60 dias, e pode chegar a 90 dias ou mais quando há glosas ou reenvios.

**Faturamento TISS** é o processo pelo qual clínicas e consultórios enviam eletronicamente, no padrão TISS (Troca de Informações em Saúde Suplementar), os atendimentos realizados para os beneficiários de planos de saúde, solicitando o reembolso à operadora. Cada guia dentro do lote precisa ter codificação correta, autorização válida e dados consistentes — qualquer divergência gera glosa e reinicia parte do ciclo.

Segundo a [ANS](https://www.gov.br/ans/pt-br/assuntos/prestadores), mais de 12% dos itens faturados em saúde suplementar sofrem algum tipo de glosa, o que significa que uma parte considerável da receita de cada clínica fica retida em ciclos de revisão. Entender o prazo real — e onde ele costuma travar — é o primeiro passo para encurtar esse caminho e melhorar o fluxo de caixa.

![Profissional de saúde analisando relatório de faturamento TISS em computador em ambiente clínico moderno](https://bydoctor.com.br/blog/faturamento-tiss-quanto-tempo-demora-receber-convenios/featured.png)

## Qual é o prazo legal para o convênio pagar?

A [Resolução Normativa ANS nº 395/2016](https://www.gov.br/ans/pt-br/assuntos/legislacao/resolucoes-normativas/resolucoes-normativas-2016/RN-395-de-24-de-marco-de-2016) é a principal referência regulatória. Ela estabelece que as operadoras de planos de saúde devem pagar os prestadores em até **30 dias corridos** após a aceitação eletrônica do lote TISS. Se o convênio não pagar no prazo, o prestador tem direito a multa e juros conforme o contrato de credenciamento.

O que muita equipe de faturamento não sabe: esse prazo começa a contar _após o aceite_, não após o envio. E o convênio tem até 15 dias para analisar o lote e emitir o aceite ou rejeição. Ou seja, o ciclo mínimo previsto na regulação é de 45 dias — 15 para análise e 30 para pagamento.

Na prática, porém, a linha do tempo é mais longa. Um levantamento informal entre gestores que usam o [software de faturamento TISS integrado ao prontuário](https://bydoctor.com.br/blog/software-faturamento-tiss-integrado) aponta que a maioria das clínicas só recebe em 50 a 70 dias quando o processo corre sem intercorrências.

### Por que o aceite demora mais do que 15 dias?

Alguns convênios têm sistemas internos de validação que só processam lotes em datas específicas — as chamadas **janelas de faturamento**. Enviar um lote no dia 16 quando a janela fecha no dia 15, por exemplo, significa esperar até o próximo ciclo. O que pode adicionar até 30 dias ao prazo.

- **Janela de competência fechada**: o lote fica na fila até o próximo ciclo de processamento
- **Inconsistência no XML**: o arquivo é rejeitado antes mesmo da análise de mérito — o relógio não começa a correr
- **Auditor sobrecarregado**: alguns convênios notificam glosas somente ao fim do prazo de 15 dias, mesmo tendo identificado o problema antes

Conhecer o calendário de faturamento de cada convênio com quem sua clínica trabalha é tão importante quanto preencher as guias corretamente. Muitas clínicas já documentam essas janelas em planilha — o ideal é que o sistema de gestão faça isso automaticamente.

## O que atrasa o pagamento na prática?

Glosas respondem pela maior parte dos atrasos. Uma glosa é, essencialmente, a recusa da operadora em pagar um item faturado, com justificativa técnica ou administrativa. O problema não é só o valor que fica retido: é o ciclo extra de revisão, recurso e reenvio que ela abre.

![Linha do tempo do ciclo de faturamento TISS mostrando envio análise pagamento e glosas em fluxo visual claro](https://bydoctor.com.br/blog/faturamento-tiss-quanto-tempo-demora-receber-convenios/section_0.png)

As principais causas de glosa que atrasam o pagamento, com base em análises do setor de saúde suplementar:

| Causa da Glosa | Frequência estimada | Dias adicionais ao ciclo | Solução preventiva |
| --- | --- | --- | --- |
| Código TUSS incorreto ou desatualizado | Alta — ~35% das glosas | +15 a +30 dias | Validação automática por tabela TUSS atualizada |
| Autorização prévia ausente ou vencida | Alta — ~28% das glosas | +20 a +45 dias | Checklist de autorização antes do atendimento |
| Número de carteirinha incorreto | Média — ~15% das glosas | +10 a +20 dias | Validação do cadastro na chegada do paciente |
| Quantidade acima do autorizado | Média — ~12% das glosas | +15 a +30 dias | Conferência de quantidade antes do envio do lote |
| Lote enviado fora da janela de competência | Baixa — ~10% dos casos | +20 a +30 dias | Calendário de fechamento por convênio no sistema |

Para clínicas que ainda fazem o faturamento de forma manual ou em planilha, o índice de glosas costuma ser significativamente maior. A [configuração correta do software de faturamento TISS](https://bydoctor.com.br/blog/como-reduzir-glosas-faturamento-tiss-bem-configurado) é o que diferencia uma taxa de glosa de 3% de uma de 18% — e isso representa meses de diferença no fluxo de caixa ao longo do ano.

## Como funciona o ciclo completo de pagamento?

Entender cada etapa ajuda a identificar onde o gargalo está. O ciclo padrão do faturamento TISS tem cinco fases — e o tempo total varia dependendo de quanto cada fase trava.

1. **Envio do lote**: a clínica envia o arquivo XML ao portal do convênio ou via integração de sistema. Deve ocorrer dentro da janela de competência do mês
2. **Validação técnica**: o sistema do convênio confere a estrutura do XML. Erros de formato geram rejeição imediata. Prazo: imediato a 48 horas
3. **Análise de mérito**: auditores verificam codificações, autorizações e quantidades. Prazo legal: até 15 dias corridos
4. **Notificação de resultado**: o convênio emite o espelho de pagamento, indicando itens aceitos e glosados. A partir daqui correm os 30 dias para pagamento
5. **Pagamento**: crédito em conta dos itens aceitos. Itens glosados entram em recurso e reiniciam o ciclo a partir da fase 3

Cada glosa não resolvida reinicia um subciclo. Uma única guia com dois itens glosados pode percorrer esse caminho três vezes antes de ser paga — ou encerrada como perda, se o prazo de recurso expirar.

Clínicas que usam o [guia prático de faturamento TISS passo a passo](https://bydoctor.com.br/blog/faturamento-tiss-guia-pratico-passo-a-passo-2025) como referência de processo tendem a reduzir o tempo nessas etapas porque sabem exatamente o que verificar antes do envio, não depois.

### Como o recurso de glosa altera o prazo?

A [ANS](https://www.gov.br/ans/pt-br) exige que o convênio processe o recurso em até 30 dias após o recebimento. Na prática, muitos convênios demoram até esse limite. Então, para um item glosado logo após o envio do lote, o cálculo fica: 15 dias (análise) + 15 dias (notificação de glosa) + 30 dias (recurso) + 30 dias (pagamento do recurso aceito) = **90 dias mínimos** para receber aquele item.

Por isso, evitar a glosa na origem vale muito mais do que ganhar o recurso depois. A [lista dos erros mais comuns no faturamento TISS](https://bydoctor.com.br/blog/erros-faturamento-tiss-glosas-como-evitar) é o ponto de partida para montar uma checagem pré-envio eficiente.

![Equipe de faturamento de clínica analisando glosas em tela de software com documentos médicos na mesa](https://bydoctor.com.br/blog/faturamento-tiss-quanto-tempo-demora-receber-convenios/section_1.png)

## O que fazer quando o convênio não paga no prazo?

Primeiro, confirme que o lote foi aceito — não apenas enviado. Muitos atrasos acontecem porque o arquivo foi rejeitado por erro técnico e a equipe não recebeu a notificação de rejeição. O aceite gera um protocolo que deve ser guardado como comprovante.

Se o aceite existir e o prazo de 30 dias tiver passado, o caminho é:

1. **Notificação escrita formal**: envie ao departamento de pagamentos do convênio, com número do protocolo de aceite, data e valor em aberto
2. **Registro em cartório**: para valores acima de R$ 5.000, considere a notificação extrajudicial — ela cria um registro com data certa e aumenta a pressão legal
3. **Denúncia à ANS**: a [ANS disponibiliza canal de atendimento](https://www.gov.br/ans/pt-br/canais_atendimento) (0800 701 9656) para reclamações de prestadores contra operadoras. O registro formal abre uma investigação e pode resultar em multa ao convênio
4. **Câmara de arbitragem ou via judicial**: para casos recorrentes ou valores expressivos, associações médicas como a [Associação Médica Brasileira (AMB)](https://amb.org.br) oferecem orientação jurídica especializada

O que não vale a pena: esperar passivamente. Convênios com fluxo de caixa apertado tendem a priorizar pagamentos para prestadores que cobram. Clínicas que monitoram ativamente o status de cada lote recebem mais rápido do que as que só percebem o atraso meses depois.

## Como reduzir o tempo de recebimento de forma consistente?

A resposta mais direta: elimine glosas antes que elas aconteçam. Cada ponto percentual a menos de glosa é um ciclo de revisão a menos — e isso se traduz diretamente em dias a menos para receber.

As estratégias com maior impacto no prazo de recebimento, ordenadas por facilidade de implementação:

1. **Validar carteirinha na recepção**: conferir número e validade antes do atendimento elimina a glosa por cadastro incorreto — que responde por ~15% dos casos
2. **Confirmar autorização antes do procedimento**: especialmente para procedimentos de alta complexidade, que têm regras rígidas de pré-autorização por convênio
3. **Usar tabela TUSS atualizada no sistema**: códigos desatualizados são a primeira causa de glosa. Um software integrado à tabela vigente elimina esse risco automaticamente
4. **Montar calendário de janelas de faturamento**: documentar os dias de corte de cada convênio para nunca perder a competência do mês
5. **Criar rotina de monitoramento pós-envio**: checar o status do lote 48 horas após o envio para identificar rejeições técnicas antes do prazo estourar

Clínicas que implementam essas cinco práticas relatam redução do ciclo médio de recebimento de 60 dias para 35 a 40 dias — sem negociar contratos diferentes com os convênios, apenas organizando o processo interno.

Para quem ainda faz faturamento manual, o salto mais significativo vem da adoção de um [faturamento TISS eletrônico integrado ao prontuário](https://bydoctor.com.br/blog/faturamento-tiss-eletronico-vantagens-sobre-papel), que elimina a redigitação de dados e valida automaticamente os campos antes do envio.

## Perguntas frequentes sobre prazo de pagamento dos convênios

### Quanto tempo o convênio tem para pagar após o faturamento TISS?

A ANS estabelece prazo de até **30 dias corridos** para pagamento após a aceitação do lote TISS. No entanto, o convênio tem 15 dias para analisar o lote e emitir o pagamento ou notificar glosas. Na prática, o ciclo completo — envio, análise, pagamento — costuma levar de 30 a 45 dias sem intercorrências.

### O que causa atraso no recebimento dos convênios?

As principais causas são: glosas técnicas por erros na guia, divergência de códigos TUSS, ausência de autorização prévia, lote enviado fora do prazo de competência e inconsistência no número de carteirinha do paciente. Cada glosa abre um novo ciclo de revisão que pode adicionar 15 a 30 dias ao prazo original.

### O que fazer quando o convênio não paga no prazo?

Primeiramente, verifique o status do lote no portal do convênio ou no software de faturamento. Se o lote foi aceito e o prazo de 30 dias expirou, notifique o convênio formalmente por escrito com número do protocolo e data de aceite. Casos persistentes podem ser encaminhados à ANS via Canal de Atendimento (0800 701 9656).

### Glosa suspende o pagamento do lote inteiro?

Não necessariamente. A maioria dos convênios paga os itens aceitos e suspende apenas os glosados. Mas alguns operadores retêm o lote inteiro até resolução das glosas — é importante conhecer o contrato de credenciamento para saber qual prática se aplica ao seu caso.

### Recurso de glosa tem prazo?

Sim. A [RN ANS nº 395/2016](https://www.gov.br/ans/pt-br/assuntos/legislacao/resolucoes-normativas/resolucoes-normativas-2016/RN-395-de-24-de-marco-de-2016) exige que operadoras informem o prazo para recurso de glosa, que normalmente é de 30 dias após a notificação. Após esse prazo, o item glosado pode ser considerado aceito pelo prestador. Por isso, controle rigoroso das notificações é essencial.

## Resumo

Em resumo: o prazo legal para o convênio pagar é de 30 dias após aceitar o lote TISS, mas o ciclo real — contando análise, notificação e eventual recurso de glosa — costuma girar entre 45 e 90 dias. A taxa de glosa da clínica é o principal fator que determina se o recebimento ficará no limite inferior ou superior dessa faixa.

Para encurtar esse ciclo, o caminho mais eficiente é prevenir glosas na origem: validar carteirinha, confirmar autorizações e usar um sistema com tabela TUSS atualizada. O ByDoctor integra faturamento TISS, prontuário eletrônico e agenda em um único ambiente — o que elimina a redigitação de dados e valida as guias automaticamente antes do envio. Se sua clínica ainda perde receita para glosas evitáveis, vale conhecer como essa integração funciona na prática.

## Artigos relacionados

- [Treinamento da Equipe de Faturamento TISS: Guia Prático](https://bydoctor.com.br/blog/faturamento-tiss-treinamento-equipe-faturamento)
- [Faturamento TISS e TUSS: Como Usar as Tabelas Corretamente](https://bydoctor.com.br/blog/faturamento-tiss-tuss-como-usar-as-tabelas-corretamente)
- [Faturamento TISS na Prática: Passo a Passo para Clínicas](https://bydoctor.com.br/blog/faturamento-tiss-guia-pratico-passo-a-passo-2025)