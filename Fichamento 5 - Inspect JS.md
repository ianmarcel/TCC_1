# InspectJS: Leveraging Code Similarity and User-Feedback for Effective Taint Specification Inference for JavaScript

Dutta, Saikat; Garbervetsky, Diego; Lahiri, Shuvendu; Schäfer, Max. "InspectJS: Leveraging Code Similarity and User-Feedback for Effective Taint Specification Inference for JavaScript," in Proceedings of the Conference’17, July 2017, Washington DC, USA.

## 1. Fichamento de Conteúdo

O artigo apresenta o InspectJS, uma ferramenta desenvolvida para aprimorar a análise de contaminação em bibliotecas JavaScript, aproveitando a similaridade de código e o feedback do usuário. A análise de contaminação se concentra em especificar "*sources*" que podem retornar dados não confiáveis e "*sinks*" que não devem receber esses dados sem a devida sanitarização,todos esses termos são referentes a segurança,para não permitir ataques por terceiros. O InspectJS automatiza a geração dessas especificações de contaminação, superando desafios de modelos manuais que podem levar a alerta de análises ausentes ou espúrias, dessa forma otimizando o desempenho com relação à segurança. Utilizando uma combinação de técnicas de aprendizado de máquina e interação com usuários, o InspectJS propõe uma metodologia eficaz para inferir novas especificações de contaminação, contribuindo significativamente para a segurança de aplicações JavaScript.

## 2. Fichamento Bibliográfico 

- ***Sinks*** : Eles são pontos onde os dados são consumidos. Se os dados consumidos estiverem corrompidos, isso poderá resultar em uma vulnerabilidade em seu aplicativo.

- **Sanitarização** : Os sanitizadores são usados ​​para higienizar a entrada de dados de usuários ou ambientes, garantindo que os dados não sejam contaminados. Ao realizar essa higienização, você elimina o risco de dados contaminados serem consumidos por um coletor.

- **Análise de contaminação**: Focada em identificar "*sources*" que retornam dados potencialmente controlados por atacantes e "*sinks*" onde esses dados não podem entrar sem sanitarização.

- **Geração automática de especificações de contaminação**: Abordagens propostas para superar limitações de modelos manuais, utilizando mineração de especificações automatizadas.

- **Confiança na previsão**: O InspectJS atribui uma pontuação a cada candidato a especificação de contaminação, indicando a confiança na previsão informada.

- **Mineração de especificações automatizadas**: Usada como um meio para detectar modelos ausentes ou incompletos, apresentando especificações de contaminação previstas aos usuários para avaliação.


## 3. Fichamento de Citações 

- _"A análise de contaminação está geralmente interessada em especificações de origem que indicam APIs de bibliotecas que podem retornar dados não confiáveis ('contaminados') possivelmente controlados por um atacante malicioso".
- _"Muitas técnicas diferentes foram propostas na literatura para gerar automaticamente especificações de contaminação".
- _"Atribui-se a cada candidato uma pontuação entre zero e um, que indica intuitivamente quão confiantes estamos de que a previsão está correta".
- _"Para tornar isso viável, precisamos de uma maneira de apresentar especificações de contaminação previstas para uma análise".
