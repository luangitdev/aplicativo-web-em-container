
# **Aplicação WEB Python/Flask com Docker**

![GitHub](https://img.shields.io/badge/Python-3.9-blue) ![Docker](https://img.shields.io/badge/Docker-Supported-blue)

Este é um projeto simples de uma aplicação web desenvolvida em Python usando o framework Flask e containerizada com Docker. O objetivo deste projeto é demonstrar os conceitos básicos de como criar, configurar e executar uma aplicação Flask dentro de um container Docker.

---

## **Índice**

1. [Descrição do Projeto](#descrição-do-projeto)
2. [Tecnologias Utilizadas](#tecnologias-utilizadas)
3. [Pré-requisitos](#pré-requisitos)
4. [Configuração Local](#configuração-local)
5. [Executando a Aplicação com Docker](#executando-a-aplicação-com-docker)
6. [Contribuição](#contribuição)
7. [Licença](#licença)

---

## **Descrição do Projeto**

Este projeto consiste em uma aplicação Flask simples que exibe a mensagem `"Hello, Docker!"` quando acessada via navegador. Ele foi desenvolvido para ajudar iniciantes a aprenderem como containerizar uma aplicação Flask usando Docker.

---

## **Tecnologias Utilizadas**

- **Python 3.9**: Linguagem de programação utilizada para desenvolver a aplicação.
- **Flask**: Framework web minimalista para Python.
- **Docker**: Plataforma usada para criar, implantar e executar a aplicação em containers.
- **Dockerfile**: Arquivo usado para definir o ambiente da aplicação dentro do container.

---

## **Pré-requisitos**

Antes de executar este projeto, certifique-se de ter as seguintes ferramentas instaladas:

- **Python 3.9+** (opcional, apenas se você quiser rodar a aplicação localmente sem Docker).
- **Docker**: Para construir e executar a imagem do container.
- **Git**: Para clonar o repositório.

Você pode verificar se o Docker está instalado corretamente executando:
```bash
docker --version
```

---

## **Configuração Local**

### Clonando o Repositório

Para começar, clone este repositório para sua máquina local:

```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
```

---

## **Executando a Aplicação com Docker**

### Passo 1: Construir a Imagem Docker

No diretório raiz do projeto, execute o seguinte comando para construir a imagem Docker:

```bash
docker build -t flask-app .
```

### Passo 2: Executar o Container

Depois de construir a imagem, execute o container com o seguinte comando:

```bash
docker run -dit -p 5000:5000 flask-app
```

Isso mapeará a porta `5000` do container para a porta `5000` do host.

### Passo 3: Acessar a Aplicação

Abra o navegador e acesse:

```
http://localhost:5000
```

Você deverá ver a mensagem:

```
Hello, Docker!
```

---

## **Estrutura do Projeto**

Aqui está a estrutura básica do projeto:

```
projeto-flask/
│
├── app.py          # Código da aplicação Flask
├── requirements.txt # Dependências Python
├── Dockerfile      # Instruções para criar a imagem Docker
└── README.md       # Documentação do projeto
```

---

## **Contribuição**

Contribuições são bem-vindas! Se você deseja contribuir para este projeto, siga estas etapas:

1. Faça um fork deste repositório.
2. Crie uma nova branch para suas alterações:
   ```bash
   git checkout -b feature/nova-funcionalidade
   ```
3. Faça suas alterações e commit:
   ```bash
   git commit -m "Adiciona nova funcionalidade"
   ```
4. Envie suas alterações para o GitHub:
   ```bash
   git push origin feature/nova-funcionalidade
   ```
5. Abra um Pull Request neste repositório.

---

## **Licença**

Este projeto está licenciado sob a **MIT License**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## **Contato**

Se tiver dúvidas ou sugestões, sinta-se à vontade para entrar em contato:

- **Nome**: Luan Castro
- **Email**: luandecastrosilva@gmail.com
- **LinkedIn**: [linkedin.com/in/luancastrosilva](https://www.linkedin.com/in/luancastrosilva/)
- **GitHub**: [github.com/luangitdev](https://github.com/luangitdev)
