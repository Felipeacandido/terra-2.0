### Animação-CSS "Terra"

![Vídeo sem título ‐ Feito com o Clipchamp](https://github.com/Felipeacandido/Anima-o-CSS/assets/161148912/5f55d9d7-0279-4a33-a7f9-a26416665e7f)

https://codepen.io/Felipeacandido/pen/jOoPKvN

Este código simula a Lua orbitando ao redor da Terra em um ciclo contínuo de 5 segundos, mudando de posição em relação ao observador (passando por trás da Terra a cada metade do ciclo). A animação utiliza uma combinação inteligente de CSS para o movimento e a profundidade visual. É uma maneira simples e eficaz de criar uma representação visual do movimento orbital sem a necessidade de scripts complexos.

*HTML*


O HTML define uma estrutura básica com um div para o planeta (Terra) e outro div para o satélite (Lua), ambos contidos em um div de classe container.

*CSS*

Estilização Geral
Reset CSS: Os estilos globais removem as margens e o preenchimento padrão dos elementos, além de definir a cor de fundo do corpo para um cinza escuro, criando um fundo que simula o espaço.
.container

Posicionamento e Tamanho: O container é dimensionado e centralizado na tela usando position: absolute e transform: translate(-50%, -50%). Isso cria um centro fixo para a animação.
.terra (Terra)

Estilização e Posicionamento: A Terra é estilizada como um círculo azul usando border-radius: 50% e posicionada centralmente dentro do container.

Detalhes Decorativos: O uso de :before com múltiplas sombras box simula características geográficas na superfície da Terra, como continentes e ilhas.
.lua (Lua)

Estilização e Posicionamento: A Lua também é um círculo, mas de cor cinza. Inicialmente, ela é posicionada à esquerda da Terra.

Animação: A animação chamada spin move a Lua de sua posição inicial para a direita da Terra e depois de volta, mudando também sua profundidade z-index para criar um efeito de passar por trás da Terra.

*Animação @keyframes spin*

Movimento: A animação é definida para executar indefinidamente (infinite) com uma duração de 5 segundos. Ela muda a posição da Lua (propriedades bottom e left), assim como a z-index para manipular a Lua passando por trás da Terra no ponto médio da animação.

