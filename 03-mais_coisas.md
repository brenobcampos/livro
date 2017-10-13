# Mais detalhes da sintaxe do tubaina

## Trabalhando com itálico, negrito, sublinhado e código inline

Quando precisamos utilizar no meio de um texto algum conteúdo de código, citar o nome de um arquivo, nome de classe ou algo do tipo,
sem gerar uma quebra de linha para isso,  podemos utilizar \`codigo aqui\` (dois \`).

Como exemplos teríamos: A tag html deve ser sempre fechada (como em `<html></html>`). Não esqueça de salvar esse arquivo como `hibernate.cfg.xml`. Através do método `adicionaCategoria`, podemos ver que a classe `ControladorSeguro` está como pretendíamos.

Esse texto terá fonte `monoespaçada`. **Não use aspas para se referir a variáveis, classes, arquivos**. É para isto que existe o \`. Aliás, evite aspas ao máximo.

Quando quiser que um texto apareça em itálico, basta adicioná-lo entre \_conteúdo aqui\_ ou entre \*conteúdo aqui\* (underlines ou asteriscos), dessa forma, o _texto ficará assim_. O itálico pode ser usado para termos em inglês que apareçam raramente no seu livro. Se for um termo que aparece com frequência, pode utilizá-lo sem destaque algum (ou então traduzi-lo a primeira vez entre parenteses). O acesso ao menu e mensagens de erro/caixas também aparecem em itálico: "Agora acesse o menu _Window -> Console -> Show log_", por exemplo.

Para fazer com que um trecho do texto fique em negrito, coloque-o entre \_ \_conteúdo aqui\_ \_ ou \*\*conteúdo aqui\*\* (dois underlines seguidos ou dois asteriscos seguidos), com isso, **o texto ficará em assim**. Utilize o negrito para destacar um trecho extremamente importante, uma definição curta, um conselho fundamental. **Cuidado para não abusar**, em especial do negrito, que não deixa a leitura fluir tanto, como você pode ver aqui.

Vale ressaltar que em algumas linguagens como `C`, `C++` e `Python` símbolos como '*', '_' e ':' são frequentemente utilizados. Por isso, quando colocados dentro de \`\` eles serão interpretados literalmente, e seu código deve ficar algo como `char **nomes`, ou então `__init__.py`.

## Ilustre seu livro com bastante código

Antes de tudo, lembre-se das recomendações já dadas: mantenha o código curto (snippets sucintos) e sempre dê motivação para aquele código aparecer **antes** de ele aparecer. Códigos com mais de 15-20 linhas devem ser raros. Se for necessário algo mais extenso, quebre em pedaços e evite  detalhes desnecessários. Você pode deixar o código completo do arquivo em um gist (https://gist.github.com/) e linkar para ele. Se o público for mais avançado, você pode até omitir os trechos mais óbvios.

Também evite a notação húngara (usar `ps` para PreparedStatement em vez de `statement` ou algo mais significativo ainda). Sobre os exemplos, torne-os reais. Evite classes como `MinhaClasse`, `MeuModelo` etc. Mesmo que esteja explicando detalhes de sintaxe, procure trazer o exemplo para o cotidiano do leitor. **Exemplos palpáveis, curtos e bem nomeados são sempre melhores**.

Lembre-se: o leitor está comprando um livro no Brasil e existe uma chance enorme de seu inglês ser fraco ou nenhum. Utilize nomes de variáveis, métodos, funções, classes e projetos todos em português. Pode ser contra a sua convenção de código, mas esse é um ponto importante. Pode parecer fácil para você apenas algumas palavras em inglês, mas isso torna a leitura muito difícil para quem não conhece a língua, que é a esmagadora maioria dos leitores.

É possível escrever código em diversas linguagens e fazer com que eles tenham syntax highlight adequado. Para isso, basta usar \`\`\` especificando uma linguagem. Exemplo:

```
``` java
double preco;
System.out.println("oi");
``````

E isso gerará o seguinte conteúdo:

``` java
    double preco;
    System.out.println("oi");
```

Para a indentação do código, será utilizada a mesma que for colocada dentro do  \`\`\`. Para garantir que o espaçamento sairá bem, utilize TABs em vez de espaço para a indentação.

Para uma lista das linguagens disponíveis, veja: https://highlightjs.org/static/demo/

Se necessário, é possível utilizar um trecho de código sem formatação alguma. Para isso, basta omitir a  linguagem. É usado, para o caso da saída de um log, do console ou um arquivo `.properties`, por exemplo.

Evite utilizar comentários dentro do código para explicá-lo. Também não é atraente explicitar linhas, como por exemplo "Na segunda linha fazemos com que a mensagem _oi_ seja impressa", é melhor e mais didático escrever que "E então invocamos `System.out.println("oi")` para imprimir _oi_", pois faz o leitor fixar os nomes de funções, classes, métodos e evita que ele fique indo e vindo no texto.

Evite se referir ao código como: "... no código abaixo ... " ou "... no código acima ...". Como a diagramação é automática, a listagem de código pode acabar em outra página e isso não será verdade. **Use referências mais genéricas**, como: "... no código anterior ..." ou "... no código seguinte/adiante".

**Cuidado, pois existe um limite de caracteres em uma linha para o código do livro.** No caso dos livros, esse limite
e de 73 caracteres, para se encaixar bem na página. O autor deve quebrar o código onde
achar mais conveniente. Durante a revisão final, os editores verificarão se não há nenhuma linha de código estourando
a página.

## Compartilhe os exemplos no Github

Os leitores gostam muito quando o livro acompanha um download. Para simplificar esse processo, o recomendado é que você utilize um repositório público no seu github para guardar a sua aplicação de exemplo (ou suas pequenas aplicações). Caso prefira e se adeque, pode usar o gist em vez do github.

Você pode linkar para esse repositório logo no início do seu livro, avisando que os exemplos estarão completos por lá. A aplicação dentro do repositório não precisa ser exatamente igual à que você está criando no livro, possibilitando que você apare arestas, utilize um design mais arrojado, inclua imagens etc.

## Crie um canal com seus (futuros) leitores: listas, fórum e site dedicado

Temos um Fórum da Casa do Código, ao qual convidamos autores e leitores para compartilharem experiências sobre seu livro. Isso é opcional, mas indicamos fortemente que o autor lá se cadastre e participe ativamente para receber o feedback dos leitores, bem como ajudá-los a entender alguma dúvida específica. Deixe um link para esta lista de discussão logo no começo do seu livro, junto com o link para o repositório de exemplos. Algo como:

Você pode trocar ideias sobre este livro, compartilhar suas experiências e tirar dúvidas no nosso Fórum: http://forum.casadocodigo.com.br

Uma estratégia excelente de divulgação do seu livro é participar fortemente das listas de discussão e de fóruns (GUJ.com.br) relacionados à tecnologia que você está escrevendo. Comece a participar antes mesmo do lançamento do seu beta. Lembre-se de linkar sua assinatura para o livro e responder questões relacionadas. É bem impressionante o resultado que isso pode ter nas vendas. Se tiver um blog seu que está meio parado, esta é a melhor hora para voltar a atualizá-lo!

Há também a possibilidade de fazer um hotsite simples, como estes, que já são até responsivos e ficam muito bem em mobile:

http://tddnomundoreal.com.br/

http://www.arquiteturajava.com.br/

Para isso, faça clone do repositório do site. O sistema de comentários no facebook não é necessário. Usando o heroku pode-se hospedar um site como esse gratuitamente.

https://github.com/caelum/arquiteturajava.com.br
https://github.com/mauricioaniche/tddnomundoreal.com.br

## Organize informações com listas
Se deseja enumerar itens, pode-se utilizar uma lista numerada. Cada item da lista deve ser identificado com um número seguido por um ponto e de um espaço:


1. Primeiro item;
1. Segundo item;
1. Terceiro item;

Na verdade, pode ser colocado qualquer número. Não há necessidade de colocar `1. `, depois `2. `, etc... Recomendamos que você simplesmente coloque `1. ` na frente de cada item da lista.

### Insirir imagens, box ou lista dentro de lista

Se você inserir uma imagem ou um box no meio de uma lista numérica, ele reiniciará a enumeração a partir do número 1. Para dar prosseguimento à enumeração, a imagem ou box dentro daquele item da lista deve estar indentado com um tab. Exemplo:

1. Primeiro item;
    ![Imagem recortada onde as bordas estão sujas {w=40%}](imagens/borda_ruim.png)
1. Segundo item;
    > box exemplo
    
1. Terceiro item;

Caso não deseja uma lista ordenada, ou seja, sua lista terá apenas os bullets, coloque `* ` (um asterisco seguido de um espaço) no início da linha:


* Bullet 1
* Bullet 2
* Bullet 3

Além de `*`, é possível definir uma lista não ordenada com `-` ou  `+` como primeiro caractere.


Nos casos anteriores, tivemos o seguinte código:

```
    
      1. Primeiro item;
      1. Segundo item;
      1. Terceiro item;

      * Bullet 1
      * Bullet 2
      * Bullet 3
    
```

Para mais detalhes, consulte a documentação do Markdown:
http://daringfireball.net/projects/markdown/syntax#list

**Cuidado** para não utilizar listas para elencar conteúdos muito longos. Um sintoma de que isso está acontecendo é quando  o item da sua lista fica com mais de 3 ou 4 linhas de texto. Nesse caso, talvez seja mais indicado o uso de um `###`.

Mesmo para listas curtas, muitas vezes é interessante enumerar dentro do próprio parágrafo, deixando o texto mais agradável. Repare que dá para fazer essa troca e utilizar o negrito se for necessário chamar atenção:

Temos três itens importantes para um design responsivo:


* Layout fluído
* Imagens flexíveis
* Media Queries


ou...

Temos três itens importantes para um design responsivo: o **layout fluído**, as **imagens flexíveis** e as **media queries**.

Evite enumerações quando possível.

## Insira tabelas

Para inserir uma tabela, use:

```
|Nome | Idade | Profissão |
|-----|-------|-----------|
|Bianca| 18| Revisora|
|Vivian| 27| Editora|
|Adriano| 41| CEO|
```

Graficamente, fica assim:

|Nome | Idade | Profissão |
|-----|-------|-----------|
|Bianca| 12| Revisora|
|Vivian| 27| Editora|
|Adriano| 41| CEO|
