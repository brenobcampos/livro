# Como escrever um livro para a Casa do Código?

Para ser um bom escritor, você precisa começar sendo um bom leitor. Mais importante do que usar, integralmente e sem falhas, o sistema da Casa do Código para escrever o seu livro é escrever um bom livro! Leia estas poucas páginas com carinho.

O código fonte desse livro está no repositório `livro-base` no GitHub da Casa do Código. Utilize-o como referência:

http://github.com/casadocodigo/livro-base

## Defina muito bem seu público-alvo

Um dos pontos principais para o êxito do seu livro é conhecer o seu público-alvo. Você deve definir qual é o nível de conhecimento que ele possui. É feito para quem nunca ouviu falar da tecnologia? Ou para quem já está trabalhando com isso, mas não teve uma educação formal no assunto? Apenas para quem já conhece muito da tecnologia? Seja qual for, você deve respeitar esse perfil, lembrando-se disso durante todo o processo de escrita.

É claro que se o livro for voltado para alguém que esteja começando ou mesmo para alguém no nível intermediário, você pode, sim, adicionar alguns capítulos finais que sejam desafiadores, com assuntos mais específicos e aprofundados. Ou se seu livro é para um público mais avançado, também vale comentar aspectos básicos, como revisão, sempre que possível.

Em especial, saiba dizer se seu livro é para quem não conhece absolutamente nada da tecnologia, ou se é para alguém que começou a trabalhar com ela. Se for para quem já trabalha com ela, você pode ir um pouco mais rápido em alguns pontos.

## Mostre primeiro os problemas, depois as soluções, evitando definições

No começo de um capítulo ou de uma seção, é muito importante motivar o que será apresentado. Definições devem ser evitadas nesse começo. Um exemplo seria como apresentar o conceito de herança. Veja como ela é definida de forma enciclopédica na Wikipédia:

"_Inheritance is a way to reuse code of existing objects, or to establish a subtype from an existing object, or both, depending upon programming language support. In classical inheritance where objects are defined by classes, classes can inherit attributes and behavior from pre-existing classes called base classes, superclasses, parent classes or ancestor classes._"

Apesar de correto, o texto fica perdido, sem um guia, sem um porquê. Repare agora na descrição mais detalhada, que vai, ao final, mostrar a necessidade da herança:

_Como toda empresa, nosso Banco possui funcionários. Vamos modelar a classe `Funcionario`_:

``` java
  class Funcionario {
    String nome;
    String cpf;
    double salario;
     // métodos devem vir aqui
  }
```

_Além de um funcionário comum, há também outros cargos, como os gerentes. Os gerentes guardam a mesma
informação que um funcionário comum, mas possuem outras informações, além de ter funcionalidades um
pouco diferentes. Um gerente no nosso banco possui também uma senha numérica que permite o acesso ao
sistema interno do banco, além do número de funcionários que ele gerencia_

``` java
class Gerente {
  String nome;
  String cpf;
  double salario;
  int senha;
  int numeroDeFuncionariosGerenciados;
    
  public boolean autentica(int senha) {
    // ...
  }
}
```

_Se tivéssemos um outro tipo de funcionário que tem características diferentes do funcionário comum,
precisaríamos criar uma outra classe e copiar o código novamente!_

_Além disso, se um dia precisarmos adicionar uma nova informação para todos os funcionários,
precisaremos passar por todas as classes de funcionário e adicionar esse atributo.
O problema acontece novamente por não centralizarmos as informações principais do funcionário em um
único lugar!_

_Existe um jeito, em Java, de relacionarmos uma classe de tal maneira que uma delas **herda** tudo que
a outra tem. Isto é uma relação de classe mãe e classe filha. No nosso caso, gostaríamos de fazer com
que o `Gerente` tivesse tudo que um `Funcionario` tem, gostaríamos que ela fosse uma **extensão**
de `Funcionario`. Fazemos isto por meio da palavra-chave `extends`._

Conceitos precisam ser sempre apresentados de forma a motivar o leitor. Eles precisam aparecer só depois que um problema surgiu. Esse é o segredo de uma leitura fluída: primeiro, o problema; e, só depois, a solução. A definição pode sumarizar tudo isso, opcionalmente.

É claro que há exceções, em especial quando se for apresentar detalhes pequenos de uma API.

Essa técnica de mostrar primeiro o problema pode e deve também ser utilizada pensando na _big picture_. O capítulo de Introdução/Apresentação deve ser curto e interessante, desafiando o leitor com o tipo de problema que ele enfrentará e deverá resolver durante a leitura do livro. Imagens certamente auxiliam e empolgam. Abuse delas.

## Evite assustar as pessoas com códigos longos ou inesperados

Mesmo quando um código a ser apresentado é pequeno, não devemos jogá-lo na folha para depois explicá-lo. Repare neste exemplo:

_Vamos, então, acessar os serviços da Amazon S3. Crie uma classe `ConectorDoS3` com o seguinte código_:

``` java
class ConectorDoS3 {
  public static void main(String ... args) {
    // puxa as credenciais do arquivo AwsCredentials.properties
    InputStream credentials = ConectorDoS3.class.
        getResourceAsStream("AwsCredentials.properties");
    PropertiesCredentials awsCredentials = 
        new PropertiesCredentials(credentials);
    
    // cria objeto responsável por fazer conexao com o AWS
    AmazonS3 s3 = new AmazonS3Client(awsCredentials);
  }
}
```

Essa frase é pouco convidativa. Não explica o que o usuário deve esperar ou como deve proceder. O código é bastante assustador; explicá-lo através de comentários nunca é boa opção. Repare como fica melhor da seguinte forma:

_Vamos, então, acessar os serviços da Amazon S3. Para começar, certamente precisamos nos identificar de alguma forma. Para se conectar ao sistema, a API é simples: primeiro, vamos ler o conteúdo das nossas credenciais, que estão em `AwsCredentials.properties`, jogando essa informação dentro de uma classe específica do AWS, chamada `PropertiesCredentials`. Com essas informações, instanciamos uma classe que é capaz de se comunicar com o S3, a `AmazonS3Client`. Observe o código que realiza essas operações_.

``` java
InputStream credentials = ConectorDoS3.class.
    getResourceAsStream("AwsCredentials.properties");
PropertiesCredentials awsCredentials = 
    new PropertiesCredentials(credentials);
AmazonS3 s3 = new AmazonS3Client(awsCredentials);
```

O código agora está sem todo o peso da declaração da classe e do `main`, o que também facilita bastante. É claro que você deve pensar no contexto: se o livro é destinado a quem nunca viu Java na vida, é importante, sim, declarar a classe e o `main`. No caso de um livro mais avançado, você deve ter o perfil claro do seu público-alvo, para poder decidir quando deve ou não expor códigos inteiros ou apenas _snippets_. Por regra geral, quanto mais você conseguir quebrar o código e intercalá-lo com frases, melhor.

Isso é também válido pensando em uma imagem maior: o capítulo de abertura deve apresentar o desafio, o problema a ser resolvido durante a leitura do livro. Ele deve chamar atenção, abusar de imagens e motivar bastante.

## Foco e concisão

Quando for explicar um assunto, procure focar os exemplos e códigos apenas no tópico em questão. Seja conciso e evite adicionar exemplos mais complexos que tirem a atenção do leitor daquele pequeno ponto que é importante no momento.

Exemplo: se você estiver ensinando CSS e a difícil propriedade `clear`, não coloque um código como esse para exemplificar a explicação:

``` css
#topico {
  background: url(imagem.png) repeat-x;
  border-radius: 20px;
  color: #BADA55;
  clear: left;
  display: block;
  font-size: 300%;
  line-height: 1.5;
  text-align: center;
}
```

Certamente é um elemento muito bonito visualmente, com cores, fundos e até bordas redondas. Mas repare como o foco da seção, que era explicar `clear`, se perde com um código extenso, poluído com propriedades não importantes para o entendimento do assunto.

Seja conciso nos exemplos. Escreva o menor código possível que demonstre o que você precisa explicar naquele momento. Evite perder-se em coisas desnecessárias.

## Conclusão

Mostre primeiro o problema que você quer resolver.

Evite códigos grandes ou que apareçam para só depois serem explicados.

Uso do construtivismo. Você pode ir escrevendo um código que não funciona até chegar à versão funcional. Se isso ajudará a quebrar o processo em mais passos e fará com que o próprio leitor raciocine a respeito.

### Organize seu tempo para escrever o livro!

Não perca o ritmo e cobre **sempre** a revisão dos editores. Isso é fundamental no início do processo!

É preferível dispor de pouco do seu tempo, porém todos os dias, do que escrever em alguns _boosts_ de inspiração. Escrever regularmente é a melhor forma de criar um texto mais coeso e de terminar seu livro em menos tempo.
