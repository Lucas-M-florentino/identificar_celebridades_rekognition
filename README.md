# Reconhecimento de Celebridades

Este projeto demonstra como utilizar o serviço [AWS Rekognition](https://docs.aws.amazon.com/pt_br/rekognition/latest/APIReference/API_RecognizeCelebrities.html) para identificar rostos de celebridades em imagens.

## Funcionalidades

- Identificação de rostos de celebridades em imagens.
- Retorno de informações detalhadas sobre as celebridades reconhecidas, incluindo nome, ID e links associados.

## Pré-requisitos

Antes de começar, certifique-se de ter os seguintes itens:

- **Python** (versão 3.7 ou superior).
- **uv** (gerenciador de dependências).
- Uma conta AWS com acesso ao serviço Rekognition.
- Credenciais configuradas para acesso aos serviços AWS.

## Configuração do Ambiente

1. **Criar um usuário IAM**  
   No console AWS, crie um usuário IAM com permissões para o serviço Rekognition. O mínimo necessário é a política gerenciada `AmazonRekognitionReadOnlyAccess`.

2. **Configurar credenciais AWS**  
   Configure o acesso local utilizando o AWS CLI:
   ```sh
    aws configure
    ```
    Insira as chaves de acesso, região e formato de saída conforme necessário.
## Instalação

1. **Clone o repositório**
    ```sh
    git clone git@github.com:Lucas-M-florentino/identificar_celebridades_rekognition.git
    cd identificando_celebridades
    ```
2. **Instale as dependências do projeto utilizando uv**
    ```sh
    uv install
    ```
## Execução

1. **Para executar o projeto, utilize o comando abaixo**
    ```sh
        uv run main.py
    ```
    O resultado será exibido no terminal com detalhes das celebridades reconhecidas.

## Tecnologias Utilizadas
- **Python:** Linguagem de programação principal.
- **AWS Rekognition:** Serviço de reconhecimento facial.
- **uv:** Gerenciador de dependências.