# WP-AWS-cloudformation
# Projeto de Infraestrutura na AWS com AWS CloudFormation

Este projeto tem como objetivo criar uma infraestrutura na AWS usando o AWS CloudFormation para hospedar um aplicativo WordPress altamente disponível e escalável. A infraestrutura inclui:

- Uma Virtual Private Cloud (VPC) com duas sub-redes públicas.
- Um cluster ECS para a execução de contêineres Docker.
- Um Application Load Balancer (ALB) para distribuição de tráfego.
- Um sistema de arquivos Amazon Elastic File System (EFS) para armazenamento de dados persistente.
- Um banco de dados Amazon RDS para WordPress.

## Pré-requisitos

Antes de implantar este projeto, certifique-se de que você tenha:

- Uma conta da AWS configurada com permissões adequadas.
- A CLI da AWS instalada e configurada com suas credenciais.


## Implantação

Você pode implantar esta infraestrutura usando o AWS Management Console ou a linha de comando AWS CLI. Certifique-se de editar os parâmetros no arquivo `stack.yml` conforme necessário.

1. Faça o upload do arquivo `stack.yml` para o AWS CloudFormation.
2. Crie uma nova pilha e siga as etapas de configuração, fornecendo os parâmetros necessários.
3. Aguarde até que a pilha seja criada com sucesso.

## Personalização

Você pode personalizar este projeto para atender às suas necessidades específicas:

- Altere os parâmetros no arquivo `stack.yml` para ajustar o tamanho da infraestrutura, as regiões da AWS, as imagens de AMI, etc.
- Personalize a configuração do contêiner no `ECSTaskDefinition` para adicionar suas variáveis de ambiente e requisitos específicos do aplicativo.
- Configure o banco de dados RDS no `WordpressDB` para atender aos requisitos de armazenamento e desempenho.


