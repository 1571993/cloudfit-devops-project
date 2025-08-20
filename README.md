# CloudFit DevOps

## Objetivo do Projeto

Este projeto tem como objetivo demonstrar práticas de DevOps utilizando uma aplicação Flask simples e infraestrutura como código com Terraform para provisionamento na AWS. O projeto inclui automação de testes e deploy via GitHub Actions.

## Instruções para Rodar Localmente

1. Instale o Python 3.11 ou superior.
2. Instale as dependências:
   ```
   pip install -r app/requirements.txt
   ```
3. Execute a aplicação Flask:
   ```
   python app/app.py
   ```
4. Acesse `http://localhost/status` para verificar o status da API.

## Explicação da Infraestrutura

- Utiliza Terraform para provisionar uma instância EC2 na AWS (tipo `t2.micro`).
- Um grupo de segurança é criado permitindo acesso à porta 80 (HTTP).
- A aplicação Flask pode ser hospedada na instância provisionada.

## Explicação do CI/CD

- O workflow do GitHub Actions é acionado a cada push na branch `main`.
- As etapas incluem:
  1. Instalação das dependências do Python.
  2. Execução dos testes (simulado).
  3. Deploy da aplicação (simulado).
