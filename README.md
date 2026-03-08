# Sintaxe-em-Java-

Para colocar em prática os fundamentos da linguagem Java e entender as regras de sintaxe, aqui estão alguns conceitos essenciais, seguidos de exemplos:

# 1. Estrutura Básica de um Programa

Todo programa Java começa com uma classe. A seguir, um exemplo básico:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Olá, Mundo!");
    }
}
```

# 2. Variáveis e Tipos de Dados

Em Java, devemos declarar o tipo de dado da variável. Exemplos de tipos de dados incluem `int`, `double`, `char`, `boolean`, e `String`.

```java
public class Variaveis {
    public static void main(String[] args) {
        int numero = 10;
        double preco = 19.99;
        char letra = 'A';
        boolean ativo = true;
        String mensagem = "Hello, Java!";

        System.out.println(mensagem);
    }
}
```

# 3. Estruturas de Controle

# Condicional:
```java
public class Condicional {
    public static void main(String[] args) {
        int idade = 18;

        if (idade >= 18) {
            System.out.println("Você é maior de idade.");
        } else {
            System.out.println("Você é menor de idade.");
        }
    }
}
```

# Laços de Repetição:
```java
public class Repeticao {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            System.out.println("Contagem: " + i);
        }
    }
}
```

# 4. Métodos

Os métodos em Java permitem a reutilização de código. Aqui está um exemplo de método simples:

```java
public class Metodos {
    public static void main(String[] args) {
        int resultado = somar(5, 10);
        System.out.println("Resultado: " + resultado);
    }

    public static int somar(int a, int b) {
        return a + b;
    }
}
```

# 5. Classes e Objetos

Java é uma linguagem orientada a objetos. Aqui está um exemplo de como criar uma classe e um objeto:

```java
class Carro {
    String modelo;
    int ano;

    public void exibirDetalhes() {
        System.out.println("Modelo: " + modelo + ", Ano: " + ano);
    }
}

public class Main {
    public static void main(String[] args) {
        Carro meuCarro = new Carro();
        meuCarro.modelo = "Fusca";
        meuCarro.ano = 1976;
        meuCarro.exibirDetalhes();
    }
}
```

# 6. Conceitos de Encapsulamento

Para proteger os dados de uma classe:

```java
class ContaBancaria {
    private double saldo;

    public void depositar(double valor) {
        saldo += valor;
    }

    public double getSaldo() {
        return saldo;
    }
}

public class Main {
    public static void main(String[] args) {
        ContaBancaria conta = new ContaBancaria();
        conta.depositar(100.50);
        System.out.println("Saldo: " + conta.getSaldo());
    }
}
```
