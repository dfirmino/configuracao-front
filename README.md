
# Descrição

Esse arquivo tem como intenção auxiliar a configuração do ambiente de desenvolvimento do front-end.

## Pré Requisitos

Assumo que você já instalou o **Docker** e clonou o **repositório**.

## Bora Começar?

#### montando a imagem

Certifique-se de estar na raiz do projeto antes de começar a seguir os passos

Temos 2 Dockerfiles para executar, começaremos com o seguinte comando:

``
docker image build -t mr_satan .
``

aguarde ansiosamente a finalização do build e logo em seguida execute:

``
docker image build -t majin_boo -f Dockerfile2 .
``

#### Vamos conferir?

digite o seguinte comando:

``
docker image list 
``

se tudo estiver certo teremos duas imagens criadas com os nomes:

mr_satam 

<img src="https://i.pinimg.com/originals/60/ac/23/60ac23c7ceee5ebd663e93a7baac70c8.jpg" alt="satam" width="200"/>

majin_boo

<img src="https://pm1.narvii.com/6622/195d6071d5d840057ee1db9f7d82424d5a6b8ca0_00.jpg" alt="majin boo" width="200"/>


#### montando o container

Está na hora de montar os containers:

``
docker run -it -p 80:80 --name majin_boo majin_boo
``


``
docker run -it -p 3000:3000 --name mr_satan mr_satan  
``

## Testando
se tudo estiver certo agora é só acessar o localhost na porta **3000** para o ambiente de **dev** e na porta **80** para o ambiente de **produção**.

## Deu algum erro?
É só rezar e tentar novamente =)
