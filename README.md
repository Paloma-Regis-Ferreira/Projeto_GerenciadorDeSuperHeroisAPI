# Projeto_GerenciadorDeSuperHeroisAPI
Projeto desenvolvido nas aulas da DIO para gerenciar super herois com API reativa usando Spring Boot


CONFIGURAÇÂO DO AWS CLI
  - instalar:
    https://docs.aws.amazon.com/pt_br/cli/latest/userguide/install-cliv2-windows.html
  - Configurar:
    cmd: $ aws configure
    AWS ACCESS KEY ID[none] --passo abaixo
    AWS SECRET Access Key[none] --passo abaixo
    Default region name[none]: us-west-2 
    Default output format[none]: json
  - Gerar access key e key id:
    Fazer login no site da AWS > Services > computação > EC2 > clicar sobre seu nome > Security credentials > Access Keys > create new key (GUARDE AS INFORMAÇÔES)
    preencher no cmd conforme solicitado e mostrado acima
    
CONFIGURAÇÂO E DOWNLOAD DYNAMODB
  - https://docs.aws.amazon.com/pt_br/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html
  - fazer o download pela região
  - alocar a pasta e extrair
  - entrar no cmd e entrar no diretório da pasta
  - inserir :
    java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
    * ele vai subir o servidor do Dynamo que vai ficar escutando a aplicação
