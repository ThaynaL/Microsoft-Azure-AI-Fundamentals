# Reconhecimento Facial e transformação de imagens em Dados no Azure ML
Passo a passo do desafio de projeto "Reconhecimento Facial e transformação de imagens em Dados no Azure ML" da DIO. Material para consulta: [Analyze images in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html), [Detect faces in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html) e [Read text in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html).
## Passo a passo
### Criando
Pra começar deve utilizar o Azure AI services do Microsoft Azure neste caso é preciso entre na sua conta e vá no campo de pesquisa e procure por Azure AI services multi-service account e crie em seguida configure o espaço a seguir (adicionando os nomes, selecione Pricing tier como Standard S0 e concorde com os termos).
### Entrando no Vision Studio
Quando estiver pronto temos que entrar em [Vision Studio](https://portal.vision.cognitive.azure.com/) com a sua conta selecione o Subscription e o Azure Resources que você acabou de criar, depois vá em View all resources.Seleciona o diretório como padrão e feche.

## Detectar rostos
Vá em Face -> Detect faces in an image, marque a alternativa "I acknowledge that this demo will incur usage to my Azure account." e clique em uma das imagens ou adicione uma foto para fazer a detecção.No link abaixo mostra a [documentação](https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/quickstarts-sdk/identity-client-library?tabs=windows%2Cvisual-studio&pivots=programming-language-csharp) com integrar em uma aplicação.

## Analise de imagens
Documentos/textos:Vá em Optical character recognition -> Extract text from images marque a alternativa e selecione a imagem, em baixo tem como utilizar em um modelo.
Descrever a imagem:Vá em Image analysis -> Add capitions to images marque a alternativa e selecione a imagem, em baixo tem como utilizar em sua aplicação, qual linhuagem tem suporte e mais informações.