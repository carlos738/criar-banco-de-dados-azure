# criar-banco-de-dados-azure

# 1-INTRODUÇÃO
O Azure oferece uma inifindade de banco de dados como MySQL, PostgreSQL, SQL Database e muitos  outros.Este guia você terá uma noção de o que é e como criar uma intância de banco de dados no Microsoft Azure.

# 1º Passo acesse o Portal Azure
- Visite [https://portal.azure.com](https://portal.azure.com).
   - Insira suas credenciais (email e senha) para acessar o portal.
# Criar um banco de dados individual
    Para criar um banco de dados individual no portal do Azure, acesse a página de Sql do Azure :
    1 - Navegue até a página Selecionar uma opção de Implantção do Sql .
    2 - Em Bancos de dados SQL, deixe Tipo de recurso definido como Banco de dados individual e selecione Criar.
    3 - Na guia básica do formulário Criar Banco de Dados SQL, em Detalhes do projeto ,selecione Assinatura do Azure desejada.
    4 - Para Grupo de Recursos, selecione Criar,insira myResourceGroup e selecione OK.
    5 - Para Nome do banco de dados, inisira um nome para o banco de dados.
    6 - Para Servidor, selecione a opção criar e então preencha o formulário Novo servidor com os seguintes valores:
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

  
   7 - Deixe Deseja usar o pool elástico do SQL definido como Não.
   8 - No Ambiente de carga de trabalho,específique Desenvolvimento para o trabalho:
   No portal do Azure você encontrará opção de Ambiente de carga de trabalho que pode ajudar a predefinir algumas definições de configuração. 
   Você terá algumas escolhas :
 A opção de Redundância do armazenamento de backup é o armazenamento com redundância local. 
 Computação + armazenamento é de Uso geral, Sem servidor com um único vCore.
 Escolha o conjunto de ambientes de carga de trabalho de Produção:

    A Redundância de armazenamento de backup é o armazenamento com redundância geográfica, a opção padrão.
   Computação + armazenamento é Uso geral, Provisionado com 2 vCores e 32 GB de armazenamento. Isso pode ser modificado na próxima etapa.
    9 - Computação + armazenamento, selecione Configurar banco de dados.
    10 - Camada de serviço definida como Uso Geral (computação sem servidor mais econômica) e defina Camada de computação como Sem servidor. Escolha Aplicar.

   11 - Redundância de armazenamento de backup ,
   escolha uma opção de redundância para a conta de armazenamento em que os seus backups serão salvos.
   12 - Selecione Avança: Rede na parte inferior da página: CREATE SQL DATABASE.
   13 - Na guia Rede, para Método de Conectividade selecione Ponto de extremidade público
   14 - Regras de firewall, defina Adicionar o endereço IP,do cliente atual como Sim.Deixe Permitir que serviços e recursos do Azure acesse este servidor definido como Não.
   15 - Política de conexão, escolha a política de conexão Padrão e matenha Versão mínima do TLS no padrão de TLS 1.2.
   16 - Selecione Próximo: Segurança na parte inferior da página.
   17 - Na página Segurança, você pode escolher dar início a uma avaliação grátis  do Microsoft Defender para SQL, além de configurar a Razão, as Identidades gerenciadas e a Transparent Data Encryption do SQL do Azure com a chave gerenciada pelo cliente, se desejar. Selecione Avançar: Configurações adicionais na parte inferior da página.
   
   18 - Na guia Configurações adcionais,na seção Fonte de dados, para usar dados existentes, selecione Exemplo isso cria um banco de dados de amostras.
   19 - Selecione Examinar + criar na parte inferior da página.
   20 - Na página Examinar + criar, após examinar, selecione Criar.
   
   Para consultar o banco de dados depois de criado você poderá usar o Editor de consultas(versão prévia)no portal do Azure para conectar-se ao banco de dados e consultar dados
   1 - No portal, pesquise e selecione bancos de dados SQL e selecione seu banco de dados na lista.

   2 - Na página para o seu banco de dados, selecione Editor de consultas (versão prévia) no menu à esquerda.

    3 - Insira suas informações de logon do administrador do servidor da autenticação do SQL ou use a autenticação do Microsoft Entra.
 
    
 
# CONCLUSÃO
    Seguindo estás etapa acima você poderá usufruir de uma instância de banco de dados Microsoft Azure.    
