# criar-banco-de-dados-azure
https://learn.microsoft.com/pt-br/azure/azure-sql/database/design-first-database-azure-data-studio?view=azuresql

## https://learn.microsoft.com/pt-br/azure/azure-sql/database/single-database-create-quickstart?view=azuresql&tabs=azure-portal

# 1-INTRODUÇÃO
O Azure oferece uma inifindade de banco de dados como MySQL, PostgreSQL, SQL Database e muitos  outros.Este guis você terá uma noção de o que é e como criar uma intância de banco de dados no Microsoft Azure.

# 1º Passo acesse o Portal Azure
- Visite [https://portal.azure.com](https://portal.azure.com).
   - Insira suas credenciais (email e senha) para acessar o portal.
# Criar um banco de dados individual
    Para criar um banco de dados individual no portal do Azure, acesse a página de Sql do Azure :
    1- Navegue até a página Selecionar uma opção de Implantção do Sql .
    2- Em Bancos de dados SQL, deixe Tipo de recurso definido como Banco de dados individual e selecione Criar.
    3- Na guia básica do formulário Criar Banco de Dados SQL, em Detalhes do projeto ,selecione Assinatura do Azure desejada.
    4- Para Grupo de Recursos, selecione Criar,insira myResourceGroup e selecione OK.
    5- Para Nome do banco de dados, insira mySampleDatabase.
    6- Para Servidor, selecione a opção criar e então preencha o formulário Novo servidor com os seguintes valores:
# NOME DO SERVIDOR
Insira o mysqlserver e adicione os caracteres para que o nome seja exclusivo.
# LOCALIZAÇÃO
Selecione a localização suspensa na lista suspensa.
# MÉTODOS DE AUTENTICAÇÃO
Selecione uma localização na lista.
# LOGON DO ADMINISTRADOR DO SERVIDOR
Insisra o azureuser
# SENHA
Insira uma senha segura e depois insira novamente no campo Confirmar Senha
Depois:
Selecione OK.

  
   7- Deixe Deseja usar o pool elástico do SQL definido como Não.
   8- No Ambiente de carga de trabalho,específique Desenvolvimento para o trabalho:
   No portal do Azure você encontrará opção de Ambiente de carga de trabalho que pode ajudar a predefinir algumas definições de configuração. 
   Você terá algumas escolhas :
# A opção de Redundância do armazenamento de backup é o armazenamento com redundância local. 
# Computação + armazenamento é de Uso geral, Sem servidor com um único vCore.
# Escolha o conjunto de ambientes de carga de trabalho de Produção:

#    A Redundância de armazenamento de backup é o armazenamento com redundância geográfica, a opção padrão.
#    Computação + armazenamento é Uso geral, Provisionado com 2 vCores e 32 GB de armazenamento. Isso pode ser modificado na próxima etapa.
    9 - Computação + armazenamento, selecione Configurar banco de dados.
    10 - Camada de serviço definida como Uso Geral (computação sem servidor mais econômica) e defina Camada de computação como Sem servidor. Escolha Aplicar.

   
