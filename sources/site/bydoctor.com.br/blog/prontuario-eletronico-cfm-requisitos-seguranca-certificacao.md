# Source: https://bydoctor.com.br/blog/prontuario-eletronico-cfm-requisitos-seguranca-certificacao

[Voltar ao Blog](https://bydoctor.com.br/blog)

![Capa: Prontuário Eletrônico e CFM: Requisitos de Segurança e Certificação](https://bydoctor.com.br/_next/image?url=%2Fblog%2Fprontuario-eletronico-cfm-requisitos-seguranca-certificacao%2Ffeatured.png&w=3840&q=75)

O prontuário eletrônico tem validade legal no Brasil quando atende aos requisitos da **Resolução CFM nº 1.821/2007** e ao Manual de Certificação para Sistemas de Registro Eletrônico em Saúde, publicado em conjunto pelo [Conselho Federal de Medicina (CFM)](https://portal.cfm.org.br) e pela Sociedade Brasileira de Informática em Saúde (SBIS). Os dois documentos definem os critérios técnicos de segurança, os níveis de certificação e as condições sob as quais o registro digital substitui o papel — com ou sem assinatura digital ICP-Brasil.

**Prontuário eletrônico CFM-conforme** é o sistema de registro digital de saúde que segue os requisitos técnicos estabelecidos pelo Conselho Federal de Medicina, incluindo controle de acesso por profissional, log de auditoria imutável, criptografia de dados e, dependendo do nível de certificação SBIS, assinatura digital com certificado ICP-Brasil. Sem atender a esses critérios, o prontuário digital não substitui legalmente o papel.

Segundo o [portal do CFM](https://portal.cfm.org.br), mais de 260 mil médicos estão registrados no Brasil. A maioria das clínicas que adotaram sistemas digitais nos últimos anos o fez sem verificar o nível de certificação — o que cria um risco jurídico real: o prontuário em papel ainda é tecnicamente obrigatório quando o sistema não alcança o nível NGS3. Para entender quais softwares já possuem essa certificação, veja [os sistemas de prontuário eletrônico certificados pelo CFM](https://bydoctor.com.br/blog/softwares-prontuario-eletronico-certificado-cfm).

![Médica consultando prontuário eletrônico em tablet em consultório moderno com iluminação natural](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-requisitos-seguranca-certificacao/featured.png)

## O que diz a Resolução CFM nº 1.821/2007 sobre segurança?

A Resolução CFM nº 1.821/2007 é o documento que tornou legal a eliminação do prontuário em papel no Brasil — mas com condições específicas. Ela não proíbe o uso de sistemas digitais simples; estabelece que apenas os sistemas que atendam aos requisitos técnicos do Manual de Certificação SBIS/CFM podem prescindir do registro físico.

Os requisitos de segurança listados na resolução e no manual técnico são claros. O sistema precisa garantir: autenticação individual de cada profissional que acessa o prontuário, registro imutável de todas as ações (quem acessou, quando, o que alterou), criptografia dos dados durante o armazenamento e a transmissão, e backup automático com redundância geográfica. Para o nível mais alto de certificação, a assinatura digital com certificado emitido pela [Infraestrutura de Chaves Públicas Brasileira (ICP-Brasil)](https://www.iti.gov.br) é obrigatória.

O ponto que muitas clínicas ignoram: a resolução exige que o sistema seja capaz de recuperar e imprimir o prontuário em formato legível a qualquer momento, mesmo que o software original não esteja mais disponível. Isso significa que os dados precisam estar em formato aberto ou exportável — não pode haver aprisionamento de dados que impeça a portabilidade.

### O que é o Manual de Certificação SBIS/CFM?

O Manual de Certificação para Sistemas de Registro Eletrônico em Saúde é o documento técnico elaborado pela [Sociedade Brasileira de Informática em Saúde (SBIS)](https://www.sbis.org.br) em parceria com o CFM. Ele define os requisitos funcionais e de segurança que um sistema deve cumprir para cada nível de certificação (NGS1, NGS2 e NGS3) e é a base para o processo de auditoria e aprovação dos softwares.

A SBIS conduz os testes e concede a certificação. O CFM reconhece a certificação SBIS como evidência de conformidade com a Resolução nº 1.821/2007. Sem esse processo formal, o fornecedor pode afirmar que seu sistema é "CFM-compatível", mas sem auditoria independente essa afirmação não tem valor jurídico.

## Quais são os três níveis de certificação SBIS e o que cada um permite?

Os níveis de Garantia de Segurança (NGS) definem o que o sistema pode legalmente fazer. Escolher o nível errado significa manter obrigações operacionais — como o arquivo físico — que poderiam ser eliminadas com um sistema mais completo.

| Nível | O que permite | Assinatura Digital ICP-Brasil | Elimina o papel? |
| --- | --- | --- | --- |
| **NGS1** | Registro digital como apoio — o papel ainda é obrigatório | Não exigida | Não |
| **NGS2** | Substitui o papel para registros não assinados (anotações, anamneses) | Opcional para alguns documentos | Parcialmente |
| **NGS3** | Substitui integralmente o papel, incluindo documentos com validade jurídica | Obrigatória com certificado ICP-Brasil | Sim, totalmente |

A maioria dos softwares de gestão clínica disponíveis no mercado brasileiro opera em nível NGS1 — suficiente para digitalizar a rotina, mas insuficiente para eliminar o arquivo físico. Clínicas que querem atingir conformidade total e eliminar o custo e o risco do papel precisam de um sistema NGS3 ou de um módulo de assinatura digital integrado a um sistema NGS2.

Para [prescrições digitais com validade legal](https://bydoctor.com.br/blog/prescricao-digital-cinco-passos-para-implementar-com-seguranca), o requisito de assinatura ICP-Brasil também se aplica — o documento precisa ser assinado pelo médico com certificado digital emitido por uma Autoridade Certificadora credenciada pelo [Instituto Nacional de Tecnologia da Informação (ITI)](https://www.iti.gov.br).

![Diagrama comparativo dos três níveis de certificação SBIS para prontuário eletrônico em clínica médica](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-requisitos-seguranca-certificacao/section_0.png)

## Como a LGPD se aplica ao prontuário eletrônico da clínica?

A **Lei Geral de Proteção de Dados (Lei nº 13.709/2018)** trata dados de saúde como dados pessoais sensíveis — a categoria com maior nível de proteção na legislação brasileira. Isso impõe obrigações que vão além do que o CFM exige em termos técnicos de segurança: agora há regras sobre coleta, uso, compartilhamento e descarte dos dados clínicos dos pacientes.

Para o prontuário eletrônico, as principais exigências da LGPD se traduzem em quatro práticas concretas. Primeiro, o consentimento do paciente para o tratamento dos dados deve ser registrado de forma documentada — o sistema precisa guardar quando e como o paciente autorizou o uso das suas informações. Segundo, o acesso ao prontuário deve ser restrito por perfil: o recepcionista não precisa ver o histórico clínico completo, só os dados de agendamento. Terceiro, qualquer incidente de segurança que envolva dados de saúde deve ser notificado à Autoridade Nacional de Proteção de Dados (ANPD) em até 72 horas. Quarto, o paciente tem o direito de solicitar a exclusão ou portabilidade dos seus dados — e o sistema precisa ser capaz de atender a essa solicitação.

O ponto de interseção entre LGPD e CFM é o log de auditoria: ambas as normas exigem rastreabilidade total de quem acessou o quê e quando. Um sistema sem log de acesso estruturado está em desconformidade com as duas regulamentações simultaneamente. Para um guia mais detalhado sobre o tema, veja [como a LGPD impacta o software da sua clínica](https://bydoctor.com.br/blog/lgpd-software-clinica-medica-o-que-e-como-impacta).

## Checklist de segurança: o que o prontuário eletrônico da sua clínica deve ter

Antes de assumir que o sistema atual está em conformidade, vale revisar item a item. A maioria dos contratos com fornecedores de software médico não especifica o nível de certificação SBIS — e "atende ao CFM" sem mais detalhes não é uma garantia verificável.

- **Autenticação individual por profissional:** cada médico, enfermeiro ou secretária deve ter login próprio. Senhas compartilhadas invalidam o log de auditoria.

- **Log de auditoria imutável:** o sistema deve registrar automaticamente cada acesso, alteração e exportação de dados do prontuário, com data, hora e identificação do usuário. Esse registro não pode ser editado nem excluído.

- **Criptografia em repouso e em trânsito:** os dados armazenados no servidor devem ser criptografados (padrão AES-256 ou equivalente), assim como a comunicação entre o dispositivo do usuário e o servidor (protocolo TLS 1.2 ou superior).

- **Backup automático com redundância:** o sistema deve fazer cópias de segurança automáticas em intervalos definidos, com pelo menos uma cópia em localização geográfica diferente do servidor principal.

- **Controle de acesso por perfil:** cada cargo ou especialidade deve ter permissões específicas. O sistema deve impedir que um usuário acesse prontuários de pacientes que não são seus, salvo em situações de emergência documentadas.

- **Exportação dos dados em formato aberto:** o prontuário deve poder ser exportado em PDF ou XML a qualquer momento, sem dependência do fornecedor para leitura futura dos registros.

- **Assinatura digital ICP-Brasil (para NGS3):** necessária para que o prontuário digital substitua completamente o papel e para prescrições com validade jurídica plena.

Verificar esses itens com o fornecedor — por escrito, no contrato — é o caminho mais direto para saber em qual nível de certificação o sistema opera. Se o fornecedor não souber responder sobre o nível NGS, esse dado já é relevante.

![Profissional de saúde revisando checklist de conformidade de prontuário eletrônico em tela de computador](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-requisitos-seguranca-certificacao/section_1.png)

## Por quanto tempo a clínica deve guardar o prontuário eletrônico?

A Resolução CFM nº 1.821/2007 define o prazo mínimo de guarda em 20 anos a partir do último registro para pacientes adultos. Para pacientes menores de idade, o prazo é de 20 anos contados a partir do décimo oitavo aniversário. Na prática, muitas clínicas guardam prontuários por mais tempo — especialmente em especialidades como oncologia, cardiologia e psiquiatria, onde o histórico longitudinal tem valor clínico direto.

O prontuário eletrônico resolve esse problema sem custo adicional de espaço físico. Um sistema bem configurado arquiva automaticamente registros fora do período ativo e os mantém acessíveis para consulta futura sem ocupar a interface principal do sistema. A diferença em relação ao papel é concreta: um arquivo com 15 anos de prontuários de uma clínica de médio porte ocupa centenas de metros quadrados; no sistema digital, o mesmo histórico está em alguns gigabytes de armazenamento em nuvem.

Um detalhe que passa despercebido: se a clínica trocar de sistema, ela tem obrigação legal de manter o acesso aos prontuários antigos. Isso significa que, ao migrar de software, é necessário exportar todos os dados em formato legível e garantir que o novo sistema os importe corretamente — ou que o sistema anterior continue acessível para consulta, mesmo sem uso ativo. Para clínicas que estão nesse processo, veja [o guia de migração de sistema de consultório médico](https://bydoctor.com.br/blog/guia-migracao-sistema-consultorio-medico).

## Perguntas frequentes sobre prontuário eletrônico e CFM

### O prontuário eletrônico precisa de assinatura digital ICP-Brasil?

Sim, para substituir legalmente o papel. A Resolução CFM nº 1.821/2007 exige assinatura digital com certificado ICP-Brasil para sistemas que operam em nível NGS3 — o único nível que elimina completamente o prontuário físico. Sistemas NGS1 e NGS2 podem operar sem assinatura ICP-Brasil, mas o papel ainda é necessário para parte ou totalidade dos registros. A certificação pode ser obtida por meio de Autoridades Certificadoras credenciadas pelo [ITI](https://www.iti.gov.br), com custo que varia entre R$ 150 e R$ 400 por certificado anual.

### Qual a diferença entre NGS1, NGS2 e NGS3?

NGS1 é o nível básico: o sistema apoia o registro digital, mas o prontuário em papel ainda é legalmente necessário. NGS2 permite eliminar o papel para registros não assinados — como anamneses e evoluções de rotina. NGS3 é o nível completo: substitui integralmente o papel, exige assinatura ICP-Brasil e garante rastreabilidade total. A maioria dos softwares de gestão clínica do mercado opera em NGS1 ou NGS2. Para saber quais têm certificação NGS3, consulte a lista em [softwares com prontuário eletrônico certificado pelo CFM](https://bydoctor.com.br/blog/softwares-prontuario-eletronico-certificado-cfm).

### O que o CFM exige em termos de segurança para o prontuário eletrônico?

O CFM, por meio da Resolução nº 1.821/2007 e do Manual de Certificação SBIS, exige: autenticação individual por profissional, log de auditoria imutável, criptografia dos dados armazenados e transmitidos, backup automático com redundância e controle de acesso por perfil. Para nível NGS3, assinatura digital ICP-Brasil é obrigatória. Sistemas que não cumprem esses requisitos não têm o prontuário digital reconhecido como substituto legal do papel.

### Como a LGPD afeta o prontuário eletrônico das clínicas?

A Lei nº 13.709/2018 classifica dados de saúde como sensíveis, com proteção reforçada. Para prontuários eletrônicos, isso exige: consentimento documentado do paciente para tratamento dos dados, política de retenção com prazos definidos, notificação à ANPD em até 72 horas em caso de incidente, e possibilidade de exportar ou excluir os dados do paciente mediante solicitação. O log de auditoria exigido pelo CFM também atende a parte dos requisitos de rastreabilidade da LGPD.

### Por quanto tempo a clínica deve guardar o prontuário eletrônico?

Segundo a Resolução CFM nº 1.821/2007, o prazo mínimo é de 20 anos a partir do último registro para adultos. Para menores de idade, 20 anos contados a partir do décimo oitavo aniversário. Sistemas de prontuário eletrônico bem configurados arquivam registros automaticamente sem intervenção manual, mantendo o histórico acessível dentro do prazo legal sem ocupar a interface ativa do sistema.

## Resumo

O prontuário eletrônico tem validade legal no Brasil quando atende à Resolução CFM nº 1.821/2007 e ao Manual de Certificação SBIS, com requisitos de segurança que incluem log de auditoria, criptografia, backup automático e controle de acesso por perfil. Para eliminar completamente o papel, o sistema precisa operar em nível NGS3 com assinatura digital ICP-Brasil. A LGPD adiciona exigências sobre consentimento, portabilidade e notificação de incidentes que complementam as normas do CFM.

Para colocar isso em prática, o primeiro passo é confirmar com o fornecedor atual qual o nível de certificação SBIS do sistema — e obter essa informação por escrito. O ByDoctor integra os requisitos de segurança exigidos pelo CFM com [controle de acesso por perfil](https://bydoctor.com.br/#funcionalidades), log de auditoria automático e armazenamento criptografado em nuvem. Para verificar se o sistema da sua clínica atende aos requisitos de conformidade, conheça as [funcionalidades do ByDoctor](https://bydoctor.com.br/#funcionalidades) ou acesse nossa [área de ferramentas gratuitas para profissionais de saúde](https://bydoctor.com.br/ferramentas).

## Artigos relacionados

- [Modelo de Prontuário Eletrônico: O Que Não Pode Faltar](https://bydoctor.com.br/blog/modelo-prontuario-eletronico-o-que-nao-pode-faltar)
- [Receita e Atestado por Telemedicina: Como Emitir com Validade](https://bydoctor.com.br/blog/receita-atestado-telemedicina-como-emitir-com-validade)
- [Prontuário Eletrônico CFM: Assinatura Digital Válida](https://bydoctor.com.br/blog/prontuario-eletronico-cfm-assinatura-digital-validade-juridica)