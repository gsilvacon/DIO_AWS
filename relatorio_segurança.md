# RELATÓRIO DE IMPLEMENTAÇÃO DE MEDIDAS DE SEGURANÇA

Data: 04/03/2024
Empresa: Abstergo Industries
Responsável: Givaldo Silva

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa [nome da empresa], realizado por [nome do responsável pelo projeto]. O objetivo do projeto foi elencar 3 medidas de segurança em conjunto dos serviços da AWS, com a finalidade de realizar aumentar a segurança na empresa.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 medidas de segurança. A seguir, serão descritas as etapas da implementação:

Medida 1: Controle de Acesso e Gerenciamento de Identidade
- Situação: Uma empresa de tecnologia financeira (fintech) que opera com dados sensíveis de clientes e precisa garantir que apenas funcionários autorizados tenham acesso a informações específicas, baseadas em seus papéis e responsabilidades.

- Implementação: A empresa utiliza o AWS Identity and Access Management (IAM) para criar políticas de permissão detalhadas que definem o acesso aos recursos da AWS. Por exemplo, os desenvolvedores podem ter acesso para implantar e gerenciar instâncias EC2, mas apenas o pessoal de segurança da informação tem permissão para configurar regras de grupos de segurança e NACLs. Além disso, a empresa ativa a Autenticação Multifator (MFA) para todos os usuários, adicionando uma camada extra de segurança ao acessar a console da AWS, ajudando a proteger contra o comprometimento de credenciais.

Medida 2: Segurança de Rede
- Situação: Um provedor de serviços de streaming de vídeo deseja garantir que seu conteúdo seja acessível apenas em regiões geográficas específicas, devido a restrições de licenciamento de conteúdo, e quer isolar seu ambiente de produção do ambiente de desenvolvimento e teste.

- Implementação: Utilizando o Amazon Virtual Private Cloud (VPC), a empresa cria VPCs separadas para seus ambientes de produção e desenvolvimento. Dentro da VPC de produção, grupos de segurança são configurados para permitir tráfego de entrada somente de locais geográficos permitidos, usando NACLs para reforçar essa política em nível de sub-rede. Além disso, eles implementam listas de controle de acesso em nível de rede (NACLs) para bloquear explicitamente o tráfego não autorizado, mesmo que ele venha de outras partes da própria organização.

Medida 3: Criptografia de Dados
- Situação: Um hospital precisa armazenar registros médicos eletrônicos de pacientes na AWS, exigindo que esses dados sejam mantidos de forma segura e confidencial, conforme regulamentações de privacidade de dados, como o HIPAA.

- Implementação: O hospital utiliza o AWS Key Management Service (KMS) para criar e gerenciar chaves de criptografia usadas para criptografar os registros médicos eletrônicos armazenados em buckets do Amazon S3 e volumes do Amazon EBS. A criptografia de dados em repouso garante que, mesmo se o acesso físico aos dispositivos de armazenamento for obtido, os dados permanecerão inacessíveis sem as chaves de criptografia apropriadas. Para a criptografia em trânsito, o hospital garante que toda a comunicação entre seus servidores e os clientes (navegadores dos pacientes) seja realizada sobre HTTPS, utilizando TLS para proteger os dados sensíveis enquanto estão sendo transmitidos pela Internet.


## Conclusão
A implementação das medidas de segurança descritas — controle de acesso e gerenciamento de identidade, segurança de rede e criptografia de dados, na empresa Abstergo Industries — é fundamental para estabelecer uma base sólida de segurança na infraestrutura da AWS. Essas medidas não apenas protegem os recursos críticos da empresa contra acessos não autorizados e potenciais ameaças cibernéticas, mas também garantem a conformidade com padrões e regulamentações de segurança relevantes. Ao definir políticas de permissão detalhadas com o IAM, segmentar a rede com VPCs e grupos de segurança, e proteger os dados em repouso e em trânsito com criptografia, as organizações podem criar um ambiente de nuvem que suporta suas operações de maneira segura e eficiente. Essa abordagem não apenas reduz o risco de incidentes de segurança, mas também fortalece a confiança dos stakeholders no compromisso da organização com a proteção de informações sensíveis.

A continuidade da utilização dessas medidas de segurança é igualmente crítica para a proteção duradoura dos ativos de TI da organização na AWS. Isso requer uma vigilância constante, revisão e atualização das políticas de segurança para se adaptarem às novas ameaças emergentes, bem como às mudanças na infraestrutura e nos requisitos do negócio. A gestão contínua do acesso e identidades, a monitorização da segurança da rede e a gestão das chaves de criptografia devem ser consideradas atividades contínuas, integradas ao ciclo de vida operacional da organização. Além disso, a adoção de práticas recomendadas de segurança, como a realização regular de auditorias de segurança e testes de penetração, pode ajudar a identificar e mitigar vulnerabilidades proativamente. Manter um compromisso contínuo com a segurança na nuvem não apenas protege os recursos e dados da empresa, mas também sustenta a agilidade e inovação ao permitir que a organização se adapte e cresça de forma segura no ambiente dinâmico da AWS

## Anexos

[lista de anexos, como manuais, documentos, planilhas, entre outros]

Assinatura do Responsável pelo Projeto:

[Nome do Responsável pelo Projeto]