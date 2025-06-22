# Calculador de Desconto Simples

Este é um programa Java muito simples que calcula um desconto sobre um determinado preço, aplicando taxas de desconto diferentes dependendo do valor do preço.

## Descrição

O programa define um preço base e, em seguida, calcula um desconto com base na seguinte regra:

* Se o preço for menor que R$ 20.00, um desconto de 10% é aplicado.
* Caso contrário (se o preço for R$ 20.00 ou maior), um desconto de 5% é aplicado.

O programa então imprime o valor do desconto calculado no console.

## Como Executar

Para executar este código, você precisará ter o Java Development Kit (JDK) instalado em seu sistema. Siga os passos abaixo:

1.  **Salve o código:** Salve o código Java fornecido em um arquivo chamado `Main.java` dentro de uma pasta chamada `principal`. Certifique-se de que a estrutura de pastas seja `principal/Main.java`.
2.  **Compile o código:** Abra um terminal ou prompt de comando, navegue até a pasta onde você salvou o arquivo `principal` e execute o seguinte comando para compilar o código:

    ```bash
    javac principal/Main.java
    ```

    Isso criará um arquivo chamado `Main.class` dentro da pasta `principal`.

3.  **Execute o programa:** No mesmo terminal ou prompt de comando, execute o programa com o seguinte comando:

    ```bash
    java principal.Main
    ```

    O valor do desconto será impresso diretamente no console.

## Como Usar

1.  Compile e execute o programa conforme as instruções acima.
2.  Ao executar, você verá a seguinte saída no console:

    ```
    Desconto: X.XX
    ```

    Onde `X.XX` será o valor do desconto calculado (neste caso, com o preço inicial de 34.5, o desconto será de 5% desse valor).

**Observação:** O preço base está definido diretamente no código. Para calcular o desconto para diferentes preços, você precisará modificar o valor da variável `preco` no arquivo `Main.java` e recompilar o programa.

## Explicação do Código

* `package principal;`: Declara o pacote ao qual a classe `Main` pertence.
* `public class Main { ... }`: Define a classe principal do programa.
* `public static void main(String[] args) { ... }`: O método principal onde a execução do programa começa.
* `double preco = 34.5;`: Declara e inicializa uma variável chamada `preco` com o valor de 34.5.
* `double desconto = (preco < 20.0) ? preco * 0.1 : preco * 0.05;`: Esta linha utiliza o operador ternário para calcular o desconto:
    * `(preco < 20.0)`: Verifica se o preço é menor que 20.0.
    * `? preco * 0.1`: Se a condição for verdadeira, o desconto é calculado como 10% do preço.
    * `: preco * 0.05`: Se a condição for falsa, o desconto é calculado como 5% do preço.
* `System.out.println("Desconto: " + desconto);`: Imprime a mensagem "Desconto:" seguida do valor calculado do desconto no console.
