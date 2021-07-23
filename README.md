# DBeaver
Configurações e úteis para DBeaver

- Instalação:

https://dbeaver.io/

## Dicas

### Backup e Restore com DBEAVER:

- Instalar o postgres:

```
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
sudo apt-get update
sudo apt-get -y install postgresql
```

- Conectar DBEAVER no banco de dados

  * Criar uma conxeão com o banco de dados;
  * Editar a conexao criada. Clicar em Local Client: Browse...;
  * Clicar em Add Home e selecionar a pasta de instalação do postgres ex: /usr/lib/postgresql/13/bin;
  * Clicar em OK (Confirmar caso seja solicitado reiniciar a conexão com o banco);
  * Clicar com o botão direito sobre um schema e selecionar backup/restore e seguir a execução. Se desejar pode salvar a task para ser reutilizada mais vezes ou agendada.
