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
