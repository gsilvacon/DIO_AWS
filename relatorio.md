# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 04/03/2024
Empresa: Abstergo Industries 
Responsável: Givaldo Silva

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa [nome da empresa], realizado por [nome do responsável pelo projeto]. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1: 
- AWS CloudFormation:

- Foco: Automação e Gerenciamento de Infraestrutura como Código (IaC)
* Automação de Infraestrutura: Permite aos usuários modelar e provisionar automaticamente a infraestrutura de TI da AWS e de terceiros de maneira segura e repetitiva. Isso é feito através de templates que descrevem todos os recursos da AWS necessários, como instâncias EC2, VPCs, RDS, entre outros.
* Gerenciamento de Configuração: Facilita o gerenciamento de configurações e a replicação de ambientes, garantindo consistência e reduzindo erros manuais ao configurar e reconfigurar recursos da AWS.

- Caso de Uso:
Uma empresa precisa implantar e gerenciar consistentemente ambientes de desenvolvimento, teste e produção para uma aplicação web. Utilizando o AWS CloudFormation, a equipe de DevOps pode criar templates para definir toda a infraestrutura necessária (como instâncias EC2, grupos de segurança, balançadores de carga, bancos de dados RDS, etc.) em um formato de código. Isso permite que eles recriem rapidamente toda a infraestrutura em diferentes ambientes ou regiões com o clique de um botão, garantindo consistência, reduzindo erros manuais e economizando tempo.

Etapa 2: 
- AWS Elastic Compute Cloud (EC2):

- Foco: Capacidade Computacional Redimensionável
* Flexibilidade de Configuração: Oferece uma vasta seleção de tipos de instâncias, otimizadas para diferentes casos de uso (computacional, intensivo em memória, otimizado para armazenamento, etc.), permitindo aos usuários escolher o ambiente de computação mais adequado para suas aplicações.
* Escalabilidade: Permite que os usuários escalem a capacidade para cima ou para baixo automaticamente, de acordo com as condições definidas, ajudando a otimizar os custos e a performance conforme a demanda.

- Caso de Uso:
Uma startup de tecnologia está desenvolvendo uma aplicação que requer escalabilidade e flexibilidade devido à variação na demanda dos usuários. Usando o Amazon EC2, a startup pode iniciar instâncias adicionais durante picos de tráfego para manter a performance da aplicação e desligá-las quando a demanda diminui para otimizar os custos. Além disso, pode-se escolher diferentes tipos de instâncias que se adequem melhor às necessidades específicas da aplicação, como instâncias otimizadas para computação, memória ou armazenamento.

Etapa 3: 
- AWS Lambda:

- Foco: Computação Sem Servidor (Serverless)
* Execução de Código em Resposta a Eventos: Permite aos usuários executar código em resposta a eventos, como mudanças em dados em um bucket do Amazon S3 ou uma atualização em uma tabela do DynamoDB, sem a necessidade de provisionar ou gerenciar servidores.
* Eficiência de Custo e Escalabilidade Automática: Com o modelo de pagamento baseado apenas no tempo de execução real do código, sem servidores para gerenciar, os usuários podem construir aplicações que automaticamente escalam com eficiência de custo, independentemente do número de solicitações.

- Caso de Uso:
Uma empresa deseja construir um sistema de processamento de imagens que automaticamente redimensiona imagens quando são carregadas em um bucket do Amazon S3. Utilizando o AWS Lambda, ela pode criar uma função que é acionada cada vez que novas imagens são adicionadas ao bucket. Essa função do Lambda pode então processar as imagens, redimensioná-las de acordo com os requisitos e salvá-las em outro bucket ou diretório. Isso elimina a necessidade de gerenciar servidores para processar as imagens, tornando o sistema mais eficiente e escalável.



## Conclusão
A implementação de ferramentas na AWS, da empresa Abstergo Industries, incluindo AWS CloudFormation, Amazon EC2 e AWS Lambda, constituiu uma fase crítica na evolução e escalabilidade de nossa infraestrutura de TI e desenvolvimento de aplicações. Esta etapa envolveu um planejamento cuidadoso e a execução de estratégias que garantiram a integração eficiente dessas ferramentas ao nosso ecossistema de tecnologia. Por meio do AWS CloudFormation, conseguimos automatizar o provisionamento e a gestão da infraestrutura, reduzindo significativamente o tempo de implantação e os erros associados ao gerenciamento manual. Com o Amazon EC2, otimizamos a performance e a escalabilidade da aplicação, adaptando-se dinamicamente às mudanças na demanda. O AWS Lambda nos permitiu adotar uma abordagem serverless para tarefas específicas, melhorando a eficiência operacional e reduzindo custos. A fase de implementação focou não apenas na integração tecnológica, mas também no alinhamento com as necessidades do negócio, garantindo que a infraestrutura de TI suportasse os objetivos de longo prazo da organização.
Após a implementação bem-sucedida, a continuidade da utilização das ferramentas AWS CloudFormation, Amazon EC2 e AWS Lambda é fundamental para sustentar o crescimento e a inovação contínuos dentro de nossa organização. Isso envolve o monitoramento constante e a avaliação do desempenho da infraestrutura, além da atualização e otimização regulares dos recursos para garantir que eles permaneçam alinhados com as exigências em evolução do nosso ambiente de aplicação. A manutenção de uma abordagem proativa para a gestão de configurações com o AWS CloudFormation facilitará a agilidade e a flexibilidade operacional, enquanto a exploração de novas instâncias e recursos do Amazon EC2 continuará a otimizar a eficiência de custos e a performance. Com o AWS Lambda, a expansão para novas funcionalidades e a integração com outros serviços da AWS potencializarão ainda mais a capacidade de inovação da nossa organização, permitindo-nos responder rapidamente às necessidades emergentes do mercado. A continuidade dessas ferramentas, portanto, não é apenas sobre manter a operação atual, mas também sobre habilitar a expansão e a adaptação às futuras demandas do negócio e da tecnologia.

## Anexos

[lista de anexos, como manuais, documentos, planilhas, entre outros]

Assinatura do Responsável pelo Projeto:

[Nome do Responsável pelo Projeto]