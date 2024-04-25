# Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados
Este arquivo é feito para mostrar o passo a passo para soluções de mineração de conhecimento com as devidas configurações segundo a documentação [Explore an Azure AI Search index (UI)](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html) e o video na [DIO](https://www.dio.me/).

## Criando modelo
Para utilizar este recurso é preciso ir ao [Microsoft Azure](https://azure.microsoft.com/pt-br/), primeiro recurso a ser utilizado é o Azure AI services, crie o AI Search com as seguintes configurações:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img1.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img2.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img3.png"/> 
Depois isso crie um recurso no Azure AI services.
Em seguida crie uma conta de armazenamento com as seguintes configurações:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img4.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img5.png"/> 
Para as configurações dentro da conta:
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img6.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img7.png"/>
Baixe as [avaliações de café](https://aka.ms/mslearn-coffee-reviewse) compactadas e em extraia os arquivos para a pasta de avaliações ou baixe deste repositório. No portal do Azure, selecione o contêiner e carregue-as selecionar os arquivos.
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img8.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img9.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img10.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img11.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img12.png"/> 
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img13.png"/>
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img14.png"/> 
Consulta:
Entrando no serviço e através do search explorer vamos testar se tudo foi indexado e se a consulta esta funcionando, utilizando os comandos:
``search=*&$count=true ``   (  verifica se a indexação esta funcionando e mostra os documentos )
``search=locations:'Chicago' `` ( Consulta as ocorrencias acontecidas em Chicado )
``search=sentiment:'negative' `` ( Consulta as ocorrencias com sentimento negativo )
<img align="center" src="https://github.com/ThaynaL/Microsoft-Azure-AI-Fundamentals/blob/main/Azure-Cognitive-Search/img15.png"/>