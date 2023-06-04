# Instância Ubuntu - Vagrant

Este projeto tem como objetivo apresentar um exemplo simples da criação de uma instância Ubuntu 18.04.3 LTS com o Vagrant, que vai servir a API do [Via CEP](https://viacep.com.br/). Tal projeto segue as aulas do curso "Vagrant - Gerenciando máquinas virtuais", do [Iago Ferreira](https://github.com/iagoferreirati).

## Configurações do projeto

O projeto contém os seguintes arquivos / estrutura:

- `Vagrantfile` - tem o shell definido como provisionador; configurações de network com redirecionamento de porta para a porta 8090; com nome, cpu e memória ram pré-definidos;
- `script.sh` - um shell script para executar os comandos de update, instalar e ativar o servidor Nginx;
- Diretório `cep/` que contém os arquivos html e js para o Via Cep.

- _A pasta "img" não compõe o projeto._

### Exemplo

![imagem de exemplo](https://github.com/ludsilva/vagrant-shell-script/blob/master/img/Via%20cep.png)

## Como utilizar este repositório

1. Primeiro, você deve clonar este repositório com o comando: `git clone https://github.com/ludsilva/vagrant-shell-script.git`

2. Para rodar este projeto localmente, você precisa ter o Vagrant instalado em sua máquina local. 
  - [Windows](https://www.youtube.com/watch?v=yFSm6TXBuDE&ab_channel=VemcomoPY) | [Linux](https://www.youtube.com/watch?v=fwKPiyWaDbU&pp=ygUQaW5zdGFsYXIgdmFncmFudA%3D%3D) | [Documentação do Vagrant](https://developer.hashicorp.com/vagrant/downloads)

3. Após instalado, siga com os seguintes comandos no terminal / bash dentro do repositório:
```
## Criar a instância
 vagrant up
## Acessar a instância via ssh
  vagrant ssh
```

4. Para acessar a página do Via Cep, digite no seu navegador: `localhost:8080`
