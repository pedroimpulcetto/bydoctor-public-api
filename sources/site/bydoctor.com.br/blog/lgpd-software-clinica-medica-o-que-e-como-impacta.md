# Source: https://bydoctor.com.br/blog/lgpd-software-clinica-medica-o-que-e-como-impacta

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: LGPD em Clínicas Médicas: O que é e Como Afeta seu Software](https://bydoctor.com.br/_next/image?url=%2Fblog%2Flgpd-software-clinica-medica-o-que-e-como-impacta%2Ffeatured.png&w=3840&q=75)

A LGPD (Lei nº 13.709/2018) se aplica a toda clínica ou consultório que coleta, armazena ou compartilha dados de pacientes, independentemente do porte. Como dados de saúde são sensíveis (art. 11), a lei exige base legal, consentimento específico, criptografia e controle de acesso. O descumprimento pode gerar multa de até R$ 50 milhões por infração.

**LGPD** é a abreviação de Lei Geral de Proteção de Dados Pessoais (Lei nº 13.709/2018), a legislação brasileira que regula como organizações coletam, armazenam, usam e compartilham dados de pessoas físicas. Para clínicas médicas, a lei tem peso ainda maior porque dados de saúde são classificados como dados sensíveis, com exigências de proteção superiores às de categorias comuns.

O setor de saúde é um dos mais visados por ataques de ransomware e vazamentos. Segundo o relatório Cost of a Data Breach 2024 da [IBM Security](https://www.ibm.com/reports/data-breach), o custo médio de um vazamento de dados na área de saúde foi de US$ 9,77 milhões, o maior entre todos os setores pelo 14º ano consecutivo. Por concentrar dados sensíveis, uma clínica de qualquer porte é um alvo concreto — e a responsabilidade legal recai sobre ela, não sobre o invasor.

![Médica verificando conformidade de software clínica com LGPD em tablet moderno](https://bydoctor.com.br/blog/lgpd-software-clinica-medica-o-que-e-como-impacta/featured.png)

## O que a LGPD exige especificamente de clínicas médicas?

Clínicas e consultórios se enquadram como **controladores de dados** nos termos da LGPD: são eles que definem como e por quê os dados dos pacientes são tratados. O software utilizado é o **operador**, ou seja, quem executa o tratamento em nome do controlador. Essa distinção importa porque, em caso de vazamento causado por falha do software, a clínica pode ser responsabilizada perante os pacientes mesmo que a falha técnica tenha sido do fornecedor.

A lei impõe quatro obrigações principais às clínicas. Primeira, **base legal**: todo tratamento precisa de uma justificativa legal. Para dados de saúde, as bases mais usadas são o consentimento do paciente (art. 7º, I) e a tutela da saúde por profissional habilitado (art. 11, II, f). Segunda, **finalidade**: dados coletados para agendamento não podem ser usados para marketing sem nova autorização. Terceira, **transparência**: o paciente tem direito de saber quais dados são coletados, como são usados e com quem são compartilhados — o que na prática exige uma política de privacidade acessível. Quarta, **segurança**: medidas técnicas e administrativas para evitar acesso não autorizado, perda ou vazamento.

O [Conselho Federal de Medicina (CFM)](https://portal.cfm.org.br), pela Resolução CFM nº 1.821/2007, já exigia sigilo e integridade dos prontuários antes da LGPD. A lei reforça essas obrigações e adiciona direitos novos aos pacientes, como acesso, correção e exclusão dos dados.

## Dados de saúde: por que são tratados de forma diferente?

O artigo 11 da LGPD lista dados de saúde entre os chamados **dados sensíveis**, ao lado de origem racial, opinião política, crença religiosa e dados biométricos. O tratamento desses dados só é permitido em situações específicas, e o consentimento precisa ser _específico e destacado_ — não basta uma cláusula genérica no contrato de prestação de serviços.

Na prática, isso afeta a rotina de qualquer clínica. Compartilhar o prontuário de um paciente com um convênio sem autorização explícita configura infração. Enviar laudos por e-mail sem criptografia também. Até o simples fato de um recepcionista ter acesso a fichas de todos os pacientes, quando deveria ver apenas as suas, pode gerar problemas em caso de auditoria.

A tabela abaixo resume as diferenças de exigência entre dados comuns e dados sensíveis:

| Aspecto | Dados comuns (ex: nome, telefone) | Dados sensíveis (ex: diagnóstico, exames) |
| --- | --- | --- |
| Bases legais disponíveis | 10 bases (art. 7º) | 7 bases específicas (art. 11) |
| Consentimento | Livre e informado | Específico, destacado e explícito |
| Transferência internacional | Permitida com garantias | Exige aprovação adicional da ANPD |
| Impacto de vazamento | Multa + reparação de danos | Multa + reparação + possível ação penal (art. 154-A do CP) |
| Exigência de anonimização | Quando possível após prazo | Obrigatória após prazo legal de guarda |

![Profissional de saúde assinando termo de consentimento LGPD com paciente em consultório](https://bydoctor.com.br/blog/lgpd-software-clinica-medica-o-que-e-como-impacta/section_0.png)

## O que um software de clínica precisa ter para estar em conformidade com a LGPD?

Um software de gestão clínica não é apenas uma ferramenta de organização; ele é um processador de dados sensíveis operando 24 horas por dia. Escolher um sistema sem avaliar sua conformidade com a LGPD é assumir um risco que pode custar caro — tanto financeiramente quanto na relação de confiança com os pacientes.

Para o software de gestão da clínica ser um aliado e não um passivo, ele precisa reunir pelo menos estes recursos:

1. **Criptografia em trânsito e em repouso**: todos os dados devem ser transmitidos via HTTPS/TLS e armazenados com criptografia AES-256 ou equivalente. Isso torna os dados ilegíveis mesmo que um servidor seja comprometido.
2. **Controle de acesso por perfil**: cada colaborador só vê o que precisa. O recepcionista acessa a agenda; o médico, o prontuário; o financeiro, os recibos. Acesso irrestrito a todos os dados por todos os funcionários é uma violação do princípio da necessidade (art. 6º, III da LGPD).
3. **Log de auditoria**: registro automático de quem acessou, alterou ou exportou dados de pacientes, com data e hora. Esse histórico é indispensável para responder a solicitações da ANPD e identificar acessos indevidos.
4. **Acordo de Processamento de Dados (DPA)**: documento contratual em que o fornecedor do software assume as obrigações de operador de dados. Sem DPA assinado, a clínica não tem como demonstrar que cumpriu a obrigação de contratar operadores adequados.
5. **Plano de resposta a incidentes**: procedimento documentado para comunicar a ANPD e os titulares em até 3 dias úteis após tomar conhecimento de um vazamento, prazo definido pela Resolução CD/ANPD nº 15/2024.
6. **Backup com retenção e exclusão programada**: o software deve permitir definir por quanto tempo os dados ficam nos backups e eliminá-los automaticamente ao fim do prazo legal.

Use o checklist abaixo para verificar, item a item, se o software da clínica atende às exigências da LGPD:

| Requisito de conformidade | Por que importa | Base na LGPD |
| --- | --- | --- |
| Criptografia em trânsito e em repouso | Torna os dados ilegíveis mesmo se o servidor for comprometido | Art. 46 (segurança) |
| Controle de acesso por perfil | Cada colaborador vê só o necessário para sua função | Art. 6º, III (necessidade) |
| Log de auditoria | Registra quem acessou, alterou ou exportou dados, com data e hora | Art. 37 (registro das operações) |
| Acordo de Processamento de Dados (DPA) | Formaliza as obrigações do fornecedor como operador | Art. 39 (operador segue instruções) |
| Plano de resposta a incidentes | Permite comunicar a ANPD em até 3 dias úteis após o vazamento | Art. 48 + Res. CD/ANPD nº 15/2024 |
| Exclusão ou anonimização programada | Elimina dados ao fim do prazo legal de guarda, de forma rastreável | Art. 15 e 16 (término do tratamento) |

Um bom ponto de partida para avaliar um software é o [guia de escolha de sistemas para clínicas](https://bydoctor.com.br/blog/guia-completo-escolher-softwares-medicos-2026), que traz uma lista de critérios técnicos e contratuais para analisar antes de contratar. Vale também revisar como funciona o [armazenamento seguro de dados de pacientes no prontuário eletrônico](https://bydoctor.com.br/blog/prontuario-eletronico-lgpd-armazenamento-seguro-dados-paciente).

## Quais são as penalidades por descumprir a LGPD em uma clínica?

Desde agosto de 2021, a ANPD tem competência para aplicar sanções administrativas previstas no art. 52 da LGPD. As penalidades seguem uma escala progressiva, começando com advertência e podendo chegar a multa de 2% do faturamento bruto anual do grupo econômico no Brasil, limitada a R$ 50 milhões por infração.

O que muitos gestores não sabem: **cada violação é contada separadamente**. Um sistema sem criptografia que expõe 500 prontuários pode ser enquadrado como 500 infrações, cada uma com multa potencial. A ANPD publicou regulamentos sobre o cálculo das sanções disponíveis no [portal oficial da ANPD](https://www.gov.br/anpd), onde também ficam os casos julgados — úteis para entender como o órgão interpreta situações concretas.

Além das sanções administrativas, clínicas podem enfrentar ações de indenização por danos morais movidas por pacientes afetados. A jurisprudência sobre vazamentos ainda está se firmando: em casos envolvendo dados sensíveis, tribunais já reconheceram o dever de indenizar — em algumas decisões sem exigir prova do prejuízo concreto —, o que aumenta o risco de condenação da clínica.

Para consultórios menores, o risco muitas vezes não é a multa máxima, mas o custo reputacional. Pacientes que descobrem que seus dados foram expostos tendem a não retornar e a compartilhar a experiência. Em especialidades onde a relação de confiança é o principal ativo do profissional, isso pode ser mais danoso do que qualquer multa.

![Documento oficial ANPD sobre proteção de dados na área da saúde sobre mesa de trabalho](https://bydoctor.com.br/blog/lgpd-software-clinica-medica-o-que-e-como-impacta/section_1.png)

## Como avaliar se o software da sua clínica está adequado à LGPD?

Nem todo fornecedor fala abertamente sobre suas práticas de segurança. Há uma lista de perguntas que qualquer clínica deve fazer antes de contratar — e cobrar resposta documental, não apenas verbal:

- O fornecedor disponibiliza um Acordo de Processamento de Dados (DPA) para assinatura?
- Onde os dados são armazenados? (servidores no Brasil ou com garantias equivalentes conforme ANPD)
- Há criptografia AES-256 ou equivalente para dados em repouso?
- O sistema tem controle de acesso por perfil de usuário configurável?
- Existe log de auditoria com rastreabilidade de acessos e alterações?
- Qual o prazo de notificação em caso de incidente de segurança?
- O software tem certificação ou auditoria de segurança externa (ex: ISO 27001, SOC 2)?
- Como é feita a exclusão de dados após o fim do contrato?

Se o fornecedor não responde a essas perguntas com documentação, é um sinal de alerta. Clínicas que usam [prontuários eletrônicos certificados pelo CFM](https://bydoctor.com.br/blog/softwares-prontuario-eletronico-certificado-cfm) já partem de uma base melhor, pois a certificação exige critérios técnicos que se sobrepõem parcialmente às exigências da LGPD.

Para consultorios que estão passando pela [digitalização de prontuários](https://bydoctor.com.br/blog/7-erros-comuns-ao-digitalizar-prontuarios-e-como-evitar), esse momento é ideal para revisar contratos com fornecedores e garantir que os novos acordos já contemplem as obrigações da LGPD.

## Perguntas frequentes sobre LGPD e softwares de clínica médica

### A LGPD se aplica a consultórios individuais ou só a clínicas maiores?

A LGPD se aplica a qualquer pessoa física ou jurídica que trate dados de pacientes, independentemente do porte. Um consultório solo com agenda em papel ou planilha já é controlador de dados nos termos da lei e responde pelas mesmas obrigações de uma clínica com dezenas de médicos.

### Qual é a multa por descumprir a LGPD em uma clínica médica?

A ANPD pode aplicar multa de até 2% do faturamento anual da empresa no Brasil, limitada a R$ 50 milhões por infração. Além da multa, a clínica pode sofrer suspensão parcial do banco de dados e proibição de tratar dados por até seis meses, sanções independentes de ações de indenização movidas por pacientes.

### Dados de saúde têm tratamento especial na LGPD?

Sim. O artigo 11 da LGPD classifica dados de saúde como dados sensíveis, ao lado de biometria e origem racial. O tratamento exige consentimento específico e destacado do titular ou base legal própria, como a tutela da saúde por profissional habilitado. O compartilhamento com terceiros, como convênios, tem restrições adicionais.

### Por quanto tempo uma clínica pode guardar os dados de um paciente?

A Resolução CFM nº 1.821/2007 determina guarda mínima de 20 anos, a partir do último registro, para prontuários em papel; prontuários arquivados eletronicamente conforme a norma têm guarda permanente. A LGPD exige que, cumprida a finalidade e o prazo legal, os dados sejam eliminados ou anonimizados, salvo interesse legítimo documentado.

### Como saber se o software da minha clínica está adequado à LGPD?

Peça ao fornecedor um Acordo de Processamento de Dados (DPA) e confirme onde os dados ficam armazenados, se há criptografia em trânsito e em repouso, controle de acesso por perfil, logs de auditoria e plano de resposta a incidentes com prazo de notificação. Um software adequado responde a tudo isso com documentação, não apenas promessas.

## Em resumo

A LGPD obriga toda clínica a proteger dados de pacientes, que são sensíveis por definição legal (art. 11). Na prática, isso exige um software com criptografia, controle de acesso por perfil, logs de auditoria e um DPA assinado com o fornecedor. Ignorar essas medidas expõe a clínica a multas de até R$ 50 milhões e a ações de pacientes.

Se você ainda não avaliou seu sistema sob esse ângulo, o momento é agora. O ByDoctor foi desenvolvido com conformidade à LGPD desde o início, com criptografia de ponta a ponta, controle de acesso por perfil e suporte a DPA. Conheça as [funcionalidades de segurança e gestão](https://bydoctor.com.br/#funcionalidades) e veja como sua clínica pode operar com tranquilidade e dentro da lei.

## Artigos relacionados

- [Software de Clínica e LGPD: Perguntas que Médicos Fazem à ANPD](https://bydoctor.com.br/blog/software-clinica-lgpd-perguntas-medicos-anpd)
- [Como Excluir Dados de Pacientes em Conformidade com a LGPD](https://bydoctor.com.br/blog/como-excluir-dados-pacientes-lgpd)
- [Como Verificar se o Software da Sua Clínica está em Conformidade com LGPD](https://bydoctor.com.br/blog/como-verificar-conformidade-lgpd-software-clinica)