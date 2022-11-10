# Laboratório Linux usando Vagrant

Este é um laboratório que montei durante meus estudos de linux para realizar o provisionamento automático ;)

# Tutorial

Primeiro, o Vagrant se conecta à um provider (podendo esse ser o VirtualBox, Hyper-V, Docker e até mesmo o VMware) através do arquivo Vagranfile. Então, já comece instalando algum deles! ;)

Para começar a fazer uso do Vagrant é necessário primeiramente realizar a instalação dele, que pode ser feito em qualquer ambiente

**Distribuições baseadas no Debian:**

sudo apt install -y vagrant

**Distribuições baseadas na RedHat:**

sudo yum install -y vagrant

--------------------------------------------------------------------

S.O da janelinha: https://developer.hashicorp.com/vagrant/downloads

Faça o download do binário e next, next, next :)

--------------------------------------------------------------------

S.O da maça: brew install vagrant

--------------------------------------------------------------------

Após a instalação ter finalizado, iniciaremos com o provisionamento das máquinas com o comando:

vagrant up

Agora que já temos uma máquina rodando podemos acessá-la via ssh. Você consegue acessar utilizando:

vagrant ssh <nome_da_vm>

--------------------------------------------------------------------
**Façam bom proveito! ;)**
