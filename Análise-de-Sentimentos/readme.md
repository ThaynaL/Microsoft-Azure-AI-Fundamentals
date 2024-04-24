# Análise de Sentimentos com Language Studio no Azure AI
Passo a passo do desafio de projeto "Análise de Sentimentos com Language Studio no Azure AI" da DIO. Material para consulta: [Explore Speech Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html) e [Analyze text with Language Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html).
## Passo a passo
Entramos no [Azure AI Speech Studio](https://speech.microsoft.com/) com a sua conta vá nas configurações selecione um recurso ou crie um novo Subscription e aperte o butão "Usar recurso".
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/fala-texto_img1.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/fala-texto_img2.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/fala-texto_img3.png"/>
Para este teste eu escolhi colocar um trecho da musica Let It Go em Ingles do filme Frozen, assim foi mais facil para mim perceber que a capitura é execelente, mas tem um pequeno erro: acaba juntando as frases que em teoria teriam acabado, pois tem uma pausa por ser uma musica achai a detecção muito precisa em geral. 

Entramos no [Language Studio](https://language.cognitive.azure.com/) crie a conte como a seguir:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/analize-texto_img1.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/analize-texto_img2.png"/>
Espere a implantação ser concluída e volte para o Languege Studio, em seguida:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/analize-texto_img3.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/analize-texto_img4.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Análise-de-Sentimentos/img/analize-texto_img5.png"/>
Coloque o texto na caixa de texto ou arraste e solte o arquivo de texto ou procure o arquivo e concorde com "I acknowledge that running this demo will incur usage and may incur costs to my Azure resource." e execute vendo qual é o sentimento predominate.

Os arquivos estão na pasta [inputs](https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/tree/main/Análise-de-Sentimentos/inputs).