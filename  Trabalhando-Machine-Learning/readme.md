# Trabalhando com Machine Learning na Prática
Este arquivo é feito para mostrar o passo a passo para criar modelo de previsão com as devidas configurações segundo a [documentação da Microsoft](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html) e o .

## Criando modelo
Para utilizar o machine learn é preciso ter um workspace no [Microsoft Azure}(https://azure.microsoft.com/pt-br/) entre na sua conta e vá no campo de pesquisa e procure por Azure Machine Learning e crie um workspace o configure (adicionando os nomes, pois nesse caso não vai ser nescesssário mais mudanças além da localização para US) e quando estiver pronto temos que entrar no ML studio encontre a aba "ML automatizado" e crie um "novo trabalho de ML automatizado".
# Criando um ambiente de aprendizado de maquina para a previsão de aluguel de bicicletas:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/img1.png" width=""/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img2.png" width=""/> 
Adicione o tipo de tarefa: Regressão e crie o ativo.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img3.png" width=""/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img4.png" width=""/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img5.png" width=""/> 
Base de dados URL: https://aka.ms/bike-rentals
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/.png" width=""/> 
Selecione a coluna de destino e em seguida clique a Configuração Adicional
<img align="center" src="" width=""/> 
Após o envio deve esperar a execução ser concluida
<img align="center" src="" width=""/> 
O próximo passo é ir para aba modelo e o modelo deve estar criado em seguida vá para ponto de extremidade.
<img align="center" src="" width=""/> 
Logo após a implantação, que demora bastante, acessei a aba "Testar" do ponto de extremidade criado para o meu modelo.
<img align="center" src="" width=""/> 
Para o teste, utilizei o JSON abaixo:
ˋˋˋ
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}
ˋˋˋ
<img align="center" src="" width=""/> 
Eu enfrentei um problema pois meu modelo não foi criado automaticamente, mas encontrei a [solução no forum da Dio](https://web.dio.me/topics/problemas-com-o-desafio-de-projeto-trabalhando-com-machine-learning-na-pratica-do-azure-ml?back=%2Ftrack%2Fmicrosoft-azure-ai-fundamentals&order=undefined&page=1&search=%20Trabalhando%20com%20Machine%20Learning&tab=forum&track_id=a088cda7-a37f-451a-b392-46fa7e6ddc55) e vou refazer abaixo.
Para criar modelo:
<img align="center" src="" width=""/> 
<img align="center" src="" width=""/> 
Para criar o ponto de extremidade em teoria na minha opnião teria que ir para modelo, depois ponto de extremidade em seguida Implementar extremidade e criar o modelo apartir disso, mas para mim o butão não funcionou então vou fazer de outra forma.
Criando o ponto de extremidade assim:
<img align="center" src="" width=""/> 
<img align="center" src="" width=""/> 
<img align="center" src="" width=""/> 
<img align="center" src="" width=""/> 