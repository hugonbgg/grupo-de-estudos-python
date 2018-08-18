# Instalando Anaconda no Ubuntu 18.04

Neste tutorial vamos:

* Baixar o instalador Anaconda para  linux;  
* Checar se download foi bem feito;  
* Instalar o Anaconda3;

## Baixando o instalador
Usando o terminal, vamos para a pasta `tmp` e usaremos o `curl` fazer o download do instalador lá. Assim, após a instalação o instalador será removido automaticamente ao reiniciar o computador:
```
cd /tmp
curl -O https://repo.anaconda.com/archive/Anaconda3-5.2.0-Linux-x86_64.sh
```
Perceba que a versão no momento da criação deste tutorial é *Anaconda3-5.2.0*.  
:warning: **Antes de iniciar a instalação, confirme [nesse link](https://www.anaconda.com/download/#linux) qual é a ultima versão** :warning:

## Confirmando se download foi realizado com sucesso
O *sha256sum* é usado para confirmar se o pacote baixado possui as mesmas características do pacote disponibilizado. Basta esecutar no terminal e aidna na mesma pagina onde foi feito o download do Anaconda:
```
sha256sum Anaconda3-5.1.0-Linux-x86_64.sh
```
O output deverá ser: *09f53738b0cd3bb96f5b1bac488e5528df9906be2480fe61df40e0e0d19e3d48 Anaconda3-5.2.0-Linux-x86_64.sh*  
:warning: Caso você esteja instalando outra versão, o sha256 será diferente. Portanto, confirme com o que é disponibilizado [nesta pagina](https://docs.anaconda.com/anaconda/install/hashes/lin-3-64).:warning:  

**Com com sha256 confirmado, temos certeza que o download foi realizado com sucesso e o instalador não está corrompido**

## Instalando Anaconda
Com o terminal ainda na pasta onde o instalador foi descarregado, basta executar:
```
bash Anaconda3-5.2.0-Linux-x86_64.sh
```
A partir daí é seguir o texto de instalação...
Fique atento que algumas perguntas serão feitas.
** Segundo consta no guia de instalação do windows, não é necessário instalar o *Visual Studio***.
Após a instalação é preciso ativar, com o seguinte comando:
```
source ~/.bashrc
```
Tutorial baseando nesta publicação da [Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-install-the-anaconda-python-distribution-on-ubuntu-18-04)
