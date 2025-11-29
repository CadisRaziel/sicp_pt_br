# Conteúdo

## Pré-textuais
- **Formato Texinfo Não Oficial** — ix  
- **Dedicação** — xii  
- **Prefácio** — xiii  
- **Prefácio à Segunda Edição** — xix  
- **Prefácio à Primeira Edição** — xxi  
- **Agradecimentos** — xxv  

---

# 1. Construindo Abstrações com Procedimentos — 1

## 1.1 Os Elementos da Programação — 6
- **1.1.1 Expressões** — 7  
- **1.1.2 Nomenclatura e o Ambiente** — 10  
- **1.1.3 Avaliando Combinações** — 12  
- **1.1.4 Procedimentos Compostos** — 15  
- **1.1.5 O Modelo de Substituição para Aplicação de Procedimentos** — 18  
- **1.1.6 Expressões Condicionais e Predicados** — 22  
- **1.1.7 Exemplo: Raízes Quadradas pelo Método de Newton** — 28  
- **1.1.8 Procedimentos como Abstrações de Caixa-Preta** — 33  

## 1.2 Procedimentos e os Processos que Eles Geram — 40
- **1.2.1 Recursão Linear e Iteração** — 41  
- **1.2.2 Recursão em Árvore** — 47  
- **1.2.3 Ordens de Crescimento** — 54  
- **1.2.4 Exponenciação** — 57  
- **1.2.5 Máximos Divisores Comuns** — 62  
- **1.2.6 Exemplo: Testando a Primalidade** — 65  

## 1.3 Formulando Abstrações com Procedimentos de Ordem Superior — 74
- **1.3.1 Procedimentos como Argumentos** — 76  
- **1.3.2 Construindo Procedimentos Usando `lambda`** — 83  
- **1.3.3 Procedimentos como Métodos Gerais** — 89  
- **1.3.4 Procedimentos como Valores Retornados** — 97  

---

# 2. Construindo Abstrações com Dados — 107

## 2.1 Introdução à Abstração de Dados — 112
- **2.1.1 Exemplo: Operações Aritméticas para Números Racionais** — 113  
- **2.1.2 Barreiras de Abstração** — 118  
- **2.1.3 O que Significa Dados?** — 122  
- **2.1.4 Exercício Estendido: Aritmética de Intervalos** — 126  

## 2.2 Dados Hierárquicos e a Propriedade de Fechamento — 132
- **2.2.1 Representando Sequências** — 134  
- **2.2.2 Estruturas Hierárquicas** — 147  
- **2.2.3 Sequências como Interfaces Convencionais** — 154  
- **2.2.4 Exemplo: Uma Linguagem de Imagens** — 172  

## 2.3 Dados Simbólicos — 192
- **2.3.1 Cotação** — 192  
- **2.3.2 Exemplo: Diferenciação Simbólica** — 197  
- **2.3.3 Exemplo: Representando Conjuntos** — 205  
- **2.3.4 Exemplo: Árvores de Codificação de Huffman** — 218  

## 2.4 Múltiplas Representações para Dados Abstratos — 229
- **2.4.1 Representações para Números Complexos** — 232  
- **2.4.2 Dados Rotulados (Tagged Data)** — 237  
- **2.4.3 Programação Orientada a Dados e Aditividade** — 242  

## 2.5 Sistemas com Operações Genéricas — 254
- **2.5.1 Operações Aritméticas Genéricas** — 255  
- **2.5.2 Combinando Dados de Tipos Diferentes** — 262  
- **2.5.3 Exemplo: Álgebra Simbólica** — 274  

---

# 3. Modularidade, Objetos e Estado — 294

## 3.1 Atribuição e Estado Local — 296
- **3.1.1 Variáveis de Estado Local** — 297  
- **3.1.2 Benefícios da Introdução da Atribuição** — 305  
- **3.1.3 Custos da Introdução da Atribuição** — 311  

## 3.2 O Modelo de Ambiente de Avaliação — 320
- **3.2.1 Regras para Avaliação** — 322  
- **3.2.2 Aplicando Procedimentos Simples** — 327  
- **3.2.3 Frames e Estado Local** — 330  
- **3.2.4 Definições Internas** — 337  

## 3.3 Modelagem com Dados Mutáveis — 341
- **3.3.1 Estrutura de Lista Mutável** — 342  
- **3.3.2 Representando Filas** — 353  
- **3.3.3 Representando Tabelas** — 360  
- **3.3.4 Um Simulador para Circuitos Digitais** — 369  
- **3.3.5 Propagação de Restrições** — 386  

## 3.4 Concorrência: O Tempo é Essencial — 401
- **3.4.1 A Natureza do Tempo em Sistemas Concorrentes** — 403  
- **3.4.2 Mecanismos para Controlar a Concorrência** — 410  

## 3.5 Fluxos (Streams) — 428
- **3.5.1 Fluxos São Listas Atrasadas** — 430  
- **3.5.2 Fluxos Infinitos** — 441  
- **3.5.3 Explorando o Paradigma de Fluxos** — 453  
- **3.5.4 Fluxos e Avaliação Atrasada** — 470  
- **3.5.5 Modularidade de Programas Funcionais e Modularidade de Objetos** — 479  

---

# 4. Abstração Metalinguística — 487

## 4.1 O Avaliador Metacircular — 492
- **4.1.1 O Núcleo do Avaliador** — 495  
- **4.1.2 Representando Expressões** — 501  
- **4.1.3 Estruturas de Dados do Avaliador** — 512  
- **4.1.4 Executando o Avaliador como Programa** — 518  
- **4.1.5 Dados como Programas** — 522  
- **4.1.6 Definições Internas** — 526  
- **4.1.7 Separando Análise Sintática e Execução** — 534  

## 4.2 Variações — Scheme com Avaliação Lazy — 541
- **4.2.1 Ordem Normal e Aplicativa** — 542  
- **4.2.2 Interpretador com Avaliação Lazy** — 544  
- **4.2.3 Fluxos como Listas Lazy** — 555  

## 4.3 Scheme com Computação Não Determinística — 559
- **4.3.1 Amb e Busca** — 561  
- **4.3.2 Exemplos de Programas Não Determinísticos** — 567  
- **4.3.3 Implementando o Avaliador amb** — 578  

## 4.4 Programação Lógica — 594
- **4.4.1 Recuperação de Informação Dedutiva** — 599  
- **4.4.2 Funcionamento do Sistema de Consulta** — 615  
- **4.4.3 Programação Lógica é Lógica Matemática?** — 627  
- **4.4.4 Implementando o Sistema de Consulta** — 635  
  - **4.4.4.1 Loop do Driver e Instanciação** — 636  
  - **4.4.4.2 O Avaliador** — 638  
  - **4.4.4.3 Pattern Matching** — 642  
  - **4.4.4.4 Regras e Unificação** — 645  
  - **4.4.4.5 Mantendo o Banco de Dados** — 651  
  - **4.4.4.6 Operações de Fluxo** — 654  
  - **4.4.4.7 Sintaxe de Consulta** — 656  
  - **4.4.4.8 Frames e Ligações** — 659  

---

# 5. Computação com Máquinas de Registradores — 666

## 5.1 Projetando Máquinas de Registradores — 668
- **5.1.1 Linguagem para Descrição** — 672  
- **5.1.2 Abstração no Projeto** — 678  
- **5.1.3 Sub-rotinas** — 681  
- **5.1.4 Pilha e Recursão** — 686  
- **5.1.5 Sumário de Instruções** — 695  

## 5.2 Simulador de Máquina de Registradores — 696
- **5.2.1 Modelo da Máquina** — 698  
- **5.2.2 Montador (Assembler)** — 704  
- **5.2.3 Gerando Execução para Instruções** — 708  
- **5.2.4 Monitorando Desempenho** — 718  

## 5.3 Alocação de Armazenamento e Coleta de Lixo — 723
- **5.3.1 Memória como Vetores** — 724  
- **5.3.2 Ilusão de Memória Infinita** — 731  

## 5.4 Avaliador de Controle Explícito — 741
- **5.4.1 Núcleo do Avaliador** — 743  
- **5.4.2 Avaliação de Sequência e Tail Recursion** — 751  
- **5.4.3 Condicionais, Atribuições e Definições** — 756  
- **5.4.4 Executando o Avaliador** — 759  

## 5.5 Compilação — 767
- **5.5.1 Estrutura do Compilador** — 772  
- **5.5.2 Compilando Expressões** — 779  
- **5.5.3 Compilando Combinações** — 788  
- **5.5.4 Combinando Instruções** — 797  
- **5.5.5 Exemplo de Código Compilado** — 802  
- **5.5.6 Endereçamento Lexical** — 817  
- **5.5.7 Interface com o Avaliador** — 823  

---

# Pós-textuais
- **Referências** — 834  
- **Lista de Exercícios** — 844  
- **Lista de Figuras** — 846  
- **Índice** — 848  
- **Colofão** — 855  
