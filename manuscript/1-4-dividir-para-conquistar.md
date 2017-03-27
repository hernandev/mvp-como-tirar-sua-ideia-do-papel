# 4 - Dividir Para Conquistar

Você talvez já tenha ouvido essa frase em inúmeros locais. Ela se refere a, ganhar controle por fragmentar as maiores concentrações de poder, de modo que o mesmo não se mantenha indivualmente.

Apesar de eu ter usado a frase, e ela se encaixar bem como título do capítulo, não é exatamente disso que irei falar aqui.

Lembra aquele projeto de 400 horas? Como traçar um plano de trabalho que irá se manter, sem sugar todas suas energias, sem te fazer cair os cabelos, nem decepcionar ninguém (principalmente, a você mesmo)?

De modo simples, o que funcionou pra mim, de forma explêndida e foi novamente comprovado durante o desenvolvimento do MVP da [Kino](https://sejakino.com.br), é tratar o desenvolvimento como vários pequenos projetos.

Vamos chamar esses pequenos projetos de **etapas**. Vamos fazer pois é exatamente o que eles são. 

Ao invéz de te dar a teoria, vamos falar sobre isso na prática.

Quando primeiramente, eu e o [Vinicius Reis](https://github.com/vinicius73) analisamos o escopo do projeto da Kino, tínhamos em mente algo em torno de 800 horas brutas de desenvolvimento.

Lembre se que eu falei no capítulo anterior, use horas somente como um meio, não como elo.

Levantamos o escopo inicial do projeto, tudo aquilo que precisava ser desenvolvido.

Esse escopo, como disse no inicio do livro, foi negociado para ser reduzido drasticamente, até chegarmos a um escopo de MVP.

Como desenvolvedor, que precisa botar comida na mesa (mesmo que as vezes figurativamente), talvez pense negociar um contrato pra baixo, é algo ruim, visto que irá trabalhar menos, e consecutivamente, receber menos.

É comum pensar assim, porem nada poderia estar mais longe da realidade. É melhor entregar bem, um escopo menor, e depois disso, com todos satisfeitos, negociar novamente a continuidade do projeto e funcionalidades adicionais.

O rumo desse projeto tomou mudanças drásticas, que você irá acompanhar ao longo desse livro, mas por enquanto, vamos nos ater aos primeiros dias. Eles são extremamente fundamentais.

O escopo inicial chegamos a 6 meses de desenvolvimento, até o MVP da Kino estar concluido, e assim poderíamos iniciar outro estágio, de funcionlidades adicionais.

Como eu havia dito, a nossa estimativa era de 800 horas, ao longo de 6 meses, para 2 desenvolvedores. Uma média de 133 horas por mês, o que resultam em 66 horas pra cada desenvolvedor.

Como chegamos a conclusão de 6 meses? Simples, dividimos o projeto em 6 etapas, 6 pequenos projetos onde todos os envolvidos, ao final de cada mês, poderiam testar, aprovar e dar seguimento ao projeto.

Mas calma, vamos entrar em detalhes, mas antes, vou lhe apresentar um problema de grandes projetos.

## 4.1 - Síndrome do Burro do Shrek

Mesmo o título sendo meio brega, essa seção é importante. Se durante os 6 meses de desenvolvimento, fossemos marcar reuniões e mandar emails esporádicos sobre o progresso, a ansiedade e falta de comunicação pode se tornar um fator decisivo ao sucesso do projeto.

O cliente vai ficar igual ao Burro do Shrek, perguntando se "já chegamos" todo dia no Skype, no telefone. Isso gera um desgaste enorme para ambas as partes.

## 4.2 - Entregue Sempre

Se você conhece um pouco de scrum, deve estar acostumado com o termo "Sprint", uma pequena unidade de tempo, medida em dias ou semanas, onde um conjunto de tarefas é determinado, e ao final desse período, o "product-owner" sabe que alguma coisa será entregue.

O que estou me referindo aqui não é exatamente sobre sprints, é sobre uma unidade um pouco mais relaxada, que está acima da sprint.

Dividimos o escopo de trabalho da seguinte maneira:

- Criar uma lista de tudo a ser feito.
- Classificar as tarefas por ordem de dependência (por exemplo, Auth vem antes de ACL, etc)
- Dividir o trabalho em unidades de 3 semanas, que vamos chamar de etapa.
- Reservar uma semana pra ajustes a cada etapa.

Dessa forma, você faz com que o trabalho dite o cronograma, e não o contrário.

Recuperei aqui do email, o planejamento que fizemos para a Kino, assim você tem uma versão palpável do que estou falando:

**Primeira Etapa**

- Desenvolvimento de Interfaces do Sistemas
- Desenvolvimento do esqueleto das distintas áreas do sistema
- (1 item reduzido).

**Segunda Etapa**

- Controle de Contas a pagar
- (2 items reduzidos).

**Terceira Etapa**

- Assinaturas Recorrentes
- (3 items reduzidos).

**Quarta Etapa**

- Integração NFSe PBH.
- (2 items reduzidos).

**Quinta Etapa**

- Sistema de Notificações.
- (5 items reduzidos).

**Etapa Final**

- Ajustes, Bugs e Melhorias

Veja que a quantidade de items por etapa varia, pois cada item tinha uma estimativa diferente de trabalho. Mas tínhamos estimado com segurança, que era possível desenvolver os items de cada etapa durante 3 semanas.

Feito isso, o product owner sabia exatamente, que ao final de 3 semanas, iriamos testar juntos o que foi desenvolvido, e durante a quarta semana, iriamos fazer correções e ajustes.

Essa é uma forma de não criar o atrito do Burro do Shrek, nós sabíamos exatamente o tempo que tínhamos pra desenvolver um escopo limitado. O product owner sabe exatamente quando irá testar o sistema e dar feedback, e as correções mais urgentes não iriam ser deixadas para depois.

Encerrada uma etapa, tínhamos uma parte do sistema, pronta, testada, e as energias renovadas pra iniciar a próxima.

O ciclo se repete, se você ler esse capítulo com calma, perceberá que é algo realmente simples de se pôr em prática, mas alguns cuidados devem ser tomados.

- O product owner precisa entender, antes de qualquer contrato o modelo a ser seguido.
- Assim como qualquer política, não é possível implementar sem empenho e responsabilidade entre as partes.

Ainda não disse sobre a etapa final, de ajustes. Mesmo seguindo essa metodologia, problemas irão aparecer fora do escopo da etapa, um bug de uma funcionalidade da primeira etapa pode aparecer somente durante o decorrer da terceira.

Tudo Bem! Existe um momento, ao final onde tudo é retestado, e as 3 semanas da etapa ficam exclusivamente para fechar pontas soltas. Retestar e assegurar a qualidade do MVP.

Lembra sobre os 6 meses? Basicamente, estipulamos que, o escopo completo (que havia sido reduzido) poderia ser concluido em 5 iteraçes de 3 semanas. Como cada iteração tem 1 semana adicional para correções, chegamos a 1 etapa por mês. 5 meses de desenvolvimento, e uma etapa de melhorias.

## 4.3 - Mas o Cliente Tem Pressa!

Não, o cliente não tem pressa, ele somente pensa que tem.

Cabe ao desenvolvedor, explicar minimamente ao proponente, que "a mona lisa não foi pintada em 10 minutos". Para que se haja um mínimo de qualidade, é necessário tempo.

Quando digo tempo, me refiro ao tempo do capítulo anterior, e não a horas de desenvolvimento. Existem todos os fatores citados anteriormente a serem levados em conta.

Você pode até expremer 800 horas de desenvolvimento em 2 meses. Mas não irá conseguir concluir nem a metade do escopo. 

Com a correria começa a falha de comunicação, os erros constantes, e principalmente o retrabalho.

O espaço entre as atividades, o prazo prolongado pra se pensar e testar software é o que possibilitou o desenvolvimento da Kino se dar dentro desse espaço de tempo.

Se tivéssemos atacado com unhas e dentes o projeto, pra terminá-lo em 2 meses, o projeto teria falhado e você provavelmente não estaria lendo esse livro agora.

Se o cliente exige a urgência, deixe passar.

Se você quer lançar seu produto/startup que tem um software complexo em 2 meses, não o faça.

Simplesmente pelo fato de que, é impossível fazer com qualidade.

## 4.4 - Mantendo a Sanidade

Sabe quando falamos dos problemas pessoais? Basicamente, nesse modelo, você fica livre para tê-los. O projeto, estruturado dessa forma vai suportar alguns dias de folga, você vai ter tempo livro pra passar com sua família e resolver seus problemas pessoais.

Vai poder ainda, dar manutenção naquele projeto de um cliente antigo, ir a uma conferência, quem sabe pegar um freela rápido entre ou durante as etapas.

Estruturando seus projetos dessa forma, você garante que o projeto não irá sugar suas forças. Você pode inclusive, o fazer de forma paralela com outras atividades que demandam igualmente tempo (inclusive seu trampo CLT, se tiver coragem).

## 4.5 - Onde entra o Scrum Nessa Hitória?

Lembra que falamos sobre sprints certo? Você não precisa usar scrum por completo (apesar de eu gostar muito). Se você optar por usar, deixo como dica definir cada semana de uma etapa em sprints.

Dessa forma, cada etapa terá 4 sprints.

Você pode fazer isso, no primeiro dia de uma etapa, olhar as funcionalidades a serem desenvolvidas e quebrá-las em tarefas.

Dessa forma você tem um controle refinado do progresso da etapa, e consecutivamente do projeto.

A parte interessante é que, você não precisa criar 1000 entradas no backlog de tudo que tem que ser desenvolvido durante o projeto, você pode, simplesmente, criar o backlog especificamente para a etapa.


## 4.6 - Orçamento

Esse ponto é importante, e eu talvez quebre essa seção em um capítulo a parte.

Como agora você tem exatamente um framework para trabalhar seu projeto, sabe com relativa precisão quando ele será terminado, tem uma base muito mais realista de como cobrar pelos seus serviços.

Você pode definir um valor por etapa, e então aplicar esse valor ao número de etapas necessárias, incluindo a etapa de ajustes finais.
