# AWS Data Pipeline: Ingestão e Gerenciamento de Dados

Este repositório contém uma demonstração de uma pipeline de ingestão de dados na AWS, utilizando Python para gerenciar a ingestão e remoção de dados dentro do ambiente AWS.

## Estrutura do Projeto

Neste projeto, realizamos as seguintes atividades:

- **Configuração do IAM**: Configuramos o IAM para gerenciar permissões e acesso aos recursos da AWS.
- **Criação de Buckets S3**: Criamos buckets S3 com camadas Bronze e Silver para armazenar os dados de forma estruturada.
- **Configuração do Lake Formation**: Estabelecemos o Lake Formation, definindo seus administradores e Data Locations.
- **Monitoramento de Custos**: Implementamos monitoramento de custos usando AWS Budget e CloudWatch.
- **Ingestão e Remoção de Dados com Python**: Utilizamos scripts Python para ingerir dados externos no S3 e remover dados quando necessário.

## Utilização do Projeto

1. **Ingestão de Dados**: O script Python `Pipeline_AWS.ipynb` permite ingerir dados externos para o bucket S3 configurado.
2. **Remoção de Dados**: O script Python `Pipeline_AWS.ipynb` facilita a exclusão de dados específicos no bucket S3.

## Pré-requisitos

- Conta na AWS com permissões adequadas para IAM, S3, Lake Formation, AWS Budget e CloudWatch.
- Criação das camadas Bronze e Silver.
- Criação de um arquivo .env ou específicar no programa suas credenciais de acesso como chave ID, chave secreta e região do bucket.

## Como Executar

1. Clone este repositório.
2. Configure suas credenciais da AWS no seu ambiente.
3. Execute os scripts Python conforme necessário:

```bash
python Pipeline_AWS.ipynb
