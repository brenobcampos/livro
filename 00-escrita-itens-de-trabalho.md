# Escrita de Itens de Trabalho

Esse capítulo se dedicará a realizar uma introdução ao tema de escrita de itens de trabalho.

## Para quem é esse capítulo?

Este capítulo se destina especialmente para pessoas que estão entrando agora no mundo do desenvolvimento ágil, e precisam com urgência saber como se tratam os itens de trabalho (ou _work items_) de maneira básica, algo como _"Me jogaram hoje num projeto agile, e eu não faço a menor ideia de como escrever um item de trabalho, socorro!"_. A ideia é que você componha uma base de conhecimento para reduzir possíveis problemas causados por itens mal escritos. Todo o conteúdo apresentado será a base para o ínicio de um projeto e, ao longo dos demais tópicos, você poderá aprimorar esse conhecimento.

Dessa forma, caso você se encontre com a corda no pescoço e precise resolver seus problemas o mais rápido possível, a leitura deste capítulo pode acelerar essa transição. Depois que a situação se acalmar, as outras técnicas contidas nesse livro podem não só resolver seus problemas como também levar seu time ao alto desempenho.

Boa leitura! E sucesso na escrita de novos produtos!

## Introdução as _user stories_

### Qual a origem das _user stories_?

Bem, vamos falar um pouco das _user stories_, começando pelo seu surgimento (aqui, trataremos também por _**US**_). 

_User stories_ ou _histórias de usuário_ são, em alguns casos, a forma como são documentados os requisitos de software dentro de um contexto ágil. Elas surgiram há um certo tempo (a primeira descrição vem de 1998), dentro de uma metodologia chamada *eXtreme Programming*, ou *XP*. Essa foi a forma encontrada pelos seus criadores, de registrar as demandas de clientes (ou usuários) de forma a tratá-las durante o desenvolvimento. Na época, foi dito que elas deveriam ser utilizadas para definir o escopo do projeto, assim como _casos de uso_.

As _US_ tem esse nome pois devem (ou deveriam) representar a visão de um usuário acerca do que precisa ser feito para a geração de um incremento de produto. Como assim? Bem, a ideia primordial de uma _US_ é que ela represente uma necessidade real de um usuário, na forma como ele vê o problema e como ele gostaria que fosse resolvido. Por conta disso, foi criado um _"formato padrão"_ de escrita de demandas, que de fato, conta uma _"historia"_.

### Quais as boas práticas para escrever _user stories_?

Bill Wake, compilou em um artigo de 2003 algumas boas práticas sobre a escrita de _user stories_ que, até hoje, são utilizadas direta ou indiretamente. Seu artigo _["INVEST in Good Stories, and SMART Tasks"](https://xp123.com/articles/invest-in-good-stories-and-smart-tasks/)_ dá dicas de certas características desejáveis na escrita de _US_.

Mas antes de analisarmos estas características, que tal conhecermos (ou relembrarmos) o que são funcionalidades (_features_), _user stories_ (ou como trataremos ao longo do livro, **itens de trabalho**) e tarefas (_tasks_). Funcionalidade, ou _feature_, é uma ação ou comportamento do sistema em que podemos visualizar início e um fim, isto é, algo que é executado pelo sistema. Quando seu celular abre aplicativos com sua digital, isso é uma funcionalidade que se inicia ao tocar o botão e se encerra ao aplicativo ser aberto. Já _user story_, como explicado anteriormente é uma forma de documentar as funcionalidades do software, o desbloqueio por digital, por exemplo, pode ter sido desenvolvido com base em uma ou mais _user stories_ que guiaram o desenvolvimento da funcionalidade. Já tarefas são partes menores da _user story_, ou seja, pequenos incrementos de escopo dentro da _US_).

Vejamos agora, o que significam os acrônimos apresentados por Bill Wake.

**INVEST** é um acrônimo que significa:

> I - Independent
> 
> N - Negotiable 
> 
> V - Valuable
> 
> E - Estimable
> 
> S - Small
> 
> T - Testable

Vamos entender cada um dos pontos?

**Independente (_Independent_)**
A _user story_ precisa, como o nome diz, ser independente. Ou seja, de preferência, ela não deve depender de nenhuma outra dentro do fluxo de desenvolvimento. Isso quer dizer que pode ser implementada na ordem que for necessária.

**Negociável (_Negotiable_)**
Quer dizer que os detalhes referentes a funcionalidade podem ser negociados entre desenvolvedor e _product manager_, desde que não afete o objetivo final. Muito ligado a **como** será feito, mantendo a essência de **o que** será feito.

**Valiosa -ou deve possuir valor- (_Valuable_)**
Em vias gerais a _user story_ **deve** gerar valor, ou seja, deve entregar um benefício a alguém. Entregar algo que possa ser usado, e que agregue ao cliente.

**Estimável (_Estimable_)**
Quando falamos de estimativa, a ideia é ter uma base do tamanho/esforço necessário para o desenvolvimento da funcionalidade, não uma medida exata (por isso **estimativa**), mas algo que nos ajude a elencar prioridade e definir uma ordem de desenvolvimento.

**Pequena (_Small_)**
A ideia principal, é que a _user story_ tenha um tamanho referente ao trabalho de uma pessoa durante poucas semanas ou poucos dias. Um tamanho bom, é de até 2 semanas (10 dias de trabalho), pois desta forma o desenvolvedor consegue entregar valor sem passar muito tempo travado numa mesma demanda.

**Testável (_Testable_)**
É extremamente importante que seja possível testar o que se desenvolve. Se você não sabe como testar o que escreveu, como saberá se ela atende o que você precisa? Caso haja dúvidas sobre teste, há grandes possibilidades da _user story_ estar com informações incompletas.

Agora, falando de tarefas temos o conceito de **SMART** que descreve:

> S - Specific
> 
> M - Measurable
> 
> A - Achievable
> 
> R - Relevant
> 
> T - Time-boxed

Descrevendo cada tópico, temos que:

**Específica (_Specific_)**
A tarefa deve ser específica o suficiente para que todos os envolvidos no desenvolvimento tenham plena ciência do que é necessário ser feito/testado. Dessa forma evitamos que hajam tarefas semelhantes e que duas delas tratem da mesma coisa, diminuindo o risco de desperdício de esforço quando duas pessoas atuam na mesma _user story_.

**Mensurável (_Measurable_)**
Deve ser possível medir e saber quando a tarefa está pronta, delimitando bem seu escopo de desenvolvimento frente à história desenvolvida.

**Alcançável (_Achievable_)**
É possível entregar essa tarefa? É possível desenvolvê-la? O responsável pode entregá-la? Ou é simplesmente impossível realizar tal tarefa?

**Relevante (_Relevant_)**
Essa tarefa é relevante para o incremento de escopo esperado da _user story_? Agrega valor ao produto, ou seja, gera algum benefício para quem está utilizando? É esperado que cada tarefa possa ser explicada e justificada dentro de uma possível reunião para esclarecimento da _user story_.

**Com tempo definido (_Time-boxed_)**
As tarefas precisam ter um tempo definido, não necessariamente uma medida de _X_ horas ou _Y_ dias. Mas é necessário ter uma certa ideia de quando será entregue, para que seja possível _levantar uma bandeira de atenção_ caso esta tarefa leve mais tempo que o esperado e se possa avaliar o que pode ser melhorado, ou o que poderia ter sido evitado/feito diferente.

### Conclusão

Os conceitos apresentados anteriormente guiam a boa escrita de _user stories_ dentro do mundo da agilidade. São boas práticas que podem, ou não ser seguidas. A ideia é que estas boas práticas auxiliem na escrita de itens de trabalho claros e mais concisos. Não são leis ou regras, são atributos desejáveis que nem sempre poderão ser atendidos em todos os itens de trabalho escritos. Seguir estas prtáicas não garantem o sucesso de sua escrita, entretanto aumentam as chances de a comunicação ser mais efetiva.

Por último, cabe destacar que com a chegada de novas metodologias, novos conceitos e novas ideias dentro da area de gerenciamento ágil de projetos uma nova terminologia vem sendo utilizada: **Item de trabalho** ou em inglês **_Work Item_**, esta terminologia vem sendo bastante utilizada pela comunidade Kanban. Neste livro trataremos o escopo que precisará ser escrita por este nome: item de trabalho.

## Como escrever um item de trabalho

### Que formato posso utilizar para escrever meu item de trabalho?

Podemos utilizar o formato que foi tomado por "convenção" de uma _user story_ como exemplo, este é:

> Eu, como _"cliente/usuário/operador"_ gostaria de _"ação que necessito que o sistema realize"_ para que _"objetivo final a ser alcançado"_.

Desta forma, é possível ter uma visão básica de **o que** precisa ser feito, mas não necessariamente **como** precisa ser feito. Muitos times realizam a escrita dos itens de trabalho fisicamente em uma ficha pautada (que pode ser encontrada em qualquer papelaria). Outros times que trabalham remoto, acabam adicionando os itens em um software ou serviço de gerencimento de projetos, como o [Jira](https://br.atlassian.com/software/jira) ou o [Trello](https://trello.com/), por exemplo.

No caso de uma ficha pautada, a parte da frente representa a descrição do item de trabalho, e no verso devem ser escritos "detalhes" sobre a funcionalidade. 

Não há um padrão sobre como detalhar, e muitas das publicações e da literatura existente não dão grandes pistas sobre como fazer isso, deixando um novato em certos apuros sobre como detalhar o que precisa ser feito, ou como saber se o que precisa ser feito foi realmente concluído e da maneira correta. Tudo o que se diz é: "detalhe o que precisa ser feito no verso, e adicione informações complementares.".

A ideia principal de um item de trabalho é que ela sirva de comunicação entre o time, dos stakeholders aos desenvolvedores. Desta forma, é necessário clareza na escrita do item (**o que** precisa ser feito) e no detalhamento (**como** precisa ser feito), para que silos de comunicação sejam evitados, ou pelo menos diminuídos. Estes geralmente geram demandas que são completamente descartáveis por terem sido feitas com um entendimento divergente do escopo original.

Veja, não estou jogando a culpa no desenvolvedor. Como disse anteriormente a ideia de um item de trabalho é promover a comunicação, e esta é responsabilidade de ambos: tanto emissor quanto receptor. Aquela velha conversa de que "Sou responsável pelo que falo, não pelo que você entende" não faz o menor sentido. A comunicação deve ser clara, objetiva e efetiva. O emissor deve garantir que o que receptor entenda a informação assim como o receptor deve ter certeza de que entendeu exatamente o que o emissor queria comunicar.

Desta forma, existem algumas boas práticas que podemos adotar durante a escrita dessas funcionalidades.

A princípio vamos entender como utilizar o modelo "clássico de uma _user story_, ao final deste capítulo apresentaremos um exemplo de construção de produto. Utilizando o que foi mostrado anteriormente temos:

> Eu, como _"cliente/usuário/operador"_ 

Essa primeira parte representa a pessoa que vai utilizar ou operar determinada funcionalidade do sistema, o qual é o principal interessado no bom funcionamento do que será desenvolvido. Logo, é a visão dele que importa para o que será desenvolvido. 

Definindo-se quem é o interessado na funcionalidade, seguimos para a parte que diz:

> gostaria de _"ação que necessito que o sistema realize"_ 

Essa segunda parte representa a funcionalidade em si, o que precisa ser implementado. Qual o objetivo do card criado? O que o cliente espera ao final deste incremento de produto? 

Desta forma, sabendo-se quem é o interessado, e o que precisa ser feito para atendê-lo. É necessária uma justificativa ou bom motivo para o desenvolvimento do item de trabalho, por qual razão eu quero que isso seja feito?

>para que _"objetivo final a ser alcançado"_.

Assim, sabe-se o que será feito e qual a motivação para isso. Conhecendo as razões para desenvolver o item, é possível que o time possa opinar e dar melhores soluções ou formas mais simples de se entregar determinado benefício ou valor ao produto.

Seguindo estes passos, você acaba de escrever uma clássica _user story_, entendendo quem é o interessado na funcionalidade, o que ele precisa que seja feito, e por qual razão ele precisa que seja feito.

Essa é uma das formas mais lúdicas de se escrever itens de trabalho. Há pessoas que escrevem de forma diferente, mais direta e menos lúdica. Chamando apenas de "Motivação" a junção de todos os campos acima.

Em alguns projetos talvez essa escrita simples seja o suficiente para o desenvolvimento da funcionalidade, para projetos menores e/ou com menos restrições talvez seja válido e deve ser por isso que algumas pessoas dizem que *user stories* ou itens de trabalho são como convites para conversas, que devem ser desenvolvidas em cima da motivação proposta. Entretando projetos maiores e mais complexos necessitam de mais informações para o bom andamento do escopo.

Desta forma, podemos adicionar melhores esclarecimentos na descrição do item de trabalho. Existe um campo próprio pra isso no Jira e no Trello, por exemplo. Já na ficha pautada, pode-se sempre usar o verso do cartão com esse intuito.

Podemos pensar que há perguntas que não são respondidas no pequeno texto que conta uma história. Como restrições de negócio e restrições técnicas, por exemplo. Que tal pensar em um padrão para descrever o que foi pontuado anteriormente?

Adicionando uma sessão de dúvidas, sejam de negócio ou técnicas, auxilia a manter o alinhamento do time quanto a questionamentos levantados durante a etapa de análise do item, essas dúvidas podem ser removidas no momento do _Refining_ do item (falaremos disso no capítulo XXX).

Desta forma, no verso do nosso cartão podemos adicionar um campo de dúvidas. Costumo separá-las em "Dúvidas Técnicas" e "Dúvidas de Negócio". Sendo assim, durante a etapa de discutir a funcionalidade, tais questionamentos são melhor endereçados as pessoas que podem respondê-los.

Assim, o campo de descrição da ferramenta online ou o cartão físico ficariam:

> Dúvidas
> * Negócio
> 	* Aqui vai uma dúvida de negócio.
> 	* Aqui vai outra dúvida de negócio.
> * Técnicas
> 	* Aqui vai uma dúvida técnica.
> 	* Aqui vai outra dúvida técnica.
> 	* Aqui vai mais uma dúvida técnica.

Com dúvidas adicionadas, o que mais faltaria? Como saber se o item de trabalho está pronto após o desenvolvimento? Quais critérios eu tenho pra saber se foi concluído? Adicionando um campo para **critérios de aceite**, consegue-se validar quando um item está pronto, ou não.

Critérios de aceite auxiliam, e muito, na comunicação do time. Pois enquanto a descrição do item nos diz **o que** precisa ser feito, os critérios nos dizem **como** precisa ser feito. E isso nos traz os seguintes benefícios:

* Há um comprometimento dos desenvolvedores do que eles precisam desenvolver para determinada funcionalidade, ou seja, qual o escopo desta funcionalidade.
* Se cria o comprometimento do responsável de negócio, de que ele passou as especificações corretas do que a funcionalidade precisa apresentar para ser validada (lembra do aceite do PO lá do Scrum?);
* O _QA_ (analista de qualidade, ou testador) fica ciente do que está incluso no escopo da funcionalidade, e o que ele deve testar e verificar se apresenta o comportamento esperado;
* Cria o entendimento do time como um todo, de qual valor estará sendo gerado por este incremento de produto.

Além de critérios de aceite há ainda outro recurso que podemos (e devemos na medida do possível) utilizar, são wireframes e prototipações da tela, mostrando como será a jornada de usuário dentro da funcionalidade. Desta forma, todos terão a mesma visão do como será construído, e conseguiremos mais facilmente realizar testes e validações.

É interessante adicionar também um campo com dependências externas, seja de outros times dentro do mesmo projeto ou produto, ou de times externos (integração com sistemas de terceiros, por exemplo).

Outro ponto interessante de se perguntar ao escrever um item de trabalho é quais impactos ocorrerão por não entregá-lo? Ou que riscos isso traz ao negócio? Perda de clientes? Redução de receita mensal? Diminuição de participação no mercado frente aos concorrentes? Essas perguntas podem ajudá-lo durante a discussão do item para que possam simplificar o escopo e entregá-lo o mais rápido possível.

Pode-se adicionar também sessões com **Observações** ou **Pontos de atenção** acerca da funcionalidade, qual impacto ela traz ao produto? Métricas ajudam nisso, pois auxiliam na medição do valor entregue pela funcionalidade.

Outra sessão que pode ser adicionada **Como testar?**. Um item de trabalho um pouco mais técnico que exige trocas de ambiente, troca de status de um serviço ou análise de métricas pode esconder _edge_ cases perigosos. Auxiliar o analista de qualidade mostrando como testar pode otimizar o fluxo como um todo.

### Conclusão

A boa escrita de itens de trabalho está intimamente ligada ao nível de detalhamento que você dá ao que escreve. A comunicação se torna mais efetiva quando você pensa no que gostaria e precisaria saber, caso você fosse a pessoa que fosse ler o item. Desta forma, o formato do detalhamento é completamente aberto ao seu contexto. Podem haver casos que você não precise de observações ou dúvidas, mas que precise adicionar um campo que eu não citei. A ideia é que você possua flexibilidade e entenda suas necessidades para que possa evoluir seu item de trabalho de acordo com suas necessidades.

## Sessão mão na massa

### Sistema mobile de companhia aérea

Pensemos num sistema mobile de uma companhia aérea, por exemplo. Vamos criar um item de trabalho que solicite a realização de checkin para o vôo através do aplicativo.

Tendo em vista um cliente desta companhia, poderíamos descrever uma história para o usuário final, ou seja, o passageiro. Pensando no escopo definido acima, podemos escrever de duas formas. No estilo clássico de _user story_:

> Eu, como *passageiro* gostaria de *realizar o checkin dos meus vôos pelo aplicativo do meu celular* para que *eu possa agilizar os meu checkins, de forma que se torne mais fácil por já estar com o celular em mãos, e já utilizá-lo para apresentar os cartões de embarque*.

Ou de uma forma menos lúdica:

> **Motivação**: Para que um passageiro consiga otimizar o uso do aplicativo, além de somente exibição do bilhete de embarque é necessário que o aplicativo possua a opção de checkin.

Desta forma, damos conta da primeira parte da escrita de um item de trabalho, **o que** precisa ser feito. Agora podemos olhar a segunda parte, **como** entregaremos o que foi solicitado?

Como citado anteriormente, podemos adicionar mais campos na descrição, como dúvidas por exemplo. Levando em conta o cenário apresentado há perguntas que podem ficar no ar, certo?

Pensando em negócio:

> * Como saber qual o vôo do cliente?
> * Como saber se o cliente vai despachar bagagem?
> * Como saber se o checkin já está disponível para determinado vôo?

Pensando tecnicamente:
> * Onde consigo as informações de checkin?
> * Onde consigo número de vôo e assento que o passageiro comprou?

Nenhuma dessas perguntas é respondida pela motivação ou pela descrição lúdica, correto? Então podemos adicioná-las no detalhe do verso do cartão ou no campo descrição da ferramenta online.

Agora pensando em implementação mais direta:

> Como eu gostaria que fosse feito o checkin?

Na cabeça de alguém de negócio por exemplo, o usuário deve fazer o login no aplicativo mobile. Desta forma todos os próximos vôos serão exibidos para o cliente selecionar qual ele gostaria de fazer o checkin. Entretanto, na cabeça do desenvolvedor, pode vir a ideia de ignorar um possível login e de simplesmente solicitar para o usuário o código de reserva e o sobrenome do passageiro, para que desta forma ele possa retornar as informações de checkin. Concorda comigo que são duas abordagens que no final levariam ao mesmo fim - o checkin do usuário - entretanto teriam custos de desenvolvimento diferentes e experiências de usuário também diferentes? Inclusive ambas abordagens já são utilizadas nos sistemas WEB das companhias aéreas. Se essas opções não forem debatidas durante a discussão do item de trabalho, deixamos um silo de comunicação que pode ser interpretado por no mínimo duas formas diferentes.

Assim sendo, podemos escrever um critério de aceite da seguinte forma:

> O usuário deve realizar o login no aplicativo mobile, para que desta forma ele possa acessar todas as informações relativas ao seu vôo e assim escolher em qual vôo ele pode fazer o checkin.

Bom, não acha? Já temos um critério de aceite escrito! Mas, podemos melhorá-lo! Conseguiu perceber algo que poderia ser melhor descrito? Olha só:

> _"ele possa acessar todas as informações relativas ao seu vôo"_

O que são "todas as informações"? Podemos fazer melhor que isso! Podemos deixar bem descrito o que esperamos que o passageiro veja. Lembre-se: comunicação! Vamos focar na clareza! Que tal se reescrevermos desta forma:

> O usuário deve realizar o login no aplicativo mobile, para que desta forma ele possa acessar suas informações relativas ao seu vôo (data do vôo, horário do vôo, número de reserva, origem e destino) e assim escolher em qual vôo ele pode fazer o checkin.

Não ficou melhor? Estamos comunicando exatamente o que esperamos desta funcionalidade! Podemos continuar, incrementando os critérios de aceite:

> Ao selecionar seu vôo, o passageiro deve selecionar se pretende despachar bagagem através de um menu que conterá as opções "SIM" ou "NÃO".

> Ao selecionar a opção de "SIM" indicando que despachará bagagem, o aplicativo deve indicar ao passageiro para buscar a equipe de solo para entregar a bagagem a ser despachada.

> Ao selecionar seu vôo, o passageiro terá a opção de confirmar seu assento selecionado durante a compra, ou de alterar o assento para um outro disponível no momento do checkin.

Assim sendo conseguimos escrever nosso item de trabalho.

Acredito que com o que já foi apresentado anteriormente, você seja plenamente capaz de dar seus primeiros passos no mundo da escrita de itens de trabalho! Treine, escreva novas funcionalidades, pense em possíveis pontos de divergência de pensamento entre membros do time, questione, discuta! Tudo isso te fará ter uma visão de negócio melhor, e consequentemente melhorarão suas habilidades de escrita de itens!Continue lendo, o livro tem muitas outras abordagens na escrita de itens de trabalho, abordaremos melhor o critério de aceite, além de ajudá-los a refinar as demandas de maneira eficiente!