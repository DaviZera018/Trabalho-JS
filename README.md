# Contagem de Valores Dentro de um Intervalo

## Descrição do Projeto

Este projeto em Java consiste em uma aplicação simples que conta quantos valores de um array de inteiros estão dentro de um intervalo definido. O intervalo é determinado pelo primeiro valor do array e um valor máximo (`N`) fornecido no código. A contagem considera o intervalo como inclusivo, ou seja, inclui os limites inferior e superior.

---

## Estrutura do Código

O programa é composto por uma única classe chamada `Contagem` e um método principal (`main`) que executa a lógica. Segue um resumo da funcionalidade:

1. **Definição do array e dos parâmetros do intervalo**:
   - Um array de inteiros chamado `dados` é definido.
   - O limite superior do intervalo (`N`) é definido como uma variável inteira.
   - O limite inferior do intervalo é o primeiro elemento do array (`primeiro`).

2. **Lógica da contagem**:
   - Uma variável chamada `contagem` é inicializada com o valor 0.
   - Um laço `for` percorre os elementos do array.
   - Para cada elemento, verifica-se se ele está dentro do intervalo `[primeiro, N]`.
   - Se estiver, o contador é incrementado.

3. **Exibição do resultado**:
   - O programa exibe o número de valores dentro do intervalo usando `System.out.println`.

---

## Exemplo de Funcionamento

### Código

```java
int[] dados = {1, 3, 5, 7, 9, 2, 8};
int N = 10;
```

- O array `dados` contém os números: `{1, 3, 5, 7, 9, 2, 8}`.
- O limite inferior (`primeiro`) é o primeiro elemento do array: `1`.
- O limite superior (`N`) é `10`.

### Lógica do Intervalo
O programa verificará quais valores no array estão entre `1` e `10`, inclusivamente. Nesse caso, todos os elementos do array atendem à condição.

### Resultado
O programa exibirá:
```
Número de valores entre 1 e 10 (inclusive): 7
```

---

## Personalização

1. **Alterar o array**:
   - Substituir os valores no array `dados` por outros valores para diferentes cenários.

2. **Modificar o intervalo**:
   - Alterar o valor de `N` para restringir ou expandir o intervalo superior.

---

## Utilidade

Este projeto é útil como exemplo introdutório de:
- Manipulação de arrays.
- Uso de laços `for` em Java.
- Estruturas condicionais para verificar intervalos.
- Trabalhar com contadores e variáveis acumuladoras.

Além disso, é um bom ponto de partida para desenvolver lógica para problemas mais complexos envolvendo filtros ou verificações em listas de dados.








# Gerador de Sequência de Fibonacci

## Descrição do Projeto

Este projeto é uma aplicação em Java que gera e exibe os primeiros `N` números da sequência de Fibonacci. A sequência de Fibonacci é uma série de números em que cada número (a partir do terceiro) é a soma dos dois anteriores. Os dois primeiros números da sequência são, por definição, 0 e 1.

---

## Estrutura do Código

O programa está organizado da seguinte forma:

### 1. **Definição do valor de `N`**
- A variável `N` determina a quantidade de números na sequência de Fibonacci que será gerada.
- Se `N` for menor ou igual a 1, o programa exibe uma mensagem de erro e termina.

### 2. **Inicialização do array**
- Um array chamado `fib` é criado para armazenar os números da sequência.
- Os dois primeiros valores são definidos diretamente:
  - `fib[0] = 0`
  - `fib[1] = 1`

### 3. **Cálculo da sequência**
- Um laço `for` é usado para preencher os valores restantes no array.
- Cada elemento a partir do índice 2 é calculado como:
  ```java
  fib[i] = fib[i - 1] + fib[i - 2];
  ```

### 4. **Exibição da sequência**
- Os números da sequência são exibidos no console, separados por espaços.

---

## Exemplo de Funcionamento

### Código
```java
int N = 10;
```

- O valor de `N` é definido como 10, ou seja, o programa gerará os 10 primeiros números da sequência de Fibonacci.

### Resultado
A saída no console será:
```
0 1 1 2 3 5 8 13 21 34
```

---

## Personalização

1. **Alterar o valor de `N`**:
   - Modifique a variável `N` para gerar mais ou menos números da sequência.

2. **Adaptar para outros usos**:
   - Modifique o código para salvar os números em um arquivo ou utilizá-los em outras operações matemáticas.

3. **Melhorar a exibição**:
   - Substituir o espaço entre os números por vírgulas ou exibi-los em formato de tabela.

---

## Utilidade

Este projeto é útil como exemplo de:
- Implementação da sequência de Fibonacci de forma iterativa.
- Uso de arrays para armazenar dados calculados.
- Manipulação básica de laços e condicionais em Java.

Também pode ser expandido para aprender técnicas mais avançadas, como:
- Implementar a sequência de Fibonacci de forma recursiva.
- Melhorar a eficiência para valores muito grandes usando estruturas como `BigInteger`.

---

## Considerações

A sequência de Fibonacci tem aplicações em diversas áreas, como:
- Matemática (exemplo: número áureo).
- Computação (exemplo: algoritmos de divisão e conquista).
- Natureza (exemplo: padrões de crescimento de plantas). 

Este projeto é um ótimo ponto de partida para explorar essas conexões.
