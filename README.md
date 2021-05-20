[Programação Paralela](https://github.com/AndreaInfUFSM/elc139-2020a) > Trabalhos

T1: TOP500 & me - Comparativo de Arquiteturas Paralelas
-------------------------------------------------------

## Descrição
- Neste trabalho, você vai preencher uma tabela comparativa entre um supercomputador do [TOP500](http://top500.org) e um outro computador à sua escolha. Esse segundo computador deverá ter uma arquitetura paralela e, preferencialmente, deverá estar acessível para fazer alguns trabalhos da disciplina (p.ex.: seu notebook ou desktop com processador multicore, servidor do NCC, etc.).
- O modelo de tabela é fornecido [aqui](Entrega.md). Você pode modificá-lo, mas os dados solicitados na primeira coluna devem ser mantidos. 
- Para preencher a tabela, você vai ter que fazer o seguinte:
  - Buscar informações de fabricantes, tanto para o computador do TOP500 como para seu computador.
  - Executar um benchmark **Linpack** no seu computador, para preencher o item sobre Desempenho (Flop/s) na tabela comparativa.
- Existem várias distribuições do Linpack, por exemplo: HPL (High Performance Linpack), usado no TOP500; em netlib.org, com fontes disponíveis; no site da Intel; etc. O HPL é um Linpack com paralelismo e exige instalação de algumas bibliotecas. O da Intel é distribuído junto com outros benchmarks executáveis. Você pode escolher qualquer distribuição do Linpack, mas **deverá informar** onde o benchmark foi obtido.
- **Importante**: Na aula logo após a entrega do trabalho, você deve ter em mãos os dados da sua tabela.

## Entrega
- Você deverá entregar o trabalho no repositório criado após aceite do link no GitHub Classroom.
- Deadline: até segunda, 16/03, 23h.

## Bibliografia
- [Taxonomia de Flynn](https://en.wikipedia.org/wiki/Flynn%27s_taxonomy)
- [A taxonomy of computer architectures](http://www-5.unipv.it/mferretti/cdol/aca/Charts/08-multicomputers-MF%20part%20II.pdf)

