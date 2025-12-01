# 1.1.2 Nomenclatura e o Ambiente
Um aspecto crítico de uma linguagem de programação é o meio que ela fornece para usar nomes para se referir a objetos computacionais. Dizemos que o nome identifica uma variável cujo valor é o objeto.

No dialeto Scheme do Lisp, nomeamos as coisas com define. Digitar:

(define size 2)

faz com que o interpretador associe o valor 2 ao nome size.
Uma vez que o nome size tenha sido associado ao número 2, podemos nos referir ao valor 2 pelo nome:

size
2

6. Recursos de Formatação
Sistemas Lisp tipicamente fornecem recursos para auxiliar o usuário na formatação de expressões. Dois recursos especialmente úteis são um que automaticamente indenta para a posição de pretty-print apropriada sempre que uma nova linha é iniciada e um que destaca o parêntese esquerdo correspondente sempre que um parêntese direito é digitado.
7. O Valor de Toda Expressão
Lisp obedece à convenção de que toda expressão tem um valor. Esta convenção, juntamente com a antiga reputação de Lisp como uma linguagem ineficiente, é a fonte da piada de Alan Perlis (parafraseando Oscar Wilde) de que "Programadores Lisp conhecem o valor de tudo, mas o custo de nada."
8. Resposta do Interpretador a Definições
Neste livro, não mostramos a resposta do interpretador à avaliação de definições, já que isso é altamente dependente da implementação.

(* 5 size)
10

Aqui estão mais exemplos do uso de define:

(define pi 3.14159)
(define radius 10)
(* pi (* radius radius))
314.159
(define circumference (* 2 pi radius))
circumference
62.8318

define é o meio de abstração mais simples de nossa linguagem, pois nos permite usar nomes simples para nos referir aos resultados de operações compostas, como a circunferência calculada acima. Em geral, objetos computacionais podem ter estruturas muito complexas, e seria extremamente inconveniente ter que lembrar e repetir seus detalhes toda vez que quiséssemos usá-los. De fato, programas complexos são construídos pela criação, passo a passo, de objetos computacionais de complexidade crescente. O interpretador torna essa construção de programas passo a passo particularmente conveniente porque as associações nome-objeto podem ser criadas incrementalmente em interações sucessivas. Este recurso incentiva o desenvolvimento e teste incremental de programas e é em grande parte responsável pelo fato de um programa Lisp geralmente consistir em um grande número de procedimentos relativamente simples.

Deve ficar claro que a possibilidade de associar valores a símbolos e recuperá-los posteriormente significa que o interpretador deve manter alguma forma de memória que rastreia os pares nome-objeto. Essa memória é chamada de ambiente (mais precisamente o ambiente global, visto que veremos mais tarde que uma computação pode envolver vários ambientes).