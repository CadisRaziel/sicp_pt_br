# 1.1.1 Expressões
Uma maneira fácil de começar a programar é examinar algumas interações típicas com um interpretador para o dialeto Scheme do Lisp.

Imagine que você está sentado em um terminal de computador. Você digita uma expressão e o interpretador responde exibindo o resultado da avaliação dessa expressão.

Um tipo de expressão primitiva que você pode digitar é um número. (Mais precisamente, a expressão que você digita consiste nos numerais que representam o número na base 10.)  

Se você apresentar o Lisp com um número:
486
o interpretador responderá imprimindo:
486

A caracterização de números como "dados simples" é um blefe descarado. Na verdade, o tratamento de números é um dos aspectos mais complicados e confusos de qualquer linguagem de programação. Algumas questões típicas envolvidas são:
Alguns sistemas de computador distinguem inteiros, como 2, de números reais, como 2.71.
O número real 2.00 é diferente do inteiro 2?
As operações aritméticas usadas para inteiros são as mesmas que as operações usadas para números reais?
6 dividido por 2 produz 3 ou 3.0?
Qual é o tamanho máximo de número que podemos representar?
Quantas casas decimais de precisão podemos representar?
O intervalo de inteiros é o mesmo que o intervalo de números reais?
Acima e além dessas questões, é claro, reside uma coleção de problemas relacionados a erros de arredondamento e truncamento — toda a ciência da análise numérica. Uma vez que nosso foco neste livro é o projeto de programas em larga escala, e não técnicas numéricas, vamos ignorar esses problemas. Os exemplos numéricos neste capítulo exibirão o comportamento usual de arredondamento que se observa ao usar operações aritméticas que preservam um número limitado de casas decimais de precisão em operações não inteiras.

Expressões que representam números podem ser combinadas com uma expressão que representa um procedimento primitivo (como + ou *) para formar uma expressão composta que representa a aplicação do procedimento a esses números.Por exemplo:

(+ 137 349)
486

(- 1000 334)
666

(* 5 99)
495

(/ 10 5)
2

(+ 2.7 10)
12.7

Expressões como estas, formadas ao delimitar uma lista de expressões entre parênteses para denotar a aplicação de procedimento, são chamadas combinações. O elemento mais à esquerda na lista é chamado de operador, e os outros elementos são chamados de operandos. O valor de uma combinação é obtido aplicando-se o procedimento especificado pelo operador aos argumentos que são os valores dos operandos.A notação de colocar o operador à esquerda dos operandos é conhecida como notação prefixa, e pode ser um pouco confusa no início porque se afasta significativamente da convenção matemática habitual (que usa notação infixa, como 137 + 349).A notação prefixa, no entanto, tem várias vantagens. Uma delas é que ela pode acomodar procedimentos que podem receber um número arbitrário de argumentos, como nos exemplos a seguir:

(+ 21 35 12 7)
75

(* 25 4 12)
1200

Nenhuma ambiguidade pode surgir, porque o operador é sempre o elemento mais à esquerda e toda a combinação é delimitada pelos parênteses.

Vantagem da Aninhamento (Nesting)
Uma segunda vantagem da notação prefixa é que ela se estende de forma direta para permitir que as combinações sejam aninhadas (ou encaixadas), ou seja, para que as combinações tenham elementos que são, por sua vez, outras combinações:

(+ (* 3 5) (- 10 6))
19

Não há limite (em princípio) para a profundidade desse aninhamento e para a complexidade geral das expressões que o interpretador Lisp pode avaliar. Somos nós, humanos, que ficamos confusos com expressões ainda relativamente simples, como:

(+ (* 3 (+ (* 2 4) (+ 3 5))) (+ (- 10 7) 6))

que o interpretador avaliaria prontamente como 57.

Podemos nos ajudar escrevendo tal expressão no formato:

(+ (* 3
       (+ (* 2 4)
          (+ 3 5)))
   (+ (- 10 7)
      6))

seguindo uma convenção de formatação conhecida como pretty-printing (impressão elegante), na qual cada combinação longa é escrita de forma que os operandos fiquem alinhados verticalmente. As indentações resultantes exibem claramente a estrutura da expressão.

Mesmo com expressões complexas, o interpretador opera sempre no mesmo ciclo básico: Ele lê uma expressão do terminal, avalia a expressão e imprime o resultado. Esse modo de operação é frequentemente expresso dizendo-se que o interpretador roda em um loop (laço) de leitura-avaliação-impressão (read-eval-print loop).

Observe em particular que não é necessário instruir explicitamente o interpretador para imprimir o valor da expressão.