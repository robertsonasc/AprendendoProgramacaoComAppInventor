## Célula de estudos UFC Quixadá: Aprendendo Programação Com App Inventor
<div align="justify">

### 1. Motivação 

Saudações pessoal, quero começar apresentando um pouco sobre o ministrante desta célula: eu sou aluno quase concludente de Engenharia de Software (ES) aqui do Campus UFC Quixadá. Durante minha graduação fui me inclinando mais a gostar das disciplinas de programação, desde Fundamentos de Programação (FUP) - Graças ao professor David Sena. Com o passar dos semestres, mais especificamente no 8º em diante, quando cursei as disciplinas de Desenvolvimento Web e Dispositivos Móveis, criei ainda mais gosto pela nossa área. Dito isso, quero fazer o seguinte questionamento juntamente com vocês aqui e agora: **Porquê meu gosto aumentou pela área depois que fiz estas duas disciplinas?** 

Acho que vocês já entenderam onde quero chegar, meu ponto é, muitas das vezes nós (os estudantes) precisamos esperar bastante para pormos em prática o que aprendemos dos nossos estudos de computação. Principalmente quando se trata de criar aplicações com interfaces gráficas e feedback visual. Logicamente, a universidade tem seus motivos para isto, tendo que ensinar os conceitos fundamentais de computação e também conteúdos mais voltados a especificidade do respectivo curso antes de dar início a estes determinados conteúdos que envolvem interfaces gráficas, que na maioria das vezes são mais atraentes e estimulantes para os alunos.

Portanto, esta célula tem por objetivo principal ensinar alguns **conceitos de FUP, usando uma ferramenta de criação de aplicativos móveis, por programação por blocos, que será a [MIT App Inventor](https://appinventor.mit.edu/).** A programação por blocos resume muitas das coisas das quais se é preciso dominar se comparada a programação comum (codificada). Então, aproveitando as funcionalidades que o App Inventor nos fornece, podemos focar mais na parte lógica dos algoritmos de programação em si. Assim (eu espero) poder contribuir com o aprendizado de vocês, e além do mais, também lhes causar estímulo na contínua jornada que é ser um profissional da área de TI, mostrando a possibilidade de coisas que já é possível serem criadas com uma ferramenta de programação por blocos de fácil acesso. 

#### 1.1 Exemplos de aplicativos 

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

### 2. Variáveis

Se tratando de um conceito inicial em programação, porém fundamentalmente importante, as variáveis são espaços de memória que servem para armazenar dados durante a execução de um programa. Estas que, **no App Inventor, podem ser basicamente de dois tipos: Números; e Texto**. Dito isso, podemos já interpretar que devem existir tratamentos de erros com operações utilizando variáveis. Pois, imagine o cenário que o usuário quer somar dois valores que estão em variáveis lidas de dados fornecidos pelo usuário, porém um dos valores é um número e o outro é um texto, sendo assim o App Inventor irá gerar um erro, e nós, os programadores devemos tratar tal problema, de modo a restringir as operações do nosso programa durante o tempo de execução. 

#### 2.1 Tipagem

No App Inventor a tipagem de variáveis não é fixa, "como assim?", se inicializarmos uma variável com o número 1, e depois setarmos ela com o texto "eae", isto não irá lançar nenhum erro. 

Logo, precisamos de alguma funcionalidade que nos permita testar se o valor de uma determinada variável é número, por exemplo. Para isto, existe um bloco do tipo "Matemático" (cor azul) que faz exatamente esta verificação. 

#### 2.2 Escopo

O conceito de escopo de variável pode ser novo para vocês, essencialmente ele está muito relacionado ao conceito de função que é tratado no próximo módulo. Porém, é importante ser citado aqui como uma caracteristica de uma variável. 

Podemos pensar no escopo de uma variável como um sinal WIFI por exemplo, se a variável v1 tem o escopo da WIFI w1, ela só é acessível dentro da área de cobertura de w1. Ou seja, se alguém estiver dentro da zona de cobertura da WIFI w2, que fica fora de alcance da w1, e quiser acessar v1, não conseguirá. v1 neste caso pode ser definida como **variável local.**

Referindo-se a escopo, no App Inventor existem estes dois tipo: escopo local, e global. Diferentemente do escopo local, **variáveis definidas com escopo global** podem ser ecessadas de qualquer "ponto dentro de qualquer cobertura WIFI" (ler parágrafo anterior) no programa. Seguindo o exemplo da WIFI, é como se a variável global fosse de fato publicada na internet, e não apenas na rede LAN.

E um escopo dentro de um escopo? É perfeitamente normal, porém devemos ressaltar que, digamos uma variável v1 está no escopo de fora, se o programador desejar usar a variável v1 dentro do escopo de dentro não tem problema, entretanto, o contrário (acessar v1 no escopo de fora se ela tiver sido criada no escopo de dentro) resultará em um erro.

#### 2.3 Nomenclatura

Parece bobo, mas é importante que os nomes das variáveis sejam correspondentes as suas respectivas funções dentro do aplicativo. Acreditem, é bem mais fácil entender um código de variáveis com nomes do tipo "valorDeEntrada" ou "tokenDeAcesso", do que "v" ou "t". 

Aqui no curso, os nomes das variáveis podem se confundir com os nomes dos componentes de interface de usuário. Portanto, quero deixar logo claro esta divergência: Uma caixa de texto por exemplo, é o componente que é renderizado na tela do celular, podendo ter o nome "caixaDeTextoEsquerda". Já uma variável que eventualmente guarda e faz operações com o conteúdo deste componente é outra coisa, podendo ter o nome "stringEsquerda". 

#### 2.4 Blocos & Documentação

No link abaixo vocês encontrarão a documentação completa dos blocos referentes a variáveis no App Inventor.

http://ai2.appinventor.mit.edu/reference/blocks/variables.html

#### 2.5 Exercícios

<ol>
  <li>
    Crie um aplicativo que lê do usuário dois valores, salvando cada valor em uma variável. Depois junte os valores e salve em uma terceira variável, em seguida, mostre-a na tela como resultado da junção. 
  </li>

  <li>
    Faça a mesma coisa da questão anterior, porém, restrinja os valores a serem apenas números. E ao contrário de juntar os valores, faça botões para mostrar as quatro operações matemáticas entre os dois valores das variávies lidas. Desconsidere o erro de divisão por 0.
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

### 3 Funções

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

#### 3.1 Exercício de Pensamento

Imagine a situação onde um gerente de um depósito de construção precisa, todo mês, pelo menos uma vez, calcular qual será a quantidade de cada produto que será necessária a realização de uma compra mensal, com a finalidade de reposição de estoque. Ok, sendo que o gerente sabe que no seu depósito existem cinquenta tipos diferentes de produtos. Suponha que para escrever um algorítmo, um programador opte por percorrer a lista de tipos de produtos, e para cada tipo, retornando a quantidade de compras para reposição, levando em consideração o critério de reposição somente se existir 10 ou menos produtos do mesmo tipo. 

Como você acha que deve ser feito este algorítmo? Elabore um algoritmo em programação por blocos que em teoria realiza o que o gerente precisa (somente a ideia, não precisa executar).


</div>
