## Célula de estudos UFC Quixadá: Aprendendo Programação Com App Inventor
<div align="justify">

## 1. Motivação 

***Dica:*** Abra os links deste README em uma nova aba do seu navegador, para você não se perder na leitura :wink:.

<ul>
  <li>

  [Vídeo da célula de estudos relecionado a este tópico](https://youtu.be/-k7NKoM7ScA)
  </li>
</ul>

Saudações pessoal, quero começar apresentando um pouco sobre o ministrante desta célula: eu sou aluno quase concludente de Engenharia de Software (ES) aqui do Campus UFC Quixadá. Durante minha graduação fui me inclinando mais a gostar das disciplinas de programação, desde Fundamentos de Programação (FUP) - Graças ao professor David Sena. Com o passar dos semestres, mais especificamente no 8º em diante, quando cursei as disciplinas de Desenvolvimento Web e Dispositivos Móveis, criei ainda mais gosto pela nossa área. Dito isso, quero fazer o seguinte questionamento juntamente com vocês aqui e agora: **Porquê meu gosto aumentou pela área depois que fiz estas duas disciplinas?** 

Acho que vocês já entenderam onde quero chegar, meu ponto é, muitas das vezes nós (os estudantes) precisamos esperar bastante para pormos em prática o que aprendemos dos nossos estudos de computação. Principalmente quando se trata de criar aplicações com interfaces gráficas e feedback visual. Logicamente, a universidade tem seus motivos para isto, tendo que ensinar os conceitos fundamentais de computação e também conteúdos mais voltados a especificidade do respectivo curso antes de dar início a estes determinados conteúdos que envolvem interfaces gráficas, que na maioria das vezes são mais atraentes e estimulantes para os alunos.

Portanto, esta célula tem por objetivo principal ensinar alguns **conceitos de FUP, usando uma ferramenta de criação de aplicativos móveis, por programação por blocos, que será a [MIT App Inventor](https://appinventor.mit.edu/).** A programação por blocos resume muitas das coisas das quais se é preciso dominar se comparada a programação comum (codificada). Então, aproveitando as funcionalidades que o App Inventor nos fornece, podemos focar mais na parte lógica dos algoritmos de programação em si. Assim (eu espero) poder contribuir com o aprendizado de vocês, e além do mais, também lhes causar estímulo na contínua jornada que é ser um profissional da área de TI, mostrando a possibilidade de coisas que já é possível serem criadas com uma ferramenta de programação por blocos de fácil acesso. 

### 1.1 Exemplos de aplicativos 

O App Inventor possui uma página de [Galeria de Aplicativos](https://gallery.appinventor.mit.edu), que funciona de maneira parecida com uma *Play Store* da vida. Depois de finalizado o projeto de um aplicativo, o usuário autor pode publica-lo na galeria, onde lá ele ficará disponível para que outros usuários possam baixar, executar, e, por ventura, modificar a sua respectiva cópia, de modo independente do aplicativo publicado originalmente. Sendo também, uma plataforma de código aberto, se caracterizando pelo compartilhamento de conhecimento e aprendizado mútuo.

**Nota:** Para que os filtros de exibição da galaria funcionem corretamente, efetue primeiro o login na plataforma:

<ol>
  <li>
  
  [Acesse a plataforma App Inventor](https://appinventor.mit.edu/)
  </li>
  <li>
  
  Siga as instruções das imagem abaixo

  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/1.png?raw=true)
  ***
  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/2.png?raw=true)
</ol>

## 2. Variáveis

<ul>
  <li>

  [Vídeo da célula de estudos relecionado a este tópico](https://youtu.be/_D0Tp0LuU9E)
  </li>
</ul>

Se tratando de um conceito inicial em programação, porém fundamentalmente importante, as variáveis são espaços de memória que servem para armazenar dados durante a execução de um programa. Estas que, **no App Inventor, podem ser basicamente de dois tipos: Números; e Texto**. Dito isso, podemos já interpretar que devem existir tratamentos de erros com operações utilizando variáveis. Pois, imagine o cenário que o usuário quer somar dois valores que estão em variáveis lidas de dados fornecidos pelo usuário, porém um dos valores é um número e o outro é um texto, sendo assim o App Inventor irá gerar um erro, e nós, os programadores devemos tratar tal problema, de modo a restringir as operações do nosso programa durante o tempo de execução. 

### 2.1 Tipagem

No App Inventor a tipagem de variáveis não é fixa, "como assim?", se inicializarmos uma variável com o número 1, e depois setarmos ela com o texto "eae", isto não irá lançar nenhum erro. 

Logo, precisamos de alguma funcionalidade que nos permita testar se o valor de uma determinada variável é número, por exemplo. Para isto, existe um bloco do tipo "Matemático" (cor azul) que faz exatamente esta verificação. 

### 2.2 Escopo

O conceito de escopo de variável pode ser novo para vocês, essencialmente ele está muito relacionado ao conceito de função que é tratado no próximo módulo. Porém, é importante ser citado aqui como uma característica de uma variável. 

Podemos pensar no escopo de uma variável como um sinal WIFI por exemplo, se a variável v1 tem o escopo da WIFI w1, ela só é acessível dentro da área de cobertura de w1. Ou seja, se alguém estiver dentro da zona de cobertura da WIFI w2, que fica fora de alcance da w1, e quiser acessar v1, não conseguirá. v1 neste caso pode ser definida como **variável local.**

Referindo-se a escopo, no App Inventor existem estes dois tipo: escopo local, e global. Diferentemente do escopo local, **variáveis definidas com escopo global** podem ser acessadas de qualquer "ponto dentro de qualquer cobertura WIFI" (ler parágrafo anterior) no programa. Seguindo o exemplo da WIFI, é como se a variável global fosse de fato publicada na internet, e não apenas na rede LAN.

E um escopo dentro de um escopo? É perfeitamente normal, porém devemos ressaltar que, digamos uma variável v1 está no escopo de fora, se o programador desejar usar a variável v1 dentro do escopo de dentro não tem problema, entretanto, o contrário (acessar v1 no escopo de fora se ela tiver sido criada no escopo de dentro) resultará em um erro.

### 2.3 Nomenclatura

Parece bobo, mas é importante que os nomes das variáveis sejam correspondentes as suas respectivas funções dentro do aplicativo. Acreditem, é bem mais fácil entender um código de variáveis com nomes do tipo "valorDeEntrada" ou "tokenDeAcesso", do que "v" ou "t". 

Aqui no curso, os nomes das variáveis podem se confundir com os nomes dos componentes de interface de usuário. Portanto, quero deixar logo claro esta divergência: Uma caixa de texto por exemplo, é o componente que é renderizado na tela do celular, podendo ter o nome "caixaDeTextoEsquerda". Já uma variável que eventualmente guarda e faz operações com o conteúdo deste componente é outra coisa, podendo ter o nome "stringEsquerda". 

### 2.4 Blocos & Documentação

No link abaixo vocês encontrarão a documentação completa dos blocos referentes a variáveis no App Inventor.

http://ai2.appinventor.mit.edu/reference/blocks/variables.html

### 2.5 Exercícios

<ol>
  <li>
    Crie um aplicativo que lê do usuário dois valores, salvando cada valor em uma variável. Depois junte os valores e salve em uma terceira variável, em seguida, mostre-a na tela como resultado da junção. 
  </li>

  <li>
    Faça a mesma coisa da questão anterior, porém, restrinja os valores a serem apenas números. E ao contrário de juntar os valores, faça botões para mostrar as quatro operações matemáticas entre os dois valores das variáveis lidas. Desconsidere o erro de divisão por 0.
  </li>

  <li>
    Qual o valor da variável pai ao final da execução dos blocos abaixo?
  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/q1.1.png?raw=true)
  <li>
    Qual o valor da variável filho ao final da execução dos blocos abaixo? A execução gera algum erro semântico? Se sim, qual? (Leia: <a href="https://www.devmedia.com.br/forum/o-que-difere-um-erro-sintatico-de-um-erro-semantico/571029">Diferença entre erro semântico e sintático</a>)
  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/q1.2.png?raw=true)
  <li>
    Qual o valor da variável total ao final da execução dos blocos abaixo? A execução gera algum erro? Se sim, qual?
  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/q1.3.png?raw=true)
</ol>

## 3. Funções

<ul>
  <li>

  Vídeo(s) da célula de estudos relecionado a este tópico: [1 - parte 1/2](https://youtu.be/GkBEQ6v8hfM) | [1 - parte 2/2](https://youtu.be/zpb7-K_nz00)
  </li>
</ul>

Durante o processo de construção de um código, o programador irá se deparar com situações onde uma determinada tarefa deverá ser executada diversas vezes, esta que, pode ou não receber parâmetros de entrada que serão utilizados para a geração do seu resultado. Devendo terminar sua execução retornando um valor para o escopo no qual foi chamada, ou apenas realizar uma ação de modo independente, sem retorno de valor, mas com alguma mudança no contexto do programa. Isto, por sua vez, é uma definição de uma função computacional. 

Com o App Inventor em português do Brasil, os blocos referentes a funções são retratados como blocos do tipo "procedimento". Os quais podem ser dos dois tipos relatados no parágrafo anterior, sendo procedimentos com retorno, e sem retorno, podendo qualquer um dos dois possuir parâmetros de entrada ou não. 

O conceito de função pode ser muito abrangente, contudo, foi considerado aqui o que está diretamente ligado ao App Inventor. A documentação destes blocos se encontra no link a seguir.

http://ai2.appinventor.mit.edu/reference/blocks/procedures.html

Na sequência de imagens a seguir é mostrado o processo de utilização de uma função na plataforma.

<ol>
  <li>
    Primeiro selecione o bloco do procedimento que deseja usar, se é do tipo com, ou sem retorno. Neste caso, o bloco escolhido precisa de retorno.
  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/102.png?raw=true)
  <li>
    Caso precise usar parâmetros, clique na engrenagem e arraste os blocos de entrada para a parte direita do popup.
  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/104.png?raw=true)
  <li>
    Perceba que agora o bloco da função criada, está disponível para ser usado nos blocos do tipo procedimentos.
  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/105.png?raw=true)
  <li>
    Por fim, veja como seria o uso desta função:
  </li>

  ![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/106.png?raw=true)
</ol>

### 3.1 Exercício de Pensamento

Imagine a situação onde um gerente de um depósito de construção precisa, todo mês, pelo menos uma vez, calcular qual será a quantidade de cada produto que será necessária a realização de uma compra mensal, com a finalidade de reposição de estoque. Ok, sendo que o gerente sabe que no seu depósito existem cinquenta tipos diferentes de produtos. Suponha que para escrever um algoritmo, um programador opte por percorrer a lista de tipos de produtos, e para cada tipo, retornando a quantidade de compras para reposição, levando em consideração o critério de reposição somente se existir 10 ou menos produtos do mesmo tipo. 

Como você acha que deve ser feito este algoritmo? Elabore um algoritmo em programação por blocos que em teoria realiza o que o gerente precisa (somente a ideia, não precisa executar).

## 4. Seleção

<ul>
  <li>

  [Vídeo da célula de estudos relecionado a este tópico](https://youtu.be/BcXmbjZ11uo)
  </li>
</ul>

O computador nada mais faz além do que ele foi programado para fazer. Ou seja, por vezes encaramos problemas ao desenvolver algum tipo de algoritmo e acabamos nos estressando bastante. Mas, é importante manter a calma nestes momentos, lembrar que o computador não possui "vida própria", e então procurar entender o problema para em fim consertá-lo.

Não obstante a isto, o ato de estudar, aprender, e masterizar lógica de programação pode prevenir o acontecimento erros durante a produção de um algoritmo. Por isso é tão importante os estudantes de Ciência da Computação focarem em tais habilidades. A base da lógica computacional pode ser a grosso modo definida pela frase "se isso, então aquilo". Este, é o conteúdo abordado nesta seção.

Já dizia um professor meu de graduação da disciplina de Fundamentos de Programação (David Sena): "programação é como uma luta de UFC, você não aprende assistindo os outros lutando, e sim praticando luta". É importante que todos os adeptos a ingressar em programação tenham isso em mente. 

No App Inventor, os blocos de seleção são chamados de tipo "Controle". São eles:

![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/108.png?raw=true)

Perceba que existem três variações principais, e uma quarta com o bloco sendo de retorno, podendo receber uma expressão lógica, onde se ela for satisfeita, o bloco retorna o que estiver no encaixe "então", caso contrário o bloco retorna o que estiver no encaixe "senão".

A imagem abaixo mostra como é o fluxo de execução de um bloco simples de seleção. As linhas <span style="color:green">verdes</span> representam os caminhos que o algoritmo irá seguir caso as expressões de encaixe "se" forem satisfeitas. e os caminhos <span style="color:red">vermelhos</span> representam o fluxo de execução caso as duas expressões não forem satisfeitas. 

![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/109.png?raw=true)

Ao fazermos uma análise semântica sobre este bloco, percebemos que não há a possibilidade do fluxo de execução entrar dentro do "primeiro se" e também do "segundo se" durante uma mesma execução. Pois ao entrar dentro do primeiro, o fluxo acaba, sem mesmo testar a expressão do "segundo se". Além disso, também podemos notar que o que está no "ultimo se não" só será executado se as duas expressões anteriores não forem satisfeitas, ou seja, além de ser a negação do "segundo se", é como se ele também fosse um "se não" do "primeiro se". 

Por fim, podemos concluir que cada uma das três execuções que irão nos encaixes "então/senão", são exclusivas, em relação as outras duas. Um exemplo interessante que podemos pensar para facilitar o entendimento é: Imagine um cenário onde queremos testar se Bergson já passou da metade da campanha do jogo Hogwarts Legacy, o pseudocódigo ficaria 

se Bergson zerou Hogwarts Legacy, faça:<br/>&emsp;resultado = sim<br/>se não, se Bergson está entre a metade e o fim da campanha de Hogwarts Legacy, faça:<br/>&emsp;resultado =  sim<br/>se não, faça:<br/>&emsp;resultado =  não

Manipular corretamente este fluxo de execução, é uma habilidade que um bom programador precisa possuir.

### 4.1 Exercícios

Nesta seção, por se tratar de um conteúdo que requer bastante prática, vamos optar por usar exercícios de do curso [FUP is FUN](https://moodle2.quixada.ufc.br/course/view.php?id=3), disponibilizado no moodle do campus UFC Quixadá, voltado para o uso dos alunos também deste campus.

Como as questões do Fup Is Fun são feitas para serem respondidas em linguagens de programação codificadas, teremos que fazer uma adaptação para o ambiente de programação por blocos do App Inventor. Onde na grande maioria das questões, basta que utilizemos alguns poucos componentes de interface visual, sendo eles CaixaDeTexto, Legenda, e Botão. Com isso, já podemos ilustrar e testar o funcionamento correto das questões. 

Para os interessados por este curso que não são alunos do campus UFC Quixadá, vocês podem acessar as questões relacionadas ao conteúdo de seleção através [deste link](https://github.com/senapk/arcade/blob/master/lista_compiladas/01_operacoes_selecao/questoes.cpp) do GitHub do professor David Sena.

## 5. Repetição

<ul>
  <li>

  Vídeo(s) da célula de estudos relecionado a este tópico: [1](https://youtu.be/BcXmbjZ11uo) | [2 - parte 1/2](https://youtu.be/y8OFsMXRAUI) | [2 - parte 2/2](https://youtu.be/zrRGpF-_McY)
  </li>
</ul>

Quando chegamos em Repetição (laço), é provavelmente um momento de virada de página interessante no que diz respeito a evolução do nosso pensamento computacional. Podemos descrever o processo inicial de aprendizagem de programação separando-o em algumas partes principais: 
<ol>
<li>
Como o computador executa uma tarefa: Ai entendemos o que é um algoritmo.
</li>
<li>
Armazenamento e manipulação de dados durante tais tarefas: Variáveis.
</li>
<li>
Execuções de tarefas de maneira separada, que, por fim sejam integradas em uma execução (algoritmo) principal, também resultado em reaproveitamento de código: Uso de funções.
</li>
<li>
Agora, quero lhes fazer um questionamento, o que torna o computador mais eficaz que um ser humano na realização de um tarefa? O que ele tem de especial que nos faz cada dia mais avançar nas pesquisas da área de computação? Sobre isso, acredito que tal fato aconteça por duas razões:
</li>
<ul>
<li>
Repetição: O computador não "enjoa" ou "cansa" de fazer determinada tarefa várias vezes repetidamente, como contar de 1 a 1000, ou procurar números que sejam múltiplos de uma valor recebido como entrada, por exemplo. Ele simplesmente faz o que foi programado para fazer, sem fazer questionamentos ou análise sobre tal comportamento (por enquanto, desconsidere Inteligência Artificial). Já pessoas, bom, vocês sabem como pessoas são...
</li>
<li>
Programável: Isto é o que torna também o computador especial, ele não só faz uma quantidade 'x' de tarefas, mas pode ser programado para realizar infinitas tarefas de formas diferentes. 
</li>
</ul>
</ol>

Agora que já fiz vocês pensarem um pouco, vamos entrar de fato nos conceitos de repetição, vou explicar do ponto de vista de programação por blocos via App Inventor, mas o entendimento serve para programação codificada também.

### 5.1 Estado inicial, ciclo de cada repetição, e estado final

Ao se encontrar com uma situação onde se é preciso o uso de repetição, primeiro, tente pensar no "estado inicial" que o seu algoritmo deve estar para que o laço comece a executar. Após isto, analise o que deverá ser feito durante cada ciclo de execução dentro do seu programa, de modo que um ciclo, geralmente está diretamente ligado ao seus ciclos anteriores o posteriores, ou seja, tudo acontece de modo interligado, você deve pensar tanto separadamente, quando na integração da execução como um todo. Por fim, veja qual será sua condição de parada para que o laço de repetições acabe, ou seja, antes de ser executado o que está dentro do laço, esta expressão lógica será calculada, se ela for verdadeira significa que você conseguiu obter o resultado que procurava e já não precisa mais de repetições. Logicamente que este processo sem sempre acontece desta forma, ou nesta sequência. 

O processo de criação de um algoritmo e sua programação é livre, não se prenda a pensar de um determinado modo na hora de programar. Apenas faça do jeito que você conseguir, mas não esqueça de atribuir uma boa legibilidade ao seu algoritmo, pois vai facilitar tanto para você precisar entender seu código (por blocos também) no futuro, quanto para o caso de outro programador precisar entender sua "obra prima".

Os blocos essenciais do tipo de Repetição que fazem parte do App Inventor são estes:

![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/5.1.png?raw=true)

O bloco acima é o de repetição mais simples, ele pode ser descrito como um bloco equivalente ao comando `while` em uma linguagem codificada.

![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/5.2.png?raw=true)

Já este segundo bloco, é mais parecido com o comando `for`. Porém, uma ressalva importante, o bloco que encaixa em "passo" dá a entender que representa "contador mais 1, ou i++", errado! Ele apenas representa o valor dos saltos entre o valor do bloco encaixado em "deste", até o valor do bloco encaixado em "até" ("deste" e "até" inclusos). Caso você altere o valor de "número" ao final de um ciclo, no próximo ciclo, o valor da variável "número" não conterá tal alteração, é como se os valores de "número" fossem fixos de "deste" - "até", com o espaço "passo" entre cada valor de "número". 

### 5.2 Exemplos 

Pense e responda só para você, para o que os seguintes trechos de blocos servem:

<ol>
  <li>
  </li>

![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/5.3.png?raw=true)
  <li>
  </li>
 
![](https://github.com/robertsonasc/AprendendoProgramacaoComAppInventor/blob/master/imagens/5.4.png?raw=true)
</ol>

### 5.3 Exercícios

Assim como na sessão anterior, para os que possuem acesso ao Moodle UFC Quixadá, vou recomendar vocês estudarem laço fazendo questões do curso [FUP is FUN](https://moodle2.quixada.ufc.br/course/view.php?id=3). Já para os que não possuem acesso ao Moodle, acessem [este link](https://github.com/senapk/arcade/blob/master/lista_compiladas/05_laco_math/questoes.cpp) do GitHub do professor David Sena, lá tem várias questões legais que envolvem repetição. 

Lembrando que todas estas questões foram elaboradas para serem resolvidas por programação comum (codificada), porém, elas podem ser resolvidas por programação por blocos, bastando ser criado um pequeno aplicativo com componentes que recebem as entradas das questões, um campo para mostrar o resultado, e um botão para disparar o evento de execução do algoritmo que você irá criar - coisa que a essa altura, não deve ser difícil para vocês fazerem. Quero dizer, foquem na parte lógica da programação por blocos, não precisa enfeitar demais a interface gráfica dos aplicativos. 

Bons estudos e até o nosso último e não menos importante assunto, listas!

</div>