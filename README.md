[Programação Paralela](https://github.com/AndreaInfUFSM/elc139-2021a) > Trabalhos

T1: TOP500 & me - Comparativo de Arquiteturas Paralelas
-------------------------------------------------------

## Descrição
- Neste trabalho, você vai preencher uma tabela comparativa entre um supercomputador do [TOP500](http://top500.org) e um outro computador à sua escolha. Esse segundo computador deverá ter uma arquitetura paralela e, preferencialmente, deverá estar acessível para fazer alguns trabalhos da disciplina (p.ex.: seu notebook ou desktop com processador multicore, servidor do NCC, etc.).
- O modelo de tabela é fornecido [aqui](Entrega.md). Você deve entregar o arquivo exatamente com este nome e não deve modificar o modelo.
- Para preencher a tabela, você vai ter que fazer o seguinte:
  - Buscar informações de fabricantes, tanto para o computador do TOP500 como para seu computador.
  - Executar um benchmark **Linpack** no seu computador, para preencher o item sobre Desempenho (Flop/s) na tabela comparativa.

## Sobre o Linpack

- Existem várias distribuições e versões do Linpack, mas para padronizar nossos resultados, vamos utilizar o HPL (High Performance Linpack) versão 2.3, que está disponível em https://www.netlib.org/benchmark/hpl/. 
- Esse benchmark possui algumas dependências que você vai ter que instalar manualmente: MPI e BLAS (recomendável usar OpenMPI instalado manualmente em espaço de usuário, não via instalador do sistema, e BLAS do Intel MKL). 
- Os casos executados no benchmark são configurados em um arquivo HPL.dat, que é fornecido como exemplo junto com o código fonte. O arquivo que usaremos neste trabalho tem configurações diferentes e será disponibilizado no Discord posteriormente.


## Entrega
- Você deverá entregar o trabalho no repositório criado após aceite do link no GitHub Classroom.
- Deadline: até quarta, 26/05, 23h.

## Bibliografia
- [Taxonomia de Flynn](https://en.wikipedia.org/wiki/Flynn%27s_taxonomy)
- [A taxonomy of computer architectures](http://www-5.unipv.it/mferretti/cdol/aca/Charts/08-multicomputers-MF%20part%20II.pdf)
