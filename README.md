# Descrição

Ambiente "dockerizado" para desenvolvimento do tema para OJS da revista científica Barbaqua do IFMS.

# Requisitos
* Docker
* Docker-compose

# Instalação
Em seu terminal:
~~~
docker-compose up
~~~

Acesse: http://localhost:8080

Siga as instuções de instalação para o usuário. 

## Banco de dados

Informe estes dados para a configuração de banco de dados:

Driver: `MySQLi`

Servidor: `db`

Usuário da base de dados: `ojs`

Senha para acesso à base de dados: `ojs`

Nome da base de dados: `ojs`

Desmarque `"Criar nova base de dados"`

Desmarque `"Fornece um ID único ao site e a URL OAI exclusivamente para estatísticas do PKP e alertas de segurança."`

# Desenvolvimento do Tema
Os arquivos do tema devem ficar dentro da pasta `src`, que será montada na instalação do OJS.
Na configuração da revista, habilite o pluguin do tema.

