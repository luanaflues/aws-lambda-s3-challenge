# Desafio AWS CloudFormation - Automação com S3 e Lambda

## Introdução
Este repositório documenta minha implementação do desafio da DIO para criar uma infraestrutura automatizada com AWS CloudFormation, integrando S3, Lambda Function, e S3 Object Lambda. O projeto utiliza um template YAML para provisionar recursos de forma escalável, aplicando conceitos de infraestrutura como código (IaC).

## Pré-requisitos
- Conta AWS ativa (Free Tier recomendado)
- AWS CLI configurada (opcional)
- Git e GitHub configurados
- Editor de texto (ex.: VS Code)

## Passos Realizados
1. **Criação do Template**:
   - Criei um template YAML (`templates/lambda-s3-template.yaml`) para provisionar:
     - Um bucket S3 (`luanaflues-bucket-us-east-2-2025`).
     - Uma função Lambda (`LuanaLambdaFunction`) para processar objetos do bucket.
     - Um S3 Object Lambda Access Point (`luana-object-lambda`) para transformar dados.
   - Configurei permissões IAM para permitir que a Lambda acesse o bucket S3.
2. **Validação e Implantação**:
   - Validei o template usando a AWS Console ou CLI.
   - Implantei o stack `LuanaLambdaStack` na região `us-east-2`.
3. **Verificação**:
   - Confirmei a criação do bucket S3, função Lambda, e S3 Object Lambda Access Point.
   - (Capturas de tela a serem adicionadas na pasta `/images`).
4. **Documentação**:
   - Estruturei este README com detalhes do processo.
   - Planejado adicionar capturas de tela para ilustrar os resultados.

## Resultados
- **Bucket S3**: Criado com sucesso (`luanaflues-bucket-us-east-2-2025`).
- **Função Lambda**: Configurada e ativa.
- **S3 Object Lambda**: Configurado para transformar dados do bucket.
- Capturas de tela (a serem adicionadas):
  - [Stack no CloudFormation](images/captura1.png)
  - [Bucket S3](images/captura2.png)
  - [Função Lambda](images/captura3.png)
  - [S3 Object Lambda Access Point](images/captura4.png)

## Insights e Lições Aprendidas
- Aprendi a estruturar templates CloudFormation para integrar S3, Lambda, e S3 Object Lambda.
- Entendi a importância de configurar permissões IAM corretamente para a Lambda.
- Notei que nomes de buckets S3 devem ser globalmente únicos.
- Aprendi a gerenciar repositórios GitHub e resolver conflitos.

## Referências
- [Documentação AWS CloudFormation](https://docs.aws.amazon.com/cloudformation/)
- [Documentação AWS Lambda](https://docs.aws.amazon.com/lambda/)
- [Documentação S3 Object Lambda](https://docs.aws.amazon.com/AmazonS3/latest/userguide/transforming-objects.html)
- [Guia de Markdown do GitHub](https://docs.github.com/en/get-started/writing-on-github)
- [AWS Samples - CloudFormation](https://github.com/awslabs/aws-cloudformation-templates)# aws-lambda-s3-challenge
Aplique os conceitos de automação de infraestrutura na AWS utilizando o CloudFormation.
