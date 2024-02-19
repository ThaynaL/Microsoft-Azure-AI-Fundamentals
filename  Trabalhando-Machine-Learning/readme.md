# Trabalhando com Machine Learning na Prática
Este arquivo é feito para mostrar o passo a passo para criar modelo de previsão com as devidas configurações segundo a [documentação da Microsoft](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html) e o video na [DIO](https://www.dio.me/).

## Criando modelo
Para utilizar o machine learn é preciso ter um workspace no [Microsoft Azure](https://azure.microsoft.com/pt-br/) entre na sua conta e vá no campo de pesquisa e procure por Azure Machine Learning e crie um workspace o configure (adicionando os nomes, pois nesse caso não vai ser nescesssário mais mudanças além da localização para US) e quando estiver pronto temos que entrar no ML studio encontre a aba "ML automatizado" e crie um "novo trabalho de ML automatizado".
# Criando um ambiente de aprendizado de maquina para a previsão de aluguel de bicicletas:

<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img1.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img2.png"/> 
Adicione o tipo de tarefa: Regressão e crie o ativo.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img3.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img4.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img5.png"/> 
A URL da base de dados: https://aka.ms/bike-rentals .
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img6.png"/> 
Altere o cabeçalho de coluna para Somente o primeiro arquico tem cabeçalho.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img7.png"/> 
Continue com a configuração sugerida.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img8.png"/>  
E ativo criado.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img9.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img10.png"/> 
Selecione a coluna de destino e em seguida clique a Configuração Adicional.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img11.png"/> 
Desmarque as opções e selecione os modelos permitidos a seguir e salve.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img12.png"/> 
Defina os limites como:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img13.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img14.png"/> 
Continue com as configurações padrões em computação.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img15.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img16.png"/> 
E o envie trabalho e espere que a execução seja concluída.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img17.png"/> 
O próximo passo é ir para aba modelo e clicar nele. 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img18.png"/> 
Deve estar criado em seguida vá para ponto de extremidade.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img19.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img20.png"/> 
Acesse a aba "Testar".
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img21.png"/> 
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
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img22.png"/> 
Eu enfrentei um problema pois meu modelo não foi criado automaticamente, mas encontrei a [solução no forum da Dio](https://web.dio.me/topics/problemas-com-o-desafio-de-projeto-trabalhando-com-machine-learning-na-pratica-do-azure-ml?back=%2Ftrack%2Fmicrosoft-azure-ai-fundamentals&order=undefined&page=1&search=%20Trabalhando%20com%20Machine%20Learning&tab=forum&track_id=a088cda7-a37f-451a-b392-46fa7e6ddc55) e vou refazer a solução abaixo.
Para criar modelo:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img23.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img24.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img25.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img26.png"/>  
Para criar o ponto de extremidade em teoria na minha opnião teria que ir para modelo, depois ponto de extremidade em seguida Implementar extremidade e criar o modelo apartir disso, mas para mim o butão não funcionou então vou fazer de outra forma.
Criei o ponto de extremidade assim:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img27.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img28.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img29.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img30.png"/>  
Espere concluir e pode testar como mostrado acima.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/%20Trabalhando-Machine-Learning/img/img31.png"/> 

