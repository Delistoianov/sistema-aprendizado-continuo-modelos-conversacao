# Proposta de Aprendizado Contínuo em Sistemas Conversacionais

**Autor:** João Lucas Delistoianov Gonzalez

## Introdução

O mundo está em constante transformação e evolução, e esse contexto abrange não apenas aspectos sociais, tecnológicos e culturais, mas também a maneira como nos comunicamos. O modo de falar, as gírias, expressões e sotaques não estão imunes a essas mudanças, sendo influenciados e moldados pela dinâmica da sociedade. Nesse contexto em constante mutação, surge um desafio significativo para manter atualizadas as inteligências artificiais que utilizam sistemas de conversação. Isso se aplica tanto ao processo de speech-to-text, em que a inteligência artificial deve compreender com precisão as necessidades do usuário, quanto ao text-to-speech, no qual é essencial que as respostas sejam formuladas de maneira clara e acessível para que o usuário compreenda plenamente o que está sendo comunicado.

Entretanto, a tarefa de manter as inteligências artificiais atualizadas ainda é um processo intrincado, para o qual ainda não existem soluções eficazes estabelecidas. Esses modelos armazenam conhecimento em seus parâmetros, porém, diante da constante evolução do mundo, esse conhecimento pode rapidamente se tornar obsoleto, o que é conhecido como "concept drift".. Nessa perspectiva, o desafio substancial reside em como cultivar uma inteligência artificial capaz de discernir entre os dados permanentes, que são imutáveis com o tempo, os dados que precisam ser atualizados e os novos dados que surgem constantemente. Além disso, a habilidade de discernir a veracidade de novas informações também é fundamental para que o modelo não transmita falsas informações.

## Solução Proposta

### Diagrama de Blocos

![Diagrama de Blocos](/assets/diagrama_bloco.jpg)

[Link para o miro](https://miro.com/app/board/uXjVNf0RyGY=/?share_link_id=637619826480)

### Descrição Textual

Cada bloco foi nomeado com um número para facilitar o entendimento.

B1 - Bloco de entrada dos dados. Os dados de entrada são os falas.

B2 - Bloco de conversão do áudio para texto.

B3 - Esse bloco divide os dados em 3 categorias diferentes de acordo com seu tipo.

B4 - Esse bloco são para dados que não devem sofrer alterações ao longo do tempo.

B5 - Esse bloco finaliza o processo de categorização dos dados.

B6 - Esse bloco são para dados que podem ser atualizados conforme o tempo.

B7 - Esse bloco são para novos dados.

B8 - Esse bloco checa se o novo dado existe no banco de dados.

B9 - Esse bloco são para dados que existem. Se o dado existir no banco de dados ele finaliza o processo, ou seja, volta para o bloco 5.

B10 - Esse bloco verifica se o novo dado é uma atualização de algum dado antigo.

B11 - Esse bloco são para dados novos.

B12 - Adiciona e  atualiza os novos dados.

B13 - Esse bloco treina de novo o modelo com os novos dados.

## Conclusão

A proposta apresentada visa aprimorar o processo de atualização de dados em modelos de aprendizado de máquina, abordando uma das questões mais desafiadoras enfrentadas pelos sistemas conversacionais que é a capacidade de manter-se relevantes e atualizados em um mundo em constante mudança.

Para aprimorar o processo de atualização de dados em modelos de aprendizado de máquina, foi proposta uma solução com o objetivo de otimizar a seleção de dados. Essa abordagem envolve a divisão dos dados em três categorias distintas. A primeira categoria é de dados estáticos, ou seja, permanecem inalterados ao longo do tempo. A segunda categoria abrange dados passíveis de alterações, que podem evoluir com o tempo, como gírias, expressões e informações sujeitas a mudanças culturais e sociais no contexto conversacional. A terceira categoria compreende novos dados, que são informações que ainda não foram incorporadas ao modelo. Essa classificação tem como finalidade simplificar o procedimento de reentrenamento do algoritmo, pois proporciona uma maneira eficaz de filtrar e categorizar os dados de acordo com suas características intrínsecas. Além disso, essa abordagem economiza processamento das máquinas.

Essa classificação cuidadosa tem como objetivo simplificar o procedimento de reentrenamento do algoritmo. Os dados estáticos formam a base inabalável do conhecimento, minimizando a necessidade de ajustes constantes. Os dados passíveis de alterações são atualizados periodicamente, permitindo que o modelo se adapte às mudanças na linguagem e nas preferências dos usuários. Por fim, os novos dados são tratados com cuidado, passando por um processo de verificação antes de serem incorporados ao conhecimento do sistema.

Além disso, o sistema proposto oferece a capacidade de discernir entre informações verdadeiras e falsas, garantindo que informações incorretas não sejam incorporadas ao modelo. Isso é fundamental para manter a qualidade e a credibilidade das respostas fornecidas pelo sistema.

No entanto, a implementação desse sistema de aprendizado contínuo oferece a perspectiva de melhorias substanciais na experiência do usuário e na precisão das respostas fornecidas pelos sistemas conversacionais. Ao lidar com o conceito de concept drift e adotar uma abordagem proativa para a atualização de dados, o sistema tem o potencial de se tornar uma ferramenta valiosa em um mundo em constante transformação, mantendo-se relevante e eficaz em suas interações com os usuários.

## Referências Bibliográficas

1. Joel Jang, Seonghyeon Ye, Sohee Yang, Joongbo Shin, Janghoon Han, Gyeonghun Kim, Stanley Jungkyu Choi, Minjoon Seo. "Towards Continual Knowledge Learning of Language Models." KAIST AI, LG AI Research em TOWARDS CONTINUAL KNOWLEDGE LEARNING OF
LANGUAGE MODELS. 
[Link para o artigo](https://arxiv.org/pdf/2110.03215.pdf)


2. Shivali Agarwal, Shubham Atreja e Gargi Dasgupta em Continuous Learning as a Service for Conversational Virtual Agents
[Link para o artigo](https://link.springer.com/chapter/10.1007/978-3-319-69035-3_47#author-information)