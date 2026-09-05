As coleções em Java permitem armazenar e manipular conjuntos de dados de forma mais flexível do que estruturas de tamanho fixo, como arrays.

O Java Collections Framework reúne interfaces e implementações utilizadas para diferentes necessidades de organização de dados.

Entre as principais estruturas estão:

- **List:** mantém a ordem dos elementos e permite valores repetidos. Uma implementação comum é o `ArrayList`.
- **Set:** não permite elementos duplicados. Uma implementação comum é o `HashSet`.
- **Queue:** representa uma fila e pode seguir o princípio FIFO (First In, First Out). Uma implementação comum é o `ArrayDeque`.
- **Map:** trabalha com pares de chave e valor. Cada chave é única e pode ser associada a um valor. Uma implementação comum é o `HashMap`.

A escolha da coleção depende das necessidades do problema, como manter a ordem dos elementos, impedir duplicidades, localizar informações por uma chave ou processar dados em forma de fila.

O uso de generics permite definir o tipo de dado armazenado em uma coleção, como:

`ArrayList<String>`, `HashSet<Integer>` e `HashMap<Integer, String>`.

Diferentemente de um array, estruturas como `ArrayList` podem aumentar ou diminuir de tamanho conforme elementos são adicionados ou removidos.
