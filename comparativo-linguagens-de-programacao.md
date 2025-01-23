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
