# my-linux-vim-cheatsheet
Cheatsheet of useful linux commands that I always forget

## Linux

|O que faz   | Comando  |  
|---|---|
|Encontrar arquivos grandes| du -sh /* |  
|Compactar   | tar -czvf arquivo.tar.gz pasta  |   


## VIM

|O que faz| Comando|
|---|---|
|Localizar e substituir| :%s/foo/bar/g|

## Postgres

|O que faz| Comando|
|---|---|
|Encontrar maiores bancos de dados | SELECT pg_database.datname, pg_size_pretty(pg_database_size(pg_database.datname)) AS size FROM pg_database ORDER BY pg_database_size(pg_database.datname) DESC; |

SELECT 'rollback prepared ' || gid || ';' FROM pg_prepared_xacts WHERE CURRENT_TIMESTAMP - prepared > '1 min';

