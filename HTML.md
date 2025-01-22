# cheat-sheet
Principais CHEAT-SHEET DA PROGRAMAÇÃO
### **HTML Cheat-Sheet: Principais Propriedades e Atributos**

#### **Estrutura Básica**
```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>
</head>
<body>
    <!-- Conteúdo vai aqui -->
</body>
</html>
```

---

### **Principais Tags e Seus Atributos**

#### **Tags Estruturais**
- `<html lang="pt-BR">`  
  - **lang**: Define o idioma do documento.
  
- `<head>`  
  - Contém metadados da página (não visíveis no navegador).
  
- `<body>`  
  - Contém o conteúdo visível.

#### **Metadados**
- `<meta>`  
  - **charset**: Define a codificação (ex.: `UTF-8`).  
  - **name**: Especifica o tipo de metadado (ex.: `viewport`).  
  - **content**: Define valores para o metadado.

#### **Textos e Cabeçalhos**
- `<h1> a <h6>`: Cabeçalhos (h1 é o maior, h6 o menor).  
- `<p>`: Parágrafo.  
- `<span>`: Container inline para estilização.  
- `<strong>`: Texto em negrito (semântico).  
- `<em>`: Texto em itálico (semântico).  
- `<br>`: Quebra de linha.  

#### **Links**
- `<a href="URL" target="_blank">Texto</a>`  
  - **href**: Define o destino do link.  
  - **target**: Define como abrir o link (`_blank`, `_self`).

#### **Imagens**
- `<img src="URL" alt="Descrição" width="300" height="200">`  
  - **src**: Caminho da imagem.  
  - **alt**: Texto alternativo (acessibilidade).  
  - **width** e **height**: Dimensões da imagem.

#### **Listas**
- `<ul>`: Lista não ordenada.  
- `<ol>`: Lista ordenada.  
- `<li>`: Item da lista.

#### **Tabelas**
```html
<table>
    <thead>
        <tr><th>Coluna 1</th><th>Coluna 2</th></tr>
    </thead>
    <tbody>
        <tr><td>Item 1</td><td>Item 2</td></tr>
    </tbody>
</table>
```
- **thead**: Cabeçalho.  
- **tbody**: Corpo.  
- **tr**: Linha.  
- **th**: Célula de cabeçalho.  
- **td**: Célula comum.

#### **Formulários**
```html
<form action="/submit" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" required>
    <button type="submit">Enviar</button>
</form>
```
- **action**: URL de envio.  
- **method**: `GET` ou `POST`.  
- `<input>`: Campo de entrada.  
  - **type**: Define o tipo (`text`, `email`, `password`, etc.).  
  - **required**: Campo obrigatório.  
- `<button>`: Botão.

#### **Multimídia**
- `<audio controls src="audio.mp3"></audio>`  
  - **controls**: Mostra controles de reprodução.  
- `<video controls width="640" height="360" src="video.mp4"></video>`  

#### **Semântica**
- `<header>`: Cabeçalho da página/seção.  
- `<footer>`: Rodapé.  
- `<article>`: Conteúdo independente.  
- `<section>`: Seção do documento.  
- `<aside>`: Conteúdo relacionado.  
- `<nav>`: Navegação.

---

### **Atributos Globais**
- **id**: Identificador único.  
- **class**: Classe para estilização ou comportamento.  
- **style**: CSS inline.  
- **title**: Texto de dica ao passar o mouse.  
- **hidden**: Oculta o elemento.  
- **data-*:** Atributos personalizados para dados.

---

### **Atributos de Acessibilidade**
- **alt**: Descrição de imagens para leitores de tela.  
- **aria-label**: Fornece uma descrição para elementos interativos.  
- **role**: Define o papel de um elemento (ex.: `button`, `navigation`).  
- **tabindex**: Controla a ordem de navegação pelo teclado.  
- **aria-hidden**: Esconde elementos de tecnologias assistivas.

---

### **Boas Práticas**
1. **Usar Tags Semânticas**: Priorize elementos como `<header>`, `<footer>`, `<main>` e `<article>` para melhorar acessibilidade e SEO.
2. **Manter Código Limpo**: Evite estilos inline e prefira CSS externo.
3. **Alt e Aria**: Sempre forneça descrições adequadas para imagens e elementos interativos.
4. **Validação**: Utilize ferramentas como [W3C Validator](https://validator.w3.org/) para verificar erros no HTML.
5. **Responsividade**: Sempre inclua `<meta name="viewport" content="width=device-width, initial-scale=1.0">` para otimizar em dispositivos móveis.

---

### **Tópicos Avançados**

#### **HTML5 Canvas**
Usado para desenhar gráficos, animações e outros conteúdos dinâmicos.
```html
<canvas id="meuCanvas" width="400" height="300"></canvas>
<script>
    const canvas = document.getElementById('meuCanvas');
    const ctx = canvas.getContext('2d');
    ctx.fillStyle = 'blue';
    ctx.fillRect(50, 50, 100, 100); // Desenha um quadrado azul
</script>
```

---

#### **Elementos para APIs**
- `<script>`: Carrega e executa JavaScript.
  ```html
  <script src="app.js"></script>
  ```
- `<link>`: Inclui recursos externos, como CSS ou fontes.
  ```html
  <link rel="stylesheet" href="styles.css">
  ```
- `<meta>`: Define dados para integração (ex.: Open Graph, SEO).
  ```html
  <meta property="og:title" content="Título da Página">
  ```

---

#### **Formulários Avançados**
1. **Campos de Arquivo**
   ```html
   <input type="file" name="arquivo" accept=".png, .jpg">
   ```
   - **accept**: Restringe tipos de arquivos.

2. **Campos de Data**
   ```html
   <input type="date" name="data">
   ```

3. **Validação Personalizada**
   ```html
   <input type="text" pattern="[A-Za-z]{3,}" title="Apenas letras, mínimo 3 caracteres">
   ```

4. **Campos Ocultos**
   ```html
   <input type="hidden" name="token" value="12345">
   ```

---

#### **Multimídia Avançada**
1. **Legendas em Vídeos**
   ```html
   <video controls>
       <source src="video.mp4" type="video/mp4">
       <track src="legendas.vtt" kind="subtitles" srclang="pt" label="Português">
   </video>
   ```

2. **Embed de Conteúdo Externo**
   ```html
   <iframe src="https://www.youtube.com/embed/ID_DO_VIDEO" width="560" height="315" allowfullscreen></iframe>
   ```

---

#### **Elementos Customizados**
Com o uso de **Web Components**, você pode criar seus próprios elementos.
```html
<meu-componente></meu-componente>
<script>
    class MeuComponente extends HTMLElement {
        connectedCallback() {
            this.innerHTML = '<p>Componente Customizado</p>';
        }
    }
    customElements.define('meu-componente', MeuComponente);
</script>
```

---

#### **Propriedades de SEO**
- **Meta Tags Essenciais**
  ```html
  <meta name="description" content="Descrição da página">
  <meta name="keywords" content="HTML, SEO, Exemplo">
  <meta name="author" content="Seu Nome">
  ```
- **Estrutura Semântica**
  Use `<header>`, `<nav>`, `<main>` e `<footer>` para melhorar o ranqueamento.

---

