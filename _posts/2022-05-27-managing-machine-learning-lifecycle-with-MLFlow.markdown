---
layout: post
title: "Managing machine learning lifecycle with MLFlow - Script"
date: 2022-05-27 12:30:00 -0000
---

# Introdução

Bom dia a todos, 
É um prazer estar aqui no TDC falando com vocês, essa é a primeira palestra presencial que eu dou então espero que vocês curtam, meu objetivo aqui é deixar vocês com vontade e um norte para criar pipelines de inteligência artificial robustos, escaláveis e performáticos.
Minha ideia aqui é apresentar um protótipo de uma pipeline que independente da indústria de atuação pode ser considerada sólida, eu atualmente trabalho numa startup aqui de florianópolis chamada BoletoFlex, nós concedemos crédito para pessoas que não tem acesso pelos bancos tradicionais ou não pode onerar o limite do cartão de crédito com gastos em bens de consumo duráveis. Isso na prática significa que somos uma instituição financeira que concede crédito a partir do varejo, estamos presentes como forma de pagamento no checkout da mobly, da cvc, da ame e diversas outras lojas. 

E assim como toda instituição financeira que utiliza modelos de inteligência artificial, nossos erros de modelagem podem custar muito caro e dependendo do grau de dependencia da empresa nos modelos, erros podem quebrar uma instituição, seja elevando nível de inadimplência, não identificando fraudes corretamente, e etc.

Portanto eu vou apresentar uma solução conceitualmente simples, mas que a partir dela é possível extrapolar para praticamente qualquer caso de uso, eu vou trazer um exemplo de arquitetura e algumas ferramentas que podem auxiliar na construção de todas as etapas de um projeto de machine learning, e tornar o ciclo de vida desse modelo virtuoso, em que a cada retreino periódico que for fazer eu não precise construir tudo do zero, e a cada a iteraçao ele melhore. E a gente só precise matar esse modelo e fazer outro quando ele não fizer mais sentido existir.


# Falando de MLOps

Bom, para iniciar a minha apresentação eu quero trazer alguns conceitos fundamentais do tema que iremos tratar, e preciso admitir que fiquei muito surpreso quando olhei o cronograma da trilha e eu seria o unico que falaria sobre MLOps, eu já tinha a impressão que era um tema que nunca esteve tão em alta, mas como bom cientista de dados que eu acredito que eu seja, fui atras de dados quando tava construindo essa apresentação, e de fato minha intuição tava correta, a tendência de pesquisas do termo MLOps é positiva. A máxima histórica foi atingida no fim do mês passado e assim como o mercado de ações vem sofrendo uma correção ao longo das últimas semanas, o que demonstra com bastante certeza a importância do tema, a gente para de pesquisar MLOps e o mercado cai, isso não é coincidencia. Não vou me aprofundar nessa teoria agora, não é o objetivo, da palestra a gente pode deixar essa conversa para o almoço.

![image tooltip here](/assets/images/mlops-trends.png)

Enfim, tirando a piadinha infame, MLOps está sendo o buzzword de quem superou o buzzword "inteligência artificial e machine learning e etc." Mas, assim como inteligência artificial, é um assunto que que tem motivo para ser falado, e o objetivo dessa disciplina é tornar os cientistas de dados capazes de mais do que só desenvolver modelos em notebooks, é criar modelos modelos e entregar um processo robusto e que permita que os modelos evoluam ao longo do tempo. O desafio da ciência de dados, pelo menos no mercado, porque na academia os objetivos são um pouco diferentes, não é criar criar modelos de machine learning, é criar soluções que entram em produção, fazem parte do fluxo da empresa em que tão presentes e agregam valor, aí de preferência é claro utilizando machine learning.

# Apresentação de ferramentas

Eu vou trazer aqui rapidamente as ferramentas que vamos usar nessa demonstração, eu não vou me ater a explicar profundamente o funcionamente delas, primeiro porque eu acho que não vai ser absorvido, e segundo porque a documentação vai fazer isso 