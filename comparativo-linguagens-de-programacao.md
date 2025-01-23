Aqui está uma cheat-sheet de lógica de programação, com conceitos básicos e exemplos para cada item, incluindo uma comparação entre linguagens de programação (Java, Javascript e Python):

---

### 1. **Estruturas de Controle**

- **Condicionais (if, else)**:
  - **Conceito**: Executa blocos de código com base em condições.
  - **Exemplo**:
    ```c
    int idade = 20;
    if (idade >= 18) {
        printf("Maior de idade");
    } else {
        printf("Menor de idade");
    }
    ```
Segue uma tabela comparativa explicando como o código fornecido seria implementado em **Java**, **JavaScript** e **Python**, com explicações detalhadas sobre a sintaxe de cada linguagem:

| **Aspecto**       | **Java**                                                                                   | **JavaScript**                                                                         | **Python**                                                                           |
|--------------------|-------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| **Declaração de variável** | `int idade = 20;`<br>- `int`: Tipo de dado (inteiro).<br>- `idade`: Nome da variável.<br>- `= 20`: Atribuição do valor 20.       | `let idade = 20;`<br>- `let`: Declaração de variável.<br>- Sem especificar tipo (dinâmico).<br>- `= 20`: Atribuição.     | `idade = 20`<br>- Não há necessidade de especificar o tipo.<br>- Dinâmico, baseado no valor atribuído.                 |
| **Estrutura condicional** | `if (idade >= 18) {`<br>- `if`: Início da condição.<br>- `(idade >= 18)`: Testa se `idade` é maior ou igual a 18.<br>- `{}`: Delimita o bloco do código executado caso a condição seja verdadeira. | `if (idade >= 18) {`<br>- Semelhante ao Java.<br>- Usa parênteses e chaves para definir a condição e o bloco de código. | `if idade >= 18:`<br>- Não usa parênteses obrigatórios na condição.<br>- Dois pontos (`:`) indicam o início do bloco.  |
| **Bloco "então"** | `printf("Maior de idade");`<br>- `printf`: Função para exibir texto na saída.<br>- `("Maior de idade")`: Texto entre aspas duplas.         | `console.log("Maior de idade");`<br>- `console.log`: Função para exibir texto no console.<br>- Aspas duplas ou simples podem ser usadas. | `print("Maior de idade")`<br>- `print`: Função para exibir texto na saída.<br>- Aspas simples ou duplas podem ser usadas. |
| **Bloco "senão"** | `} else {`<br>- `else`: Indica o bloco alternativo, caso a condição seja falsa.<br>- `{}`: Delimita o bloco alternativo.                 | `} else {`<br>- Semelhante ao Java.<br>- Usa chaves para delimitar o bloco.          | `else:`<br>- Sem parênteses ou chaves.<br>- Dois pontos (`:`) indicam o início do bloco.                                |
| **Saída no bloco "senão"** | `printf("Menor de idade");`<br>- Mesma estrutura do bloco "então".                                                      | `console.log("Menor de idade");`<br>- Mesma estrutura do bloco "então".              | `print("Menor de idade")`<br>- Mesma estrutura do bloco "então".                                                        |

### Código completo em cada linguagem:

**Java**:
```java
int idade = 20;
if (idade >= 18) {
    System.out.println("Maior de idade");
} else {
    System.out.println("Menor de idade");
}
```

**JavaScript**:
```javascript
let idade = 20;
if (idade >= 18) {
    console.log("Maior de idade");
} else {
    console.log("Menor de idade");
}
```

**Python**:
```python
idade = 20
if idade >= 18:
    print("Maior de idade")
else:
    print("Menor de idade")
```

Essa tabela e os exemplos ajudam a entender as diferenças e semelhanças entre as linguagens, tornando mais fácil a adaptação para quem está iniciando.

---

### 2. **Laços de Repetição**

- **For**:
  - **Conceito**: Repeita um bloco de código um número fixo de vezes.
  - **Exemplo**:
    ```c
    for (int i = 0; i < 5; i++) {
        printf("%d\n", i);  // Imprime 0 a 4
    }
    
    ```
Segue a análise comparativa do código fornecido em **Java**, **JavaScript** e **Python**, detalhando a sintaxe do **laço `for`**:

| **Aspecto**             | **Java**                                                                                     | **JavaScript**                                                                           | **Python**                                                                                   |
|--------------------------|---------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| **Declaração do laço**   | `for (int i = 0; i < 5; i++) {`<br>- `for`: Início do laço.<br>- `(int i = 0;`: Declaração e inicialização da variável `i`.<br>- `i < 5;`: Condição de execução.<br>- `i++`: Incremento da variável após cada iteração. | `for (let i = 0; i < 5; i++) {`<br>- Semelhante ao Java.<br>- Usa `let` (ou `var`, `const`) para declarar `i`.<br>- Estrutura do laço idêntica. | `for i in range(5):`<br>- `for`: Início do laço.<br>- `i in range(5)`: Itera valores de `0` a `4`.<br>- Não precisa de inicialização, condição ou incremento separados. |
| **Bloco de código**      | `{ printf("%d\\n", i); }`<br>- `{}`: Delimita o bloco do laço.<br>- `printf("%d\\n", i);`: Imprime o valor atual de `i` com quebra de linha. | `{ console.log(i); }`<br>- `{}`: Delimita o bloco.<br>- `console.log(i);`: Exibe o valor de `i` no console. | `print(i)`<br>- Bloco definido pela indentação.<br>- `print(i)`: Imprime o valor atual de `i` com quebra de linha automática. |
| **Incremento**           | `i++`: Incrementa `i` em 1 após cada iteração.                                              | `i++`: Incrementa `i` em 1 após cada iteração.                                           | O incremento é gerenciado automaticamente pelo `range()`.                                    |
| **Faixa de valores**     | De 0 a 4. O laço termina quando `i` não atende mais à condição (`i < 5`).                    | De 0 a 4. O laço termina quando `i` não atende mais à condição (`i < 5`).                | `range(5)` gera os valores de 0 a 4 automaticamente.                                        |

### Código completo em cada linguagem:

**Java**:
```java
for (int i = 0; i < 5; i++) {
    System.out.printf("%d\n", i);  // Imprime 0 a 4
}
```

**JavaScript**:
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);  // Imprime 0 a 4
}
```

**Python**:
```python
for i in range(5):
    print(i)  # Imprime 0 a 4
```

### Observações:
1. **Java** e **JavaScript** utilizam uma estrutura de laço `for` tradicional, que inclui três partes: inicialização, condição e incremento.
2. **Python** simplifica o laço com o uso do `range()`, que gera a sequência de valores automaticamente.
3. Em todas as linguagens, o laço itera de 0 a 4, pois a condição de parada ou o intervalo exclui o limite superior (5).


- **While**:
  - **Conceito**: Repete um bloco de código enquanto a condição for verdadeira.
  - **Exemplo**:
    ```c
    int i = 0;
    while (i < 5) {
        printf("%d\n", i);  // Imprime 0 a 4
        i++;
    }

    
    ```

- **Do While**:
  - **Conceito**: Repete um bloco de código ao menos uma vez e continua enquanto a condição for verdadeira.
  - **Exemplo**:
    ```c
    int i = 0;
    do {
        printf("%d\n", i);  // Imprime 0 a 4
        i++;
    } while (i < 5);
    ```

---

### 3. **Operadores Aritméticos**

- **Conceito**: Usados para realizar operações matemáticas.
- **Exemplo**:
  ```c
  int a = 10, b = 5;
  printf("%d\n", a + b);  // 15 (soma)
  printf("%d\n", a - b);  // 5  (subtração)
  printf("%d\n", a * b);  // 50 (multiplicação)
  printf("%d\n", a / b);  // 2  (divisão)
  printf("%d\n", a % b);  // 0  (módulo)
  ```

---

### 4. **Operadores Lógicos**

- **Conceito**: Usados para combinar condições booleanas.
- **Exemplo**:
  ```c
  int a = 1, b = 0;
  if (a && b) {
      printf("Verdadeiro");
  } else {
      printf("Falso");
  }
  ```

---

### 5. **Operadores Relacionais**

- **Conceito**: Usados para comparar valores.
- **Exemplo**:
  ```c
  int a = 5, b = 10;
  if (a == b) {
      printf("São iguais");
  } else {
      printf("São diferentes");
  }
  ```

---

### 6. **Funções**

- **Conceito**: Blocos de código que podem ser chamados para realizar uma tarefa específica.
- **Exemplo**:
  ```c
  int soma(int a, int b) {
      return a + b;
  }

  int resultado = soma(3, 4);  // Chama a função soma
  printf("%d", resultado);     // 7
  ```

---

### 7. **Vetores/Arrays**

- **Conceito**: Estruturas que armazenam múltiplos valores do mesmo tipo.
- **Exemplo**:
  ```c
  int arr[5] = {1, 2, 3, 4, 5};
  printf("%d", arr[2]);  // Acessa o valor 3
  ```

---

### 8. **Entrada e Saída**

- **Entrada (scanf)**:
  - **Conceito**: Recebe dados do usuário.
  - **Exemplo**:
    ```c
    int idade;
    printf("Digite sua idade: ");
    scanf("%d", &idade);
    ```

- **Saída (printf)**:
  - **Conceito**: Exibe informações para o usuário.
  - **Exemplo**:
    ```c
    printf("Olá, Mundo!");
    ```

---

### 9. **Recursão**

- **Conceito**: Função que chama a si mesma para resolver problemas menores.
- **Exemplo**:
  ```c
  int fatorial(int n) {
      if (n == 0) return 1;
      return n * fatorial(n - 1);
  }
  printf("%d", fatorial(5));  // 120
  ```

---

### 10. **Ponteiros**

- **Conceito**: Variáveis que armazenam o endereço de outra variável.
- **Exemplo**:
  ```c
  int x = 10;
  int *p = &x;  // p armazena o endereço de x
  printf("%d", *p);  // Acessa o valor de x através de p (10)
  ```

---

### 11. **Estruturas (Structs)**

- **Conceito**: Agrupamento de variáveis de diferentes tipos.
- **Exemplo**:
  ```c
  struct Pessoa {
      char nome[50];
      int idade;
  };

  struct Pessoa p1 = {"João", 25};
  printf("%s tem %d anos", p1.nome, p1.idade);
  ```

---

### 12. **Busca Linear**

- **Conceito**: Pesquisa elemento por elemento em uma lista.
- **Exemplo**:
  ```c
  int arr[] = {1, 3, 5, 7, 9};
  int target = 5;
  for (int i = 0; i < 5; i++) {
      if (arr[i] == target) {
          printf("Elemento encontrado na posição %d", i);
          break;
      }
  }
  ```

---

### 13. **Busca Binária**

- **Conceito**: Pesquisa em um vetor ordenado, dividindo o espaço de busca ao meio.
- **Exemplo**:
  ```c
  int arr[] = {1, 3, 5, 7, 9};
  int target = 5;
  int inicio = 0, fim = 4, meio;
  while (inicio <= fim) {
      meio = (inicio + fim) / 2;
      if (arr[meio] == target) {
          printf("Elemento encontrado na posição %d", meio);
          break;
      } else if (arr[meio] < target) {
          inicio = meio + 1;
      } else {
          fim = meio - 1;
      }
  }
  ```

---

### 14. **Ordenação (Bubble Sort)**

- **Conceito**: Ordena elementos trocando valores adjacentes.
- **Exemplo**:
  ```c
  int arr[] = {5, 2, 9, 1, 5, 6};
  for (int i = 0; i < 6-1; i++) {
      for (int j = 0; j < 6-i-1; j++) {
          if (arr[j] > arr[j+1]) {
              int temp = arr[j];
              arr[j] = arr[j+1];
              arr[j+1] = temp;
          }
      }
  }
  ```

---

Esta cheat-sheet cobre os conceitos básicos de lógica de programação com exemplos práticos em C. Ela é útil para revisar rapidamente os fundamentos e entender como aplicar cada conceito.

### 15. **Estruturas de Dados - Pilha (Stack)**

- **Conceito**: Estrutura de dados onde o último elemento inserido é o primeiro a ser removido (LIFO - Last In, First Out).
- **Exemplo**:
  ```c
  #include <stdio.h>
  #define MAX 5

  int pilha[MAX], topo = -1;

  void push(int valor) {
      if (topo == MAX - 1) {
          printf("Pilha cheia!\n");
      } else {
          pilha[++topo] = valor;
      }
  }

  int pop() {
      if (topo == -1) {
          printf("Pilha vazia!\n");
          return -1;
      } else {
          return pilha[topo--];
      }
  }

  int main() {
      push(10);
      push(20);
      printf("Removido: %d\n", pop());  // 20
      return 0;
  }
  ```

---

### 16. **Estruturas de Dados - Fila (Queue)**

- **Conceito**: Estrutura de dados onde o primeiro elemento inserido é o primeiro a ser removido (FIFO - First In, First Out).
- **Exemplo**:
  ```c
  #include <stdio.h>
  #define MAX 5

  int fila[MAX], inicio = 0, fim = 0;

  void enqueue(int valor) {
      if ((fim + 1) % MAX == inicio) {
          printf("Fila cheia!\n");
      } else {
          fila[fim] = valor;
          fim = (fim + 1) % MAX;
      }
  }

  int dequeue() {
      if (inicio == fim) {
          printf("Fila vazia!\n");
          return -1;
      } else {
          int valor = fila[inicio];
          inicio = (inicio + 1) % MAX;
          return valor;
      }
  }

  int main() {
      enqueue(10);
      enqueue(20);
      printf("Removido: %d\n", dequeue());  // 10
      return 0;
  }
  ```

---

### 17. **Estruturas Condicionais - Switch Case**

- **Conceito**: Avalia uma variável e executa diferentes blocos de código com base no valor.
- **Exemplo**:
  ```c
  int dia = 3;
  switch (dia) {
      case 1:
          printf("Domingo");
          break;
      case 2:
          printf("Segunda-feira");
          break;
      case 3:
          printf("Terça-feira");
          break;
      default:
          printf("Dia inválido");
  }
  ```

---

### 18. **Matrizes (Arrays Multidimensionais)**

- **Conceito**: Arrays que possuem mais de uma dimensão.
- **Exemplo**:
  ```c
  int matriz[2][3] = {
      {1, 2, 3},
      {4, 5, 6}
  };

  for (int i = 0; i < 2; i++) {
      for (int j = 0; j < 3; j++) {
          printf("%d ", matriz[i][j]);
      }
      printf("\n");
  }
  ```

---

### 19. **Ordenação (Insertion Sort)**

- **Conceito**: Ordena elementos inserindo-os em suas posições corretas em uma sublista ordenada.
- **Exemplo**:
  ```c
  int arr[] = {5, 2, 4, 6, 1, 3};
  int n = 6;

  for (int i = 1; i < n; i++) {
      int chave = arr[i];
      int j = i - 1;

      while (j >= 0 && arr[j] > chave) {
          arr[j + 1] = arr[j];
          j--;
      }
      arr[j + 1] = chave;
  }

  for (int i = 0; i < n; i++) {
      printf("%d ", arr[i]);  // 1 2 3 4 5 6
  }
  ```

---

### 20. **Estruturas de Repetição Aninhadas**

- **Conceito**: Estruturas de repetição dentro de outras.
- **Exemplo**:
  ```c
  for (int i = 1; i <= 3; i++) {
      for (int j = 1; j <= 3; j++) {
          printf("i=%d, j=%d\n", i, j);
      }
  }
  ```

---

### 21. **Manipulação de Strings**

- **Conceito**: Trabalhar com sequências de caracteres.
- **Exemplo**:
  ```c
  #include <stdio.h>
  #include <string.h>

  int main() {
      char str1[50] = "Olá, ";
      char str2[] = "Mundo!";
      strcat(str1, str2);
      printf("%s", str1);  // Olá, Mundo!
      return 0;
  }
  ```

---

Essa continuação complementa a cheat-sheet com conceitos mais avançados e exemplos úteis para a aplicação prática. Se precisar de mais detalhes ou outros tópicos, é só pedir!

### 22. **Algoritmo de Busca Sequencial**

- **Conceito**: Pesquisa elemento por elemento em uma lista não ordenada até encontrar o valor desejado.
- **Exemplo**:
  ```c
  int buscaSequencial(int arr[], int n, int valor) {
      for (int i = 0; i < n; i++) {
          if (arr[i] == valor) {
              return i;  // Retorna a posição do elemento
          }
      }
      return -1;  // Retorna -1 se não encontrar
  }

  int main() {
      int arr[] = {10, 20, 30, 40, 50};
      int posicao = buscaSequencial(arr, 5, 30);
      if (posicao != -1) {
          printf("Elemento encontrado na posição %d", posicao);
      } else {
          printf("Elemento não encontrado");
      }
      return 0;
  }
  ```

---

### 23. **Estruturas de Dados - Lista Encadeada**

- **Conceito**: Estrutura onde cada elemento (nó) contém um valor e um ponteiro para o próximo nó.
- **Exemplo**:
  ```c
  #include <stdio.h>
  #include <stdlib.h>

  struct Node {
      int data;
      struct Node* next;
  };

  void imprimeLista(struct Node* n) {
      while (n != NULL) {
          printf("%d -> ", n->data);
          n = n->next;
      }
      printf("NULL\n");
  }

  int main() {
      struct Node* head = NULL;
      struct Node* segundo = NULL;
      struct Node* terceiro = NULL;

      head = (struct Node*)malloc(sizeof(struct Node));
      segundo = (struct Node*)malloc(sizeof(struct Node));
      terceiro = (struct Node*)malloc(sizeof(struct Node));

      head->data = 1;
      head->next = segundo;

      segundo->data = 2;
      segundo->next = terceiro;

      terceiro->data = 3;
      terceiro->next = NULL;

      imprimeLista(head);
      return 0;
  }
  ```

---

### 24. **Ordenação (Selection Sort)**

- **Conceito**: Ordena elementos selecionando o menor valor e colocando-o na posição correta.
- **Exemplo**:
  ```c
  void selectionSort(int arr[], int n) {
      for (int i = 0; i < n - 1; i++) {
          int minIndex = i;
          for (int j = i + 1; j < n; j++) {
              if (arr[j] < arr[minIndex]) {
                  minIndex = j;
              }
          }
          int temp = arr[minIndex];
          arr[minIndex] = arr[i];
          arr[i] = temp;
      }
  }

  int main() {
      int arr[] = {64, 25, 12, 22, 11};
      int n = 5;
      selectionSort(arr, n);
      for (int i = 0; i < n; i++) {
          printf("%d ", arr[i]);  // 11 12 22 25 64
      }
      return 0;
  }
  ```

---

### 25. **Estruturas de Dados - Árvores**

- **Conceito**: Estrutura hierárquica onde cada nó tem um valor e pode ter filhos (subárvores).
- **Exemplo**:
  ```c
  #include <stdio.h>
  #include <stdlib.h>

  struct Node {
      int data;
      struct Node* left;
      struct Node* right;
  };

  struct Node* novoNode(int data) {
      struct Node* node = (struct Node*)malloc(sizeof(struct Node));
      node->data = data;
      node->left = NULL;
      node->right = NULL;
      return node;
  }

  void preOrder(struct Node* root) {
      if (root != NULL) {
          printf("%d ", root->data);
          preOrder(root->left);
          preOrder(root->right);
      }
  }

  int main() {
      struct Node* root = novoNode(1);
      root->left = novoNode(2);
      root->right = novoNode(3);
      root->left->left = novoNode(4);
      root->left->right = novoNode(5);

      printf("Pré-Ordem: ");
      preOrder(root);  // 1 2 4 5 3
      return 0;
  }
  ```

---

### 26. **Algoritmo de Ordenação (Merge Sort)**

- **Conceito**: Divide a lista em partes menores, ordena cada parte e depois combina.
- **Exemplo**:
  ```c
  void merge(int arr[], int l, int m, int r) {
      int n1 = m - l + 1;
      int n2 = r - m;
      int L[n1], R[n2];

      for (int i = 0; i < n1; i++) L[i] = arr[l + i];
      for (int j = 0; j < n2; j++) R[j] = arr[m + 1 + j];

      int i = 0, j = 0, k = l;
      while (i < n1 && j < n2) {
          if (L[i] <= R[j]) arr[k++] = L[i++];
          else arr[k++] = R[j++];
      }

      while (i < n1) arr[k++] = L[i++];
      while (j < n2) arr[k++] = R[j++];
  }

  void mergeSort(int arr[], int l, int r) {
      if (l < r) {
          int m = l + (r - l) / 2;
          mergeSort(arr, l, m);
          mergeSort(arr, m + 1, r);
          merge(arr, l, m, r);
      }
  }

  int main() {
      int arr[] = {12, 11, 13, 5, 6, 7};
      int n = 6;
      mergeSort(arr, 0, n - 1);
      for (int i = 0; i < n; i++) {
          printf("%d ", arr[i]);  // 5 6 7 11 12 13
      }
      return 0;
  }
  ```

---


### 27. **Algoritmo de Busca Binária**

- **Conceito**: Pesquisa eficiente em uma lista ordenada, dividindo-a em metades para encontrar o valor desejado.
- **Exemplo**:
  ```c
  int buscaBinaria(int arr[], int n, int valor) {
      int inicio = 0, fim = n - 1;
      while (inicio <= fim) {
          int meio = inicio + (fim - inicio) / 2;
          if (arr[meio] == valor) {
              return meio;  // Elemento encontrado
          }
          if (arr[meio] < valor) {
              inicio = meio + 1;
          } else {
              fim = meio - 1;
          }
      }
      return -1;  // Elemento não encontrado
  }

  int main() {
      int arr[] = {10, 20, 30, 40, 50};
      int posicao = buscaBinaria(arr, 5, 30);
      if (posicao != -1) {
          printf("Elemento encontrado na posição %d", posicao);
      } else {
          printf("Elemento não encontrado");
      }
      return 0;
  }
  ```

---

### 28. **Recursão**

- **Conceito**: Função que chama a si mesma para resolver problemas menores de forma iterativa.
- **Exemplo**:
  ```c
  int fatorial(int n) {
      if (n == 0 || n == 1) {
          return 1;  // Caso base
      }
      return n * fatorial(n - 1);  // Chamada recursiva
  }

  int main() {
      int numero = 5;
      printf("Fatorial de %d é %d", numero, fatorial(numero));  // 120
      return 0;
  }
  ```

---

### 29. **Algoritmo de Ordenação (Quick Sort)**

- **Conceito**: Escolhe um elemento como pivô, particiona a lista em menores e maiores que o pivô e ordena recursivamente.
- **Exemplo**:
  ```c
  void troca(int* a, int* b) {
      int temp = *a;
      *a = *b;
      *b = temp;
  }

  int particiona(int arr[], int baixo, int alto) {
      int pivô = arr[alto];
      int i = baixo - 1;

      for (int j = baixo; j < alto; j++) {
          if (arr[j] < pivô) {
              i++;
              troca(&arr[i], &arr[j]);
          }
      }
      troca(&arr[i + 1], &arr[alto]);
      return i + 1;
  }

  void quickSort(int arr[], int baixo, int alto) {
      if (baixo < alto) {
          int pi = particiona(arr, baixo, alto);
          quickSort(arr, baixo, pi - 1);
          quickSort(arr, pi + 1, alto);
      }
  }

  int main() {
      int arr[] = {10, 7, 8, 9, 1, 5};
      int n = 6;
      quickSort(arr, 0, n - 1);
      for (int i = 0; i < n; i++) {
          printf("%d ", arr[i]);  // 1 5 7 8 9 10
      }
      return 0;
  }
  ```

---

### 30. **Estruturas de Dados - Tabela Hash**

- **Conceito**: Estrutura que associa chaves a valores usando uma função de hash para mapeamento.
- **Exemplo**:
  ```c
  #include <stdio.h>
  #include <stdlib.h>

  #define TAMANHO 10

  struct Node {
      int chave;
      int valor;
      struct Node* proximo;
  };

  struct Node* tabelaHash[TAMANHO];

  int hash(int chave) {
      return chave % TAMANHO;
  }

  void insere(int chave, int valor) {
      int indice = hash(chave);
      struct Node* novoNode = (struct Node*)malloc(sizeof(struct Node));
      novoNode->chave = chave;
      novoNode->valor = valor;
      novoNode->proximo = tabelaHash[indice];
      tabelaHash[indice] = novoNode;
  }

  int busca(int chave) {
      int indice = hash(chave);
      struct Node* temp = tabelaHash[indice];
      while (temp != NULL) {
          if (temp->chave == chave) {
              return temp->valor;
          }
          temp = temp->proximo;
      }
      return -1;  // Não encontrado
  }

  int main() {
      insere(1, 10);
      insere(2, 20);
      insere(11, 30);
      printf("Valor para chave 11: %d\n", busca(11));  // 30
      return 0;
  }
  ```

---

### 27. **Algoritmo de Busca Binária**

- **Conceito**: Pesquisa eficiente em uma lista ordenada, dividindo-a em metades para encontrar o valor desejado.
- **Exemplo**:
  ```c
  int buscaBinaria(int arr[], int n, int valor) {
      int inicio = 0, fim = n - 1;
      while (inicio <= fim) {
          int meio = inicio + (fim - inicio) / 2;
          if (arr[meio] == valor) {
              return meio;  // Elemento encontrado
          }
          if (arr[meio] < valor) {
              inicio = meio + 1;
          } else {
              fim = meio - 1;
          }
      }
      return -1;  // Elemento não encontrado
  }

  int main() {
      int arr[] = {10, 20, 30, 40, 50};
      int posicao = buscaBinaria(arr, 5, 30);
      if (posicao != -1) {
          printf("Elemento encontrado na posição %d", posicao);
      } else {
          printf("Elemento não encontrado");
      }
      return 0;
  }
  ```

---

### 28. **Recursão**

- **Conceito**: Função que chama a si mesma para resolver problemas menores de forma iterativa.
- **Exemplo**:
  ```c
  int fatorial(int n) {
      if (n == 0 || n == 1) {
          return 1;  // Caso base
      }
      return n * fatorial(n - 1);  // Chamada recursiva
  }

  int main() {
      int numero = 5;
      printf("Fatorial de %d é %d", numero, fatorial(numero));  // 120
      return 0;
  }
  ```

---

### 29. **Algoritmo de Ordenação (Quick Sort)**

- **Conceito**: Escolhe um elemento como pivô, particiona a lista em menores e maiores que o pivô e ordena recursivamente.
- **Exemplo**:
  ```c
  void troca(int* a, int* b) {
      int temp = *a;
      *a = *b;
      *b = temp;
  }

  int particiona(int arr[], int baixo, int alto) {
      int pivô = arr[alto];
      int i = baixo - 1;

      for (int j = baixo; j < alto; j++) {
          if (arr[j] < pivô) {
              i++;
              troca(&arr[i], &arr[j]);
          }
      }
      troca(&arr[i + 1], &arr[alto]);
      return i + 1;
  }

  void quickSort(int arr[], int baixo, int alto) {
      if (baixo < alto) {
          int pi = particiona(arr, baixo, alto);
          quickSort(arr, baixo, pi - 1);
          quickSort(arr, pi + 1, alto);
      }
  }

  int main() {
      int arr[] = {10, 7, 8, 9, 1, 5};
      int n = 6;
      quickSort(arr, 0, n - 1);
      for (int i = 0; i < n; i++) {
          printf("%d ", arr[i]);  // 1 5 7 8 9 10
      }
      return 0;
  }
  ```

---

### 30. **Estruturas de Dados - Tabela Hash**

- **Conceito**: Estrutura que associa chaves a valores usando uma função de hash para mapeamento.
- **Exemplo**:
  ```c
  #include <stdio.h>
  #include <stdlib.h>

  #define TAMANHO 10

  struct Node {
      int chave;
      int valor;
      struct Node* proximo;
  };

  struct Node* tabelaHash[TAMANHO];

  int hash(int chave) {
      return chave % TAMANHO;
  }

  void insere(int chave, int valor) {
      int indice = hash(chave);
      struct Node* novoNode = (struct Node*)malloc(sizeof(struct Node));
      novoNode->chave = chave;
      novoNode->valor = valor;
      novoNode->proximo = tabelaHash[indice];
      tabelaHash[indice] = novoNode;
  }

  int busca(int chave) {
      int indice = hash(chave);
      struct Node* temp = tabelaHash[indice];
      while (temp != NULL) {
          if (temp->chave == chave) {
              return temp->valor;
          }
          temp = temp->proximo;
      }
      return -1;  // Não encontrado
  }

  int main() {
      insere(1, 10);
      insere(2, 20);
      insere(11, 30);
      printf("Valor para chave 11: %d\n", busca(11));  // 30
      return 0;
  }
  ```

---
