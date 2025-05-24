# Prova PRW1 2025-1

> Backend utilizado para prova prática de PRW1 no ano/semestre de 2025-1, versando sobre Fetch API e Manipulação DOM.

### Avisos

Este código é puramente didático e deve ser utilizado apenas como modelo inicial de desenvolvimento.

## 💻 Pré-requisitos

Antes de começar, verifique que sua máquina possua:

- Docker

## 🚀 Instalando

Este projeto utiliza o Docker Compose para automatizar o processo de deploy do ambiente de desenvolvimento. Para executá-lo, no terminal, digite o seguinte comando:

```
docker compose up --build
```

## ☕ Usando

A API pode ser acessada com base no endereço `http://localhost:8080/`.

As rotas disponíveis e seus propósitos são:

- GET `/perfil` - Retorna a lista de perfis cadastrados no sistema.
- GET `/perfil/id/foto` - Retorna a imagem associada ao perfil de determinado **id**.
- GET `/foto/xxxxx` - Retorna a imagem cujo nome complete é **xxxxx**. Este é o valor retornado para a *foto* na rota `/perfil`.
- POST `/perfil` - Insere um novo perfil no sistema. Deve ser enviado no corpo da requisição os parâmetros **login** e **foto**, ambos no formato *multipart/form-data*.
- DELETE `/perfil/id` - Remove o perfil do sistema, removendo também a foto associada ao perfil.

