# Introdução #

Este projeto implementa uma pilha baseado em armazenamento com
lista com memória sequencial (vetor).

A pilha tem um funcionamento LIFO (last in, first out).

Este exemplo é utilizado nas aulas de Estruturas de Dados Básca 1 (BTI - UFRN) sobre listas sequenciais.

# Operações #

As operações básicas suportadas são: *verificar quem é o topo*, *inserção* e *remoção*.

Outras operações também são implementas: *esvaziar* e *verificar se vazia*.

A classe `AbsStack` é uma interface para a classe `StackInt`, que implementa uma pilha de inteiros e dobra o tamanho da pilha se a sua capacidade for alcançada, e outra classe `StackAr`, que neste caso é uma pilha de objetos genéricos, por meio de `template`.
 
Diferentemente da classe `StackInt`, `StackAr` não dobra o tamanho da pilha. Ela trabalha com a biblioteca `stdexcept`, que gera uma execeção caso o tamanho máximo seja alcançado (`include/stackar.inl`) :

	(14) throw std::length_error( "[push()]: O Tamanho máximo dessa pilha foi alcançando.\n");

-------------------------------------------
Estudo dirigido das disciplinas de **Linguagem de Programação** e **Estrutuda de Dados Básica**, do curso de Bacharelado em Tecnologia da Informação da Universidade Federal do Rio Grande do Norte (BTI - UFRN)

Professor: Selan R. dos Santos

-- The end

