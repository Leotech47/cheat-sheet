Aqui está uma cheat-sheet de lógica de programação, com conceitos básicos e exemplos para cada item:

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

