# Livro: Gestão de Escopo em Projetos Ágeis

Este projeto é a escrita do livro de Gestão de Escopo em Projetos Ágeis por Breno e Alfred.

## Como contribuir?

Se compartilhamos com você, acreditamos que pode nos ajudar revisando nossos PR's e nos dando dicas do que podemos adicionar a este livro para que seja relevante a comunidade como um todo.

## Para os autores

### Como trabalhar no GIT (eu, Breno, sempre esqueço)

Baixando o repositório para máquina (uma vez apenas)

```
git clone https://github.com/luiz-bernardo/livro-gestao-escopo.git
```

### Criando sua branch

Para que consigamos trabalhar cada um em um capítulo, e que as revisões ocorram em separado, vamos escrever os capítulos em branches.

```
git checkout -b nome-da-branch
```

Criaremos a branch no padrão sigla-"o que estamos escrevendo", por exemplo `bbv-intro-user-stories`.

### Criando os commits

Após escrever o capítulo, ou mesmo em WIP podemos enviá-lo para o repositório. Para isso, vamos adicionar as alterações que fizemos em nossa máquina.

```
git add .
```

Agora faremos o commit:

```
git commit -m "Mensagem do commit"
```

A mensagem do commit pode ser simples, indicando o que adicionamos no capítulo. Podemos também já adicionar o que pretendemos abordar para próximas passos.

### Enviando para a branch remota

Para enviarmos para o github para revisão, precisamos enviar para a branch remota, para isso o comando:

```
git push origin nome-da-branch
```

### Excluindo uma branch local finalizada

Vá para a master

```
git checkout master
```

E delete a branch desejada

```
git branch -D nome-da-branch
```
