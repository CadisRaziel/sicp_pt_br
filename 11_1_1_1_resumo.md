## Interação e Expressões em Lisp
Programar em um dialeto Lisp, como Scheme, começa com a interação básica de um interpretador (a máquina que executa o código) em um ciclo de leitura-avaliação-impressão (read-eval-print loop):

* Lê: Você digita uma expressão (seu código).

* Avalia: O interpretador calcula o valor dessa expressão.

* Imprime: O interpretador exibe o resultado automaticamente.

1. Expressões Primitivas (Números)
O tipo mais simples de expressão é o número. Se você digita um número, o interpretador o avalia e retorna o mesmo número.Nota: Embora pareça simples, o tratamento de números (como distinguir entre inteiros como $2$ e reais como $2.00$, e lidar com limites de tamanho e precisão) é, na verdade, um dos aspectos mais complexos de qualquer linguagem de programação. Para este estudo, esses problemas serão ignorados.

2. Combinações (Aplicações de Procedimento)O poder do Lisp começa com a forma como ele combina expressões para realizar ações.Notação Prefixa (O Padrão Lisp)Em Lisp, as combinações são escritas usando a notação prefixa, que é diferente da matemática usual (infixa):Matemática (Infixa): $1 + 2$Lisp (Prefixa): $$(+ 1 2)$$

## Estrutura de uma Combinação:
Uma combinação sempre segue este formato, delimitada por parênteses:$$( \text{Operador} \quad \text{Operando 1} \quad \text{Operando 2} \quad \dots )$$O operador é o elemento mais à esquerda (o procedimento, ex: $+$ ou $*$).Os operandos são os valores ou expressões seguintes (os argumentos).Exemplos:(+ 137 349) $\rightarrow$ 486 (O operador $+$ é aplicado aos operandos $137$ e $349$).(* 5 99) $\rightarrow$ 495

Vantagens da Notação PrefixaArgumentos Variáveis: Permite que procedimentos recebam um número arbitrário de argumentos sem ambiguidade.Exemplo: $$(+ 21 \ 35 \ 12 \ 7) \rightarrow 75$$Aninhamento Simples (Nesting): Facilita a combinação de combinações (aninhamento). O valor de uma combinação interna se torna o operando para a combinação externa. Não há limite (em princípio) para a profundidade.Exemplo: $$(+ (* 3 5) (- 10 6))$$Primeiro, ele calcula $$(* 3 5) \rightarrow 15$$Segundo, ele calcula $$(- 10 6) \rightarrow 4$$Finalmente, ele calcula $$(+ 15 4) \rightarrow \mathbf{19}$$Para lidar com expressões aninhadas muito complexas, os programadores usam o pretty-printing (impressão elegante), formatando o código com indentação para exibir visualmente a estrutura aninhada e facilitar a leitura humana.