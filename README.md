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
Ou `docker-compose up -d` para liberar o terminal.

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

## Configuração permanente

Ao clicar em `Instalar o sistema`, uma tela aparecerá informando que o arquivo `config.inc.php` não pode ser alterado. Isto é esperado.

Copie o código de configuração exibido abaixo da mensagem, crie um novo arquivo em `volumes/config/ojs.config.inc.php` e cole a configuração. ATENÇÃO! O nome do novo arquivo deve ser `ojs.config.inc.php`.

Não realizar esta etapa fará com que seja necessário reinstalar o sistema sempre que o comando `docker-compose up` for executado.

# Desenvolvimento do Tema
Os arquivos do tema devem ficar dentro da pasta `src`, que será montada na instalação do OJS.
Na configuração da revista, habilite o pluguin do tema.

### Atenção
**Este ambiente não deve ser usado em produção.**