# Source: https://bydoctor.com.br/blog/faturamento-tiss-tuss-como-usar-as-tabelas-corretamente

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Faturamento TISS e TUSS: Como Usar as Tabelas Corretamente](https://bydoctor.com.br/_next/image?url=%2Fblog%2Ffaturamento-tiss-tuss-como-usar-as-tabelas-corretamente%2Ffeatured.png&w=3840&q=75)

Para fazer o faturamento TISS de uma clínica sem gerar glosas, você precisa entender dois elementos distintos: o padrão de comunicação (TISS) e a tabela de códigos de procedimentos (TUSS). Confundir os dois — ou usar um código TUSS desatualizado — é uma das causas mais frequentes de rejeição de guias por operadoras de saúde.

**TISS (Troca de Informações em Saúde Suplementar)** é o padrão técnico definido pela [Agência Nacional de Saúde Suplementar (ANS)](https://www.gov.br/ans/pt-br) para a troca eletrônica de informações entre prestadores de saúde e operadoras. O padrão define o formato dos arquivos XML, os tipos de guia (consulta, SP/SADT, internação, honorários) e as regras de validação. **TUSS (Terminologia Unificada da Saúde Suplementar)** é a tabela de nomenclatura de procedimentos — os códigos de 8 dígitos que identificam cada exame, consulta ou cirurgia dentro dos documentos TISS.

Dados consolidados de operadoras do setor indicam que erros de código de procedimento respondem por cerca de 30% das glosas técnicas em faturamento de convênios. Para clínicas que faturam acima de R$ 50.000 mensais em convênios, isso pode representar perdas de R$ 5.000 a R$ 15.000 em receita retida por mês — a maioria por erros que um processo de conferência simples resolveria.

![Profissional de faturamento clínico consultando tabela TUSS no computador com guias médicas na mesa](https://bydoctor.com.br/blog/faturamento-tiss-tuss-como-usar-as-tabelas-corretamente/featured.png)

## Qual a diferença entre TISS e TUSS?

TISS é o padrão de comunicação — o "idioma" que prestadores e operadoras usam para trocar documentos eletrônicos. TUSS é o dicionário desse idioma: a lista de todos os procedimentos com seus respectivos códigos. Você não pode ter um sem o outro.

Uma guia TISS de consulta, por exemplo, contém campos obrigatórios como o código do prestador, a data de atendimento, o CID-10 e o código do procedimento realizado. Esse último campo usa obrigatoriamente um código TUSS — e se o código não existir na versão TISS vigente, a guia é rejeitada na validação técnica antes mesmo de chegar ao faturista da operadora.

Para entender melhor o funcionamento completo do padrão de comunicação, o post [faturamento TISS: o que é e por que é essencial para sua clínica](https://bydoctor.com.br/blog/faturamento-tiss-clinica-o-que-e-guia-completo) explica a estrutura dos documentos desde o credenciamento. Aqui o foco é específico: como usar os códigos TUSS de forma correta.

### A estrutura do código TUSS

Todo código TUSS tem 8 dígitos numéricos. A estrutura não é aleatória: os primeiros dois dígitos identificam o grupo de procedimento (ex.: 30 para consultas, 40 para exames de diagnóstico, 50 para cirurgias). O detalhamento aumenta conforme os dígitos seguintes.

Um exemplo: o código **30101012** corresponde à consulta médica em consultório pelo médico assistente. O código **40308019** corresponde à eletrocardiograma (ECG). Esses dois exemplos ilustram como a tabela funciona na prática — cada procedimento tem uma identificação única que a operadora usa para autorizar, pagar e auditar.

Antes da TUSS, as clínicas usavam a [Classificação Brasileira Hierarquizada de Procedimentos Médicos (CBHPM)](https://portal.cfm.org.br) — uma tabela mantida pelo Conselho Federal de Medicina (CFM) e pela Associação Médica Brasileira (AMB). A transição para a TUSS foi gradual e ainda há contratos de convênio antigos que referenciam códigos CBHPM. Quando isso acontece, o sistema de faturamento precisa fazer a correspondência entre os dois padrões.

## Como consultar e usar a tabela TUSS corretamente

![Tela de sistema de faturamento mostrando busca de código TUSS para procedimento médico com resultado validado](https://bydoctor.com.br/blog/faturamento-tiss-tuss-como-usar-as-tabelas-corretamente/section_0.png)

A tabela TUSS oficial está disponível no portal da [ANS](https://www.gov.br/ans/pt-br/assuntos/prestadores/padrao-para-troca-de-informacao-de-saude-suplementar-2013-tiss). O arquivo é publicado em formato de planilha e atualizado conforme novas versões do padrão TISS são liberadas. A versão vigente do padrão é a 3.05.00.

O processo de busca do código correto segue quatro etapas:

1. **Identifique o procedimento pelo nome clínico**: use a descrição técnica do exame ou cirurgia, não o nome popular. "Hemograma completo" tem um código diferente de "hemograma com contagem diferencial de leucócitos".
2. **Verifique o status do código**: códigos podem ser ativos, inativos ou migrados para outro código. Usar um código inativo gera rejeição imediata.
3. **Confirme a compatibilidade com a especialidade**: algumas operadoras só aceitam determinados códigos TUSS quando o prestador está habilitado na especialidade correspondente. Um cardiologista não pode faturar um procedimento de neurologia, mesmo que o código TUSS exista.
4. **Verifique a compatibilidade com o CID-10**: guias de SADT e internação exigem coerência entre o diagnóstico (CID-10) e o procedimento (TUSS). A rejeição por incompatibilidade CID-TUSS é frequente e fácil de evitar com uma tabela de compatibilidade atualizada. O post sobre [CID-10 para convênios: códigos aceitos e rejeitados](https://bydoctor.com.br/blog/cid-10-para-convenios-codigos-aceitos-e-rejeitados) detalha as combinações mais comuns de rejeição.

Em clínicas com volume alto de guias, fazer essa verificação manualmente para cada procedimento é inviável. Sistemas de faturamento integrados ao TISS fazem a validação automaticamente no momento do lançamento — antes do envio da guia à operadora.

## Comparativo: TUSS, CBHPM e tabelas próprias de operadoras

Uma fonte recorrente de confusão no faturamento de convênios é entender qual tabela está sendo usada em cada contexto. O quadro abaixo resume as diferenças:

| Tabela | Mantida por | Uso no faturamento TISS | Situação atual |
| --- | --- | --- | --- |
| TUSS | ANS | Obrigatória em todos os documentos TISS desde 2012 | Vigente — versão atualizada periodicamente |
| CBHPM | CFM / AMB | Referência de precificação em contratos antigos; não substitui TUSS no XML | Usada como referência de valor; não é o código do arquivo |
| Tabela própria da operadora | Cada operadora (Unimed, SulAmérica, etc.) | Define os valores pagos por código TUSS — não muda o código em si | Vigente — varia por contrato e especialidade |
| AMB (Associação Médica Brasileira) | AMB | Base histórica de codificação; migrada para TUSS | Em desuso no faturamento eletrônico |

O ponto mais importante da tabela acima: o código TUSS identifica o procedimento, mas o valor pago por ele depende da tabela de honorários do seu contrato com cada operadora. Uma consulta com código TUSS 30101012 pode ser remunerada em R$ 42 por uma operadora e R$ 67 por outra — tudo depende do contrato negociado.

Isso significa que conferir a tabela de preços do contrato é tão importante quanto conferir o código correto. Para entender como as versões do padrão impactam os contratos existentes, o post sobre [diferença entre as versões TISS 3.04, 3.05 e a versão atual](https://bydoctor.com.br/blog/faturamento-tiss-versoes-diferencas) detalha o que mudou em cada atualização e quais campos foram afetados.

## Quais erros de TUSS geram mais glosas?

![Relatório de glosas de faturamento médico com destaque em erros de código TUSS em planilha clínica](https://bydoctor.com.br/blog/faturamento-tiss-tuss-como-usar-as-tabelas-corretamente/section_1.png)

Glosa por erro de código TUSS acontece em padrões bem definidos. Os cinco erros mais frequentes, em ordem de ocorrência:

1. **Código inativo**: o procedimento foi descontinuado ou migrado para outro código em uma atualização da tabela TUSS, mas o sistema de faturamento não foi atualizado. Resultado: rejeição automática na validação do XML.

2. **Código incompatível com a especialidade do prestador**: a operadora só aceita aquele código TUSS quando o CRM e a especialidade cadastrada batem com o procedimento. Isso varia por contrato — e muitas clínicas descobrem a incompatibilidade só depois da glosa.

3. **Código divergente do CID-10**: em guias de SADT, a operadora cruza o CID-10 informado com o procedimento realizado. Pedir um ecocardiograma com CID de dermatite vai ser glosado. O alinhamento CID-TUSS precisa fazer sentido clínico.

4. **Código correto, mas versão TISS desatualizada**: o código existe, mas o arquivo XML foi gerado no padrão 3.04 enquanto a operadora já exige 3.05. O erro aparece no nível do envelope, não do código, mas o resultado é o mesmo: guia rejeitada.

5. **Uso de código genérico quando existe código específico**: algumas equipes de faturamento usam um código de procedimento genérico (ex.: "outros procedimentos") para evitar dúvida sobre qual código usar. Operadoras auditam esse padrão e tendem a glosar guias com alta concentração de códigos inespecíficos.

Para uma análise completa de como corrigir glosas já geradas e evitar as recorrentes, o post [como reduzir glosas com o faturamento TISS bem configurado](https://bydoctor.com.br/blog/como-reduzir-glosas-faturamento-tiss-bem-configurado) traz o protocolo de revisão passo a passo.

## Perguntas frequentes sobre TISS e TUSS

### Qual a diferença entre TISS e TUSS?

**TISS é o padrão técnico de comunicação eletrônica** entre prestadores e operadoras de saúde, estabelecido pela ANS por meio da [Resolução Normativa nº 305/2012](https://www.gov.br/ans/pt-br). TUSS é a tabela de códigos de procedimentos usada dentro dos documentos TISS. Em termos práticos: o arquivo TISS é o container; o código TUSS é o conteúdo que identifica o que foi realizado.

### Como encontrar o código TUSS correto para um procedimento?

**Acesse a tabela TUSS atualizada no portal da ANS**, localize o procedimento pelo nome técnico ou pela especialidade e verifique se o código está ativo na versão TISS vigente. Sistemas de faturamento que integram a tabela TUSS internamente atualizam os códigos a cada nova versão, eliminando a consulta manual e reduzindo o risco de usar um código inativo.

### O que acontece se eu usar um código TUSS incorreto na guia?

**A guia é glosada** — total ou parcialmente — pela operadora. O motivo mais comum de glosa por código é o uso de um código inativo, incompatível com a especialidade do prestador ou divergente do CID-10 informado. Dados do setor indicam que cerca de 30% das glosas técnicas têm origem em erro de código TUSS, a maioria evitável com validação automática antes do envio.

### A tabela TUSS é igual para todos os convênios?

**A tabela TUSS é padronizada pela ANS e serve como base comum para todos os convênios.** O que varia entre operadoras é a tabela de honorários: o valor pago por cada código TUSS pode diferir significativamente de um contrato para outro. O código identifica o procedimento; o preço é definido em contrato separado.

### Com que frequência a tabela TUSS é atualizada?

**A ANS atualiza a tabela TUSS em média uma a duas vezes por ano**, geralmente junto com novas versões do padrão TISS. As atualizações incluem novos códigos para procedimentos recentemente reconhecidos, inativação de códigos obsoletos e ajustes de nomenclatura. Clínicas que usam sistemas de faturamento integrados recebem essas atualizações automaticamente.

## Resumo

TISS é o padrão eletrônico de troca de documentos entre prestadores e operadoras; TUSS é a tabela de códigos de procedimentos usada dentro desses documentos. Para faturar corretamente, a clínica precisa usar o código TUSS ativo, compatível com a especialidade do prestador e coerente com o CID-10 — tudo isso dentro de um arquivo XML gerado na versão TISS vigente (atualmente 3.05.00). Os cinco erros mais comuns — código inativo, incompatibilidade de especialidade, divergência CID-TUSS, versão desatualizada e código genérico — respondem pela maioria das glosas técnicas evitáveis.

A forma mais confiável de garantir esse alinhamento é usar um [software de faturamento TISS integrado](https://bydoctor.com.br/blog/software-faturamento-tiss-integrado) que atualize a tabela TUSS automaticamente e valide os campos antes do envio. O [ByDoctor](https://bydoctor.com.br/) faz essa validação em tempo real no módulo de faturamento — antes de a guia sair do sistema, os campos críticos já foram conferidos contra a versão TISS vigente e as regras de compatibilidade da operadora.

## Artigos relacionados

- [Tabela TUSS: O Que É e Como Usar os Códigos no Faturamento](https://bydoctor.com.br/blog/tabela-tuss-o-que-e-como-usar-codigos-faturamento)
- [Treinamento da Equipe de Faturamento TISS: Guia Prático](https://bydoctor.com.br/blog/faturamento-tiss-treinamento-equipe-faturamento)
- [Faturamento TISS: Quanto Tempo Demora para Receber dos Convênios?](https://bydoctor.com.br/blog/faturamento-tiss-quanto-tempo-demora-receber-convenios)