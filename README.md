## GetUp Cloud - Worker

Esse respositório foi criado em base ao [Example Voting App](https://github.com/dockersamples/example-voting-app). A aplicação worker é baseda em `.Net Core` que cosome os votos da aplicação [Vote](https://github.com/hebersonaguiar/vote) e armazena no banco de dados.

Essa aplicação foi criada em container e para o desafio [GetUp Cloud Docs](https://github.com/hebersonaguiar/getupclouddocs) não foi realizada nenhum tipo de alteração em relação ao seu desenvolvimento, para o projeto foi realizado o clone desse repositório, buildado e enviado ao [Hub Docker](https://hub.docker.com), para isso foram reealizados os seguintes passos:

* Clone do repositório:

```bash
git clone https://github.com/hebersonaguiar/worker.git
```

* Build da imagem:

```bash
docker build -t hebersonaguiar/worker worker/
```

* Login no [Hub Docker](https://hub.docker.com):

```bash
docker login
```
Obs: foi utilizado uma conta pessoal.

* Push da imagem para o [Hub Docker](https://hub.docker.com):

```bash
docker push hebersonaguiar/worker
```