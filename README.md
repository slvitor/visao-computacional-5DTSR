# MBA FIAP Inteligência Artificial & Machine Learning
## Visão Computacional: Detecção Liveness
Atenção: este notebook foi desenhado para funcionar no Google Collab.

Uma determinada fintech focada em consumidores finais pessoa física constataou um grande número de fraudes em transações bancárias.

O setor de fraudes apontou que existem clientes que se queixaram de não contratar serviços específicos, como o crédito pessoal, e após isso transferir para outras contas desconhecidas.

Após análises pelas equipes de segurança, os protocolos de utilização da senha foram realizados em conformidade, ou seja, cada cliente autenticou com sua própria senha de maneira regular.

Em função disso, o banco precisa arcar com reembolsos e medidas de contenção para evitar processos judiciais, pois os clientes alegam terem sido invadidos por hackers ou algo parecido.

Uma das formas de solucionar ou minimizar este problema é com a utilização de outras formas de autenticação, sobretudo em operações críticas, como a obtenção de crédito pessoal.

Desta forma podemos implementar uma verificação de identidade com prova de vida (liveness), que utilize uma verificação e identificação facial.

Caso o cliente não seja autenticado, ele será atendido por uma esteira dedicada e as evidências da não identificação serão encaminhadas para a área de IA para validação dos parâmetros e limiares para aperfeiçoamento do modelo.

Será necessário construir:

Detector de faces
Identificação de faces (podendo ser um comparador entre um rosto de documento e outra da prova de vida)
Detecção de vivacidade (liveness) para evitar que um fraudador utilize uma foto estática.
Formas alternativas de prover a identificação e prova de vivacidade, além destas que foram solicitadas poderão ser submetidas.

![alt text](imagem/liveness.jpg)

## Instruções
Este projeto final tem como objetivo explorar os conhecimentos adquiridos nas aulas práticas.

Iremos constuir uma forma de validar se uma determinada imagem foi ou não adulterada e se trata de uma produção fraudade.

Existem diversas formas de validar a vivacidade, e neste sentido conto com a criatividade de vocês dado que já dominam encontrar uma face numa imagem, aplicar marcos faciais e até mesmo construir uma rede neural convulacional.

A abordagem mais simples é pela construção de uma rede neural com imagens de fotos de rostos de outras fotos e fotos de rostos sem modificações. Tal classificador deverá classificar se dada imagem possui vivacidade ou não com uma pontuação de probabilidade.

### Pacotes utilizados

* [OpenCV](https://opencv.org/)
* [Keras](https://keras.io/)
* [Matplotlib](https://matplotlib.org/)
* [MobilinetV2](https://keras.io/api/applications/mobilenet/) 


## Notebook do projeto

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/slvitor/visao-computacional-5DTSR/blob/main/Deteccao_liveness_mobilinet.ipynb)

Executar somete a etapa 5 Teste fima-a-fim. A aplicação irá carregar a arquitetura e os pesos do modelo que ja foi treinado.
