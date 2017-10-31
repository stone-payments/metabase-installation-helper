# Metabase


## O que é 

Metabase é um servidor Open source de BI (business Intelligence), que você pode instalar rapidamente na sua máquina e que pode se conectar ao MySQL , PostgreSQL, MongoDB e muito mais!

Ele é uma maneira mais rápida e fácil de analisar dados. Onde qualquer pessoa pode usá-lo para construir gráficos e dashboards.

## Este repositório

Repositório criado apenas para facilitar a instalação de uma instância do metabase em um PAAS através da documentação dos passos necessários.

## Instalação

1. Clonar este repositório em sua máquina;

2. Criar as variáveis de ambiente necessárias:

| Nome | Descrição |
| ---- | --------- |
| SECRET_KEY | Chave criptográfica de 32 dígitos que deve ser gerada para uso interno do metabase.
| DATABASE_TYPE | tipo de banco de dados do backend do metabase a ser usado. Os valores possíveis são: mysql, postgres ou h2 |
| DATABASE_NAME | Nome do banco de dados a ser usado no backend | 
| DATABASE_PORT | Porta do banco de dados a ser usado no backend | 
| DATABASE_USER | Usuário do banco de dados a ser usado no backend |
| DATABASE_PASS | Senha do usuário a ser usada no backend | 
| DATABASE_HOST | Endereço do banco de dados a ser usado no backend |

3. Fazer download do JAR do metabase e colocá-lo na raiz deste repositório. O nome do arquivo deverá ser ***exatamente*** **metabase.jar**

> https://www.metabase.com/start/jar.html

4. Fazer o deploy normalmente no PAAS deu sua preferência.

Obs.: Para execução local basta fazer os passos acima e executar o arquivo **metabase.sh**