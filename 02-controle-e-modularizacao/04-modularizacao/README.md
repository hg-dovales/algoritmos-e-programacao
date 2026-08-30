A **modularização** consiste em dividir um programa em partes menores e organizadas, chamadas de **métodos**, permitindo separar responsabilidades e facilitar a compreensão, manutenção e reutilização do código.

Um método pode receber informações através de **parâmetros**:

    static int calcularDobro(int numero) {
        return numero * 2;
    }

O **parâmetro** é a variável declarada na definição do método, enquanto o **argumento** é o valor fornecido no momento da chamada:

    int resultado = calcularDobro(10);

Nesse exemplo:

- `numero` é o parâmetro;
- `10` é o argumento;
- `resultado` recebe o valor retornado pelo método.

Métodos que precisam produzir um resultado possuem um **tipo de retorno** e utilizam `return`:

    static double calcularArea(double base, double altura) {
        double area = base * altura;
        return area;
    }

O `return` devolve um valor para o local onde o método foi chamado e também encerra a execução daquele método.

Quando um método realiza apenas uma ação e não precisa devolver um valor, podemos utilizar `void`:

    static void exibirMensagem(String mensagem) {
        System.out.println(mensagem);
    }

Cada método possui seu próprio **escopo**. Uma variável criada dentro de um método é uma variável local e não pode ser acessada diretamente por outros métodos.

Os dados necessários podem ser enviados de um método para outro através de argumentos e parâmetros.

Um método também pode chamar outro método:

    static double calcularPrecoFinal(double preco) {
        double desconto = calcularDesconto(preco);
        return preco - desconto;
    }

A **decomposição** consiste em dividir um problema maior em problemas menores, fazendo com que cada método tenha uma responsabilidade clara.

A **reutilização de código** permite utilizar o mesmo método várias vezes sem repetir sua implementação.

Essa ideia está relacionada ao princípio **DRY (Don't Repeat Yourself)**, que busca evitar duplicações desnecessárias de código.

A modularização permite construir programas mais organizados, dividindo a solução em pequenas partes que podem trabalhar em conjunto:

    Problema maior
          ↓
    Decomposição
          ↓
    Métodos menores
          ↓
    Cada método possui uma responsabilidade
          ↓
    Métodos trabalham em conjunto
          ↓
    Solução completa

Dessa forma, métodos ajudam a tornar o código mais **organizado, reutilizável, compreensível e fácil de manter**.
