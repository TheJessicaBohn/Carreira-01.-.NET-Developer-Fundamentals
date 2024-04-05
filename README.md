# [Carreira 01. .NET Developer Fundamentals](https://balta.io/carreiras/dotnet-fundamentals)

## Linguagens e Compiladores:
- ## O que são linguagens de programação?
    - **Definições:**
        - É uma forma de comunicação humano-computador, onde o humano fala para o computador como executar um comando;
        - Já que os computadores entendem apenas binário, uma LP (linguagem de programação), faz esse intermédio;
        - O que escrevemos em determinada linguagem o compilador transforma em liguagem de maquina (binário);
        - Em resumo temos um arquivo de texto:
            - Que um humano consegue ler;
            - Que será traduzido para binário;

- ## Alto e Baixo Nível:
    - **Definições:**
      - O envio de instruções ao computador é o nível de maquina;
      - As instruções ao computador sempre serão no formato binário;
      - Quanto mais detalhada(como microproessadores que tem pouca memória) a necessidade, mais baixo é o nível;
      - Linguagens mais modernas e mais proximas do usuário, como C# e Java, são chamados de liguagem de alto nível, pois é mais favorecida para os usuários em detrimento do processador;
      - Assembly: Baixo nível;
      - C#: Alto nível;
      - Linguagens de alto nível são geralmente mais escolhidas pois trazem um acesso há tudo que precisamos em nível de hardware, já prontos;
 
- ## Linguagens compiladas e interpretadas:
    - **Definições:**
      - **Compiladas:**
          - É quando existe o processo de compilção da linguagem;
          - Consiste em receber um arquivo de texto e convertê-lo num binário;
          - Normamente são mais legíveis para o ser humano;
      - **Interpretadas:**
          - Arquivos de testo puro, não transformados em binários;
          - Eles são lidos em tempo de execução, por um intérprete;
          - JavaScript é um exemplo de linguagem interpretada;
          - No caso do JavaScript:
              - O navegador é escrito em uma linguagem de auto nível;
              - Possuindo um interpretador;
              - Lê e executa um arquivo de JavaScript;

- ## Compilada VS Interpretada:
    - **Definições:**
      - Geralmente usamos as duas, principalmente se você for um desenvolvedor Web;
      - Não se prenda há um tipo de linguagem pois no fim,não faz diferença pois a compilação ou interpretação ocorre "por baixo dos panos";
      - Aprenda bem uma(Seja especialista em uma), mas conheça outras também;
      - **Interpretadas:**
        - **Prós:**
          - Não precisa ser compilada (só colocar um novo arquivo) ;
          - Correções mais faceis de serem executadas, pois são arquivos estáticos e não tem a necessidade de ser traduzida para uma linguagem de maquina antes, um output antes;
          - Mais simples de serem distribuídas;
        - **Contras: (Tradeoffs)**
          - Detecção de erros: só ocorrem em tempo de execução (só aparecem quando o cliente estiver visualizando o seu site);
          - Tamanho maior no final da aplicação, pois são arquivos textos e não binários que seriam quase como um zip, porém existe ferramentes que fazem a minificação do arquivo;
          - Menor otimização da execução;
          - Multiplos arquivos;
      - **Compiladas:**
        - **Prós:**
          - Tempo de compilação: Detectamos os erros no tempo de compilação, por isso a detecção dos erros são mais rápidos, e conseguimos ver isso já do nosso lado sem precisar a nossa aplicação para o cliente e depois ter que mandar uma correção, caso algo de errado;
          - Tamanho menor das aplicações, um exemplo em .NET no Windowns temos um .exe, ou um .dll, ou no Mac ou Linux temos sempre uma .dll, ou seja já é um arquivo nativamente mais compactado num formato que o computador entende, binário, com espaços e caracteres expeciais já removidos;
          - E como resultado final ele tem apenas um arquivo final por projeto;
        - **Contras: (Tradeoffs)**
          - Precisa de um compilador, nas linguagem interpretadas, podemos simplesmente pegar o arquivo e "jogar" para o browser, enquanto as complidas precisamos instalar um compilador;
          - Pode ser mais burocrática, pelo fato de ter que instalar programas a parte, além de que se você criou uma aplicação com erro, é necessário recompilar de novo e redistribuir a aplicação;

- ## Tipagem de dados:
  - **Definições:**
    - São linguagens também chamadas de fortemente tipadas;
    - Obrigam a especificar o **tipo de dado** da informação;
    - Menor liberdade (diferente do JavaScript com var);
    - Maior otimização, pois ele já sabe onde na memória ele vai guardar aquela informação, pois pelo tipo ele sabe o tamanho e nde guardar aquela variável;
     ``` int idade = 18; // Ok
     int idade = 18.2; // Erro
     int idade = "18"; // Erro
     int idade = 'a'; // Erro
     ```
    - Nada fora de um número inteiro é aceito no caso acima em C#, que é uma linguagem fortemente tipada;
    - Esse mesmo exemplo em JavaScript que é uma linguagem fracamente ou não tipada, teriamos o seguinte resultado:
     ``` int idade = 18; // Ok
      int idade = 18.2; // Ok
      int idade = "18"; // Ok
      int idade = 'a'; // Ok
      ```
    - Por definição os tipos são para padronizar os dados, para nós e para o processador/memória;
    - O **let** utiliza sempre o mesmo tamanho de alocação;
    - Tipando temos uma otimização, o compilador avisa do erro, além de saber o espaço de memória a ser alocado previamente, trazendo assim mais performance para o programa;
    - Exemplo no **C#**:
     ``` int => 32 bit
      float => 32 bit
      double => 64 bit
      decimal => 128 bit
      ```
- ## Revisão:
  - **Definições:**
  - Linguagens Tipadas e não tipadas;
      - Sendo o C# uma linguagem tipada ou fortemente tipada;
  - Linguagens compiladas ou interpretadas;
      - Sendo o C# uma linguagem compilada;
  - Linguagens de alto e de baixo nível;
      - Sendo o C# de alto nível;
  - Compildores Vs Interpretadores;

## C#:
- ## Por que utilizar C#?
  - C# é ima linguagem de programação: tipada compilada e gerenciada;
  - Criada por Anders Hejlsberg (também criador do Delphi e do TypeScript)
em meados de 2001;
  - Principal linguagem da Microsoft (Substituindo VB) ;
   - **Vantagens:**
   - Linguagem completa - Uma das mais completas do mercado atualmente, e como ele faz parte de um ecossistema não serve para apenas para aplicações web ou desktop e mobile, ele serve também para machine learn em data science, diversas outras tecnologias e frameworks também usam C#, assim como games, por exemplo o Unity que é uma das plataformas mais famosas;
   - Maturidade, desde a sua criação em 2001 ele vem sido atualizado, e pelo tempo que ele está no mercado tem muito conteúdo, diferente de uma nova tecnologia que você tem que desbravar tudo sozinho além do fato que pode ser que não vingue. Além de achar mais facilmente profissionais na área;
   - Mercado enterprise, mais voltado para grande empresas, até pela dificulade das grandes empresas em fazer mudanças;
   - Comunidade, grande quantidade de comunidade pelo mundo trazendo assim um amparo;
   - Aplicabilidade, por ser muito completa, aprendendo bem o C#, você está hábil a criar qualquer tipo de aplicação com uma boa base;
   - MicroSoft por trás;
   - Orientação à Objetos;

- ## C# como primeira linguagem:
  - **Definições:**
  - Não é a mais fácil, existem outras como **Python** como **JavaScript**, onde se tem bem menos coisas pra se aprender, e por esse motivo são relativamente mais fáceis de serem aprendidas;
  - Focada em OOP (Base da programação), todo desenvolvedor precisa saber de Programação orientada a objetos, e o C# te obriga a trabalhar nesse formato;
    - Temos também a progrmação funcional;
  - Fácil no começo pode te prejudicar no fim, pois se você começa com uma linguagem não orientada a objetos uma hora você vai precisar saber sobre o assunto;
  - OOP te dá a base para aprender coisas novas, principalmente que surgem o tempo todo na nossa área atualmente;
  - A conta uma hora vem, se você não aprender agora, vai ter que voltar e aprender;
  - Quanto mais tempo na base, mais fácil de aprender coisas novas, se você passar muito rapidamente pela base e partir logo pra framework e coisas mais avançadas vai chegar uma hora que você vai ficar estaguinando na sua carreira, aí você vai ter que parar pra aprender o básico;
  - A quantidade de horas é a mesma, pois se não você vai ter que voltar para trás pra aprender;
    - Você escolhe quanto tempo vai investir no básico, não existe mágica, tem que praticar, por mais que seja chato e não prazeroso;
  - Se você não consolidou o básico ainda:
    - Você tem dificuldades de aprender coisas novas, se você demora muito pra aprender coisas novas é porque você não sabe bem o básico;
    - Dificuldade em codificar coisas diferentes do seu cotidiano;
    - Resistência a mudanças, medo de aprender ou fazer coisas novas;
    - Pare e aprenda agora;

- ## Código gerenciado:
  - **Lembrando que:**
  - C# é uma uma linguagem fortemente tipada;
  - Compilada e;
  - De código **gerenciado**;
  - **Definições:**
  - Significa que a sua execução depende de um gerenciador;
  - Também conhecida como **Runtime**;
    - No caso o do C# o **Runtime**  se chama **CLR** ou **CLR Runtime**;
  - Gerencia memória, segurança, entre outros recursos básicos;
  - Linguagens como C/C++ por exemplo, se faz necessário a alocação de memória manualmente (fora do .NET);
    - Famoso ``` p = malloc (sizeof (int));
                 *p = 123;
                 free (p);```, que alocava e desalocava memória, e as chances de dar bugs e erros eram muito grandes;
  - Sabe a famosa tela azul do Windows? Isso ocorre muitas vezes pois algum programa tentou acessar uma mémoria que era reservado para o SO;
  - Permite interagirmos menos ou quase não interagirmos com recursos de maquina, ou seja tira essa parte mais "mecanica" na mão do desenvolvedor;
    - O gerenciador vai saber a hora de alocar ou limpar a memoria, qual área é segura e assim por diante;
    - Dessa forma é possível focar muito mais nas regras de negócio;

- ## Compilação e gerenciamento:
  - **Definições:**
  - A MS possui outras linguagens como o VB.NET, F#, e até mesmo Cobol.NET;
  - Todas elas precisam ser mantidas;
    - Manutenção de código mesmo, correções de bugs e afins;
  - Quando o ecossistema de desenvolvimento MS foi criado ele foi pensado desta forma:
    -  Suporte a várias linguagens;
  - Se cada linguagem tiver um gerenciador, isto seria muito complicado;
  - Os compiladores são separados;
    - Um para cada linguagem (ou mais de uma linguagem);
  - A compilação inicial gera um código intermediário (não gera o código binário);
    - Intermediate Language (IL);
    - Serve para manter apenas um gerenciador final;
    - Quando compilamos o código C# ele é traduzido para essa liguagem intermédiaria e depois ele é compilado, assim como nas outras linguagens como o VB.Net, F# e outras linguagens;
    - Isso é muito legal pois permite que tenha apenas um gerenciador final para essas linguagens, e tenhamos diferentes tipos de arquivos dentro do nosso projeto, então nada impede de que tenhamos um arquivo VB.NET ou F# dentro do nosso projeto C#;
    - Mas geralmente escolhemos apenas um tipo de linguagem apenas;

- ## IL:
  - **Definições:**
  - Embora as compilações sejam diferentes:
    - O gerenciamento é igual;
    - Alocação de memoria;
    - Execução de instruções no processador;
  - O CLR recebe um código e compila ele para IL:
    - C#, VB.NET, F#, Cobol.NET;
  - Podemos ter arquivos C# e VB.NET no mesmo projeto:
    - Porém nunca no mesmo arquivo, pela sintaxe de cada linguagem;
  - O resultado da compilação IL é sempre o mesmo;
  - O processo de conversão do IL para binário é conhecido como JIT
    
    ![image](https://github.com/TheJessicaBohn/Carreira-01.-.NET-Developer-Fundamentals/assets/47541659/ccbee0a1-05e9-40d6-81d1-42a7e571a68c)
 
- ## Revisão:
  - **Definições:**
  - C# é maduro, completo, popular e tem muito material;
  - Linguagem, gerenciada, compilada e de alto nível;
  - É uma linguagem desafiadora,mas vai te dar uma ótima bagagem;
  - O C# é compilado inicialmente para IL;
  - Depois o CLR compila para código de maquina, executa e gerencia, mão na roda para o progrmador não ter que fazer o processo na mão;
  - IL é a linguagem intermediaria na qual todas as linguagens da Microsoft são compiladas;

## Frameworks:

- ## Frameworks:
  - **Definições:**
  - Framework é uma estrutura, um alicerce
    - Um conjunto de bibliotecas;
  - Usamos como base para construir nossas aplicações
    - Pra não precisar fazer tudo, começando do zero, como por exemplo escrever um arquivo texto no disco;
    - Quando utilizamos um framework, estamos utilizando um código base que já foi testado, estressando e temos assim, n outras garantias;
  - Conceito existente em diversas tecnologias, como por exemplo Java, JavaScript, etc;
  - Nesse curso veremos o **.NET**, um Framework Microsoft;
  - Ideia é trazer recursos comuns jé prontos:
    - Itens do dia-a-dia;
    - Escrita de arquivo em disco, por exemplo:
      - Acesso a banco de dados;
      - Criar um site;
      - Criar uma aplicação Desktop;
      - Um desenho de uma janela do Windows;
      - O desenho de um botão;
  - .NET nasceu junto com o C# em 2001
  - Framework poderoso; 
  - Validados e testados;
  - Nos poupam muito tempo;
  - Não vale a pena começar sem um pois o risco é menor;

- ## .NET Framework:
- ## .NET Core:
- ## Standard:
- ## .NET 5:
- ## LTS:
- ## Versionamento:
- ## Runtime e SDK:
- ## Revisão:

## .NET
- ## Instalação:
- ## dotnet cli:
- ## VS Code:
- ## Tipos de projeto:
- ## Fluxo de execução:
- ## Variáveis de ambiente;
- ## Estrutura do App:
- ## Debug:
- ## Revisão:

## Linguegem de Programação - com C#:
- ## Notas importantes:
- ## Escopo de um programa:
- ## Namespaces:
- ## Using:
- ## Variáveis:
- ## Constantes:
- ## Palavras Reservadas:
- ## Comentários:
- ## Tipos primitivos:
- ## System;
- ## Byte:
- ## Números inteiros:
- ## Números reais:
- ## Boolean:
- ## Char:
- ## String:
- ## Var:
- ## Object:
- ## Nullable Types:
- ## Alias:
- ## Valores padrões:
- ## Conversão implícita:
- ## Conversão explicita:
- ## Parse:
- ## Convert:
- ## Convertendo Tipos:
- ## Operadores aritméticos:
- ## Operadores de atribúição:
- ## Operadores de comparação:
- ## Utilizando operadores:
- ## Operadores lógicos:
- ## Operador condicional - IF:
- ## Utilizando IF:
- ## Estrutura Condicional - Switch:
- ## Laços de repetição - For:
- ## Laços de repetição - While:
- ## Laços de repetição - Do/While:
- ## Métodos e funções:
- ## Métodos e funções - Prática:
- ## Value Types e Reference Types:
- ## Value Types e Reference Types - Prática:
- ## Structs
- ## Structs - Prática:
- ## Enums:
- ## Revisão:

## Mão na massa - Criando uma calculadora:
- ## Iniciando o projeto:
- ## Soma:
- ## Utilizando Funções:
- ## Subtração:
- ## Divisão:
- ## Multiplicação:
- ## Menu da aplicação:
- ## Chamando as funções:
- ## Saindo da aplicação:
- ## Revisão:

## Mão na massa - Cronômetro:
- ## Iniciando o projeto:
- ## Estrutura do cronômetro:
- ## Thread e Sleep:
- ## Criando o menu:
- ## Opções do menu:
- ## Substring:
- ## Obtendo a opção:
- ## Calculando o tempo:
- ## Finalizando a aplicação
- ## Revisão:

## Mão na massa - Editor de textos:
- ## Iniciando o projeto:
- ## Iteração e caractere de escape:
- ## Do/While na prática:
- ## StreamWriter
- ## Salvando arquivo:
- ## Abrindo Arquivos:
- ## Revisão:

## Strings:
- ## Guids:
- ## Interpolação de Strings:
- ## Comparação de Strings:
- ## StartsWith/EndsWith:
- ## Equals:
- ## Índices:
- ## Métodos adicionais:
- ## Manipulando strings:
- ## StringBuilder:
- ## Revisão:

## Mão na massa - Editor HTML:
- ## Iniciando o projeto:
- ## Desenhando a tela:
- ## Exibindo o menu:
- ## Menu da aplicação:
- ## Editor:
- ## Visualizador:
- ## Substituindo caracteres:
- ## Revisão:

## Datas:
- ## Iniciando com datas:
- ## Obtendo valores da data:
- ## Formatando datas:
- ## Padrões de formatação:
- ## Adicionando valores:
- ## Comparando datas:
- ## CultureInfo:
- ## Timezone:
- ## Timespan:
- ## Revisão:

## Moedas:
- ## Tipo para moedas:
- ## Formatando moedas:
- ## Math:
- ## Revisão:

## Arrays:
- ## Arrays:
- ## Percorrendo um array:
- ## ForEach:
- ## Alterndo valores:
- ## Revisão:

## Exceptions:
- ## Exceptions:
- ## Try/Catch:
- ## Tratando erros:
- ## Disparando exceções:
- ## Finally:
- ## Revisão:

## Conclusão:

## Glossário:
- **CLR:** É a sigla para Common Language Runtime ou gerenciador de linguagem comum;
- **Compilador:** Agente que executa a compilação, que é a transformação do texto que escrevemos para binário(0 e 1). Lembrando que cada linguagem tem o seu próprio compilador. Um exemplo que eu gosto muito de usar para quem é bem leigo é que o programa escrito é como se fosse uma musica na partitura, e nós ao tocarmos somos os "compiladores".
- **IL:** Sigla para Intermediate Language;
- **JIT:** Sigla para Just In Time;
- **MS:** MicroSoft;
- **OOP - Object-oriented programming: ** Programação orientada a objetos;
- **SO:** Sistema Operacional;
- **Tempo de Execução:** É o que acontece durante a execução  do código pelo computador ou interpretador.
- **Tipo de dado:** um tipo de dado define  o formato dele, onde definimos por exemplo que aquela informação é um número, uma letra, uma cadeia de caracteres e assim por diante;

## Fonte:
- ## https://balta.io/carreiras/dotnet-fundamentals
