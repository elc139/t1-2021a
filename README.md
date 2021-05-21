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
- Conforme consta na página de download, esse benchmark possui algumas dependências que você vai ter que instalar manualmente: MPI e BLAS. É recomendável usar OpenMPI compilado e instalado manualmente em espaço de usuário (usar `configure --prefix=...`), não via instalador do sistema. Quanto ao BLAS, uma opção é usar o pacote intel-mkl.
- Após instalar as dependências, siga as instruções do arquivo `INSTALL` para gerar o binário `xhpl`. Esse arquivo também indica um comando para testar a execução.
- Os parâmetros de entrada do benchmark são configurados em um arquivo `HPL.dat`, que é fornecido como exemplo junto com o código fonte. O arquivo que usaremos neste trabalho tem configurações diferentes e está disponível [aqui](HPL.dat).
- Tanto o `xhpl` como o `HPL.dat` devem estar na mesma pasta. O comando para executar os casos de teste para este trabalho é o mesmo contido no arquivo `INSTALL`. Basta substituir o `HPL.dat` original pelo [HPL.dat](HPL.dat) fornecido.
- O HPL testa vários casos conforme os parâmetros de entrada e reporta, para cada caso, o desempenho em Gflops (notação científica). Você deve localizar o maior valor obtido entre todos os casos testados. Esse é o resultado que você preencherá no arquivo de entrega.
- **Observação:** Quando se faz benchmarking real com o HPL, o ideal é fazer *tunning*  ajustando diversos parâmetros do arquivo de configuração `HPL.dat`. Isso requer um conhecimento mais aprofundado do benchmark, por isso não será exigido neste trabalho, mas quem quiser saber mais pode procurar isso na documentação :wink:. Se você ajustar o `HPL.dat` e obtiver melhor desempenho, informe isso no arquivo de entrega.

## Entrega
- Você deverá entregar o trabalho no repositório criado após aceite do link no GitHub Classroom.
- Deadline: até quarta, 26/05, 23h.

## Bibliografia
- [Taxonomia de Flynn](https://en.wikipedia.org/wiki/Flynn%27s_taxonomy)
- [A taxonomy of computer architectures](http://www-5.unipv.it/mferretti/cdol/aca/Charts/08-multicomputers-MF%20part%20II.pdf)
