# NavyMarket-Plugin
Plugin de Entregas Automáticas com Integração ao Site!

##################################
#           config.yml           #
##################################

Nome: 'RankupMC' #Nome do seu servidor ex: RedeMain
Servidor: 'RankUP' #Servidor aonde será feito as entregas dos produtos

Site:
  Token: '####-####-####-####' #Token do servidor (Encontra-se no painel na aba Pacotes)

# Caso você queira que todos jogadores recebam algum bônus quando um jogador
# obter um produto na sua loja, basta configurar a opção abaixo.
# Obs: Utilize "true" para manter essa opção ativa, e "false" para desabilitar.
Bonus:
  Ativar: true
  ActionBar: '&aVocê ganhou um bonus dado pelo jogador(a): &e%player%'
  DarBonus: 'give %allPlayers% diamond 32'

Notificações:  #Caso habilitado, todos jogadores irão receber uma mensagem na tela quando tiver alguma ativação de produto
  Ativar: true
  Title:
    s1: '&a&l%player%'
    s1_subtitle: '&eEfetuou uma compra em nossa loja'

  ActionBar:  #Mensagem na actionbar do jogador que comprou
    s1: '&aSeu produto foi entregue com sucesso!'


Bot: #Bot Discord, qualquer ativação feita no servidor será enviada uma mensagem
  Discord: false
  Token: '{}' #Token do bot
  Channel-ID: '{}' #ID do canal onde você deseja receber as mensagens
  AutoReconnect: true #Reconectar o bot caso haja algum bug e o bot se desligue.
  #Não altere os campos abaixo caso não saiba o que esta fazendo!
  Titulo: '%name_server% - Entrega realizada'
  Presence: '%name_server% - Entregador'
  Config:
    FooterUrl: 'https://i.pinimg.com/originals/0e/c8/20/0ec820afd4d018a38b8425e0e2c30dc8.gif'
    Footer: '%name_server% - Exibindo status do servidor!'
  Embed:
    in1:
      name: '➟ **Ativação do produto:** '
      msg: '%player% realizou uma compra em nosso site e já recebeu seu produto. Nós da %name_server% agradecemos pela sua compra.'
    in2:
      name: '➟ **Servidor entregue:**'
      msg: 'Este produto foi entregue em **__%servidor%__**'
