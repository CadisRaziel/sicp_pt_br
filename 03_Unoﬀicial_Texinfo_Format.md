# Introdução ao Formato Texinfo Não Oficial (SICP)

Esta é a segunda edição do livro SICP (Structure and Interpretation of Computer Programs), no Formato Texinfo Não Oficial.

Você provavelmente está lendo em um navegador de hipertexto Info, como o modo Info do Emacs. Alternativamente, você pode estar lendo em formato TEX na sua tela ou impressora, embora isso seria bobo. E, se impresso, caro.

O formato oficial distribuído gratuitamente HTML-e-PDF foi primeiramente convertido pessoalmente para o Formato Texinfo Não Oficial (UTF) versão 1 por Lytha Ayth durante um longo fim de semana de amor com o Emacs em abril de 2001.

O UTF é mais fácil de pesquisar do que o formato HTML. Também é muito mais acessível para pessoas que utilizam computadores modestos, como PCs baseados em '386 doados. Um 386 pode, em teoria, executar Linux, Emacs e um interpretador Scheme simultaneamente, mas a maioria dos 386s provavelmente não conseguiria rodar Netscape e o necessário X Window System sem introduzir prematuramente jovens hackers subfinanciados ao conceito de thrashing (exaustão de memória/recursos). O UTF também pode caber descompactado em um disquete de 1.44 MB, o que pode ser útil para instalar o UTF em PCs que não têm acesso à Internet ou à LAN.

A conversão para Texinfo foi uma transliteração direta, na medida do possível. Assim como a conversão de TEX para HTML, isso não ocorreu sem a introdução de algumas falhas. No caso do Formato Texinfo Não Oficial, as figuras sofreram uma ressurreição amadora da arte perdida do ASCII. Além disso, é bem possível que alguns erros de ambiguidade tenham sido introduzidos durante a conversão de alguns dos copiosos sobrescritos ('^') e subscritos ('_'). Descobrir quais são foi deixado como um exercício para o leitor. Mas pelo menos não colocamos nossos bravos astronautas em risco codificando o símbolo "maior ou igual" como &gt;.

Se você modificar sicp.texi para corrigir erros ou melhorar a arte ASCII, então atualize a linha @set utfversion 2.andresraba5.6 para refletir a sua alteração (delta). Por exemplo, se você começou com a versão 1 de Lytha, e seu nome é Bob, você poderia nomear suas versões sucessivas 1.bob1, 1.bob2, . . . 1.bobn. Atualize também utfversiondate. Se você quiser distribuir sua versão na Web, incluir a string "sicp.texi" em algum lugar do arquivo ou da página da Web facilitará a localização pelas pessoas através dos motores de busca.

Acredita-se que o Formato Texinfo Não Oficial esteja em conformidade com o espírito da versão HTML graciosamente distribuída gratuitamente. Mas nunca se sabe quando a armada de advogados de alguém pode precisar de algo para fazer e ficar incomodada com alguma pequena coisa benigna, então pense duas vezes antes de usar seu nome completo ou distribuir formatos Info, DVI, PostScript ou PDF que possam incluir sua conta ou nome da máquina.

Paz, Lytha Ayth

Adendo e Atualização
Adendo: Veja também as vídeo-aulas SICP por Abelson e Sussman: na MIT OCW ou MIT CSAIL.

Segundo Adendo: O que está acima é a introdução original ao UTF de 2001. Dez anos depois, o UTF foi transformado: símbolos e fórmulas matemáticas estão devidamente tipografados, e figuras desenhadas em gráficos vetoriais. As fórmulas de texto originais e as figuras de arte ASCII ainda estão lá na fonte Texinfo, mas só serão exibidas quando compiladas para saída Info. Na aurora dos leitores de e-books e tablets, ler um PDF na tela oficialmente não é mais bobo. Aproveite!

A.R, Maio, 2011