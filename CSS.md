### **CSS Cheat-Sheet: Principais Propriedades**

#### **1. Propriedades de Texto**
- **`color`**: Define a cor do texto.  
  Exemplo: `color: blue;`
  
- **`font-size`**: Define o tamanho da fonte.  
  Exemplo: `font-size: 16px;`
  
- **`font-family`**: Define a família da fonte.  
  Exemplo: `font-family: Arial, sans-serif;`
  
- **`font-weight`**: Define a espessura da fonte.  
  Valores: `normal`, `bold`, `lighter`, números (100-900).  
  Exemplo: `font-weight: bold;`
  
- **`line-height`**: Define o espaçamento entre linhas.  
  Exemplo: `line-height: 1.5;`
  
- **`text-align`**: Alinha o texto horizontalmente.  
  Valores: `left`, `right`, `center`, `justify`.  
  Exemplo: `text-align: center;`
  
- **`text-decoration`**: Define estilos como sublinhado.  
  Valores: `none`, `underline`, `line-through`.  
  Exemplo: `text-decoration: underline;`
  
- **`letter-spacing`**: Define o espaçamento entre letras.  
  Exemplo: `letter-spacing: 2px;`

---

#### **2. Propriedades de Cor e Fundo**
- **`background-color`**: Define a cor de fundo.  
  Exemplo: `background-color: #f0f0f0;`
  
- **`background-image`**: Define uma imagem de fundo.  
  Exemplo: `background-image: url('imagem.jpg');`
  
- **`background-size`**: Ajusta o tamanho do fundo.  
  Valores: `cover`, `contain`, dimensões específicas.  
  Exemplo: `background-size: cover;`
  
- **`background-position`**: Define a posição do fundo.  
  Valores: `center`, `top`, `bottom`, `left`, `right`.  
  Exemplo: `background-position: center;`
  
- **`background-repeat`**: Define a repetição do fundo.  
  Valores: `repeat`, `no-repeat`, `repeat-x`, `repeat-y`.  
  Exemplo: `background-repeat: no-repeat;`

---

#### **3. Propriedades de Layout**
- **`width`**: Define a largura do elemento.  
  Exemplo: `width: 100%;`
  
- **`height`**: Define a altura do elemento.  
  Exemplo: `height: 50px;`
  
- **`max-width` / `min-width`**: Define larguras máxima/mínima.  
  Exemplo: `max-width: 600px;`
  
- **`margin`**: Define o espaçamento externo.  
  Exemplo: `margin: 10px;` ou `margin: 10px 15px;`
  
- **`padding`**: Define o espaçamento interno.  
  Exemplo: `padding: 10px;` ou `padding: 10px 15px;`
  
- **`border`**: Define a borda.  
  Exemplo: `border: 1px solid black;`
  
- **`box-sizing`**: Inclui ou exclui bordas e preenchimentos no cálculo de largura/altura.  
  Valores: `content-box`, `border-box`.  
  Exemplo: `box-sizing: border-box;`

---

#### **4. Propriedades de Posição**
- **`position`**: Define o método de posicionamento.  
  Valores: `static`, `relative`, `absolute`, `fixed`, `sticky`.  
  Exemplo: `position: absolute;`
  
- **`top`, `right`, `bottom`, `left`**: Define a posição relativa ao contêiner pai.  
  Exemplo: `top: 10px; left: 20px;`
  
- **`z-index`**: Define a ordem de empilhamento.  
  Exemplo: `z-index: 10;`

---

#### **5. Propriedades de Exibição e Flexbox**
- **`display`**: Define o comportamento do elemento.  
  Valores: `block`, `inline`, `inline-block`, `flex`, `grid`, `none`.  
  Exemplo: `display: flex;`
  
- **`flex-direction`**: Direção dos itens em um contêiner flexível.  
  Valores: `row`, `row-reverse`, `column`, `column-reverse`.  
  Exemplo: `flex-direction: column;`
  
- **`justify-content`**: Alinha itens no eixo principal.  
  Valores: `flex-start`, `center`, `space-between`, `space-around`, `space-evenly`.  
  Exemplo: `justify-content: space-between;`
  
- **`align-items`**: Alinha itens no eixo cruzado.  
  Valores: `flex-start`, `center`, `flex-end`, `stretch`.  
  Exemplo: `align-items: center;`
  
- **`gap`**: Define o espaçamento entre itens flexíveis ou em grid.  
  Exemplo: `gap: 10px;`

---

#### **6. Propriedades de Grid**
- **`grid-template-columns`**: Define o layout das colunas.  
  Exemplo: `grid-template-columns: 1fr 2fr;`
  
- **`grid-template-rows`**: Define o layout das linhas.  
  Exemplo: `grid-template-rows: 100px auto;`
  
- **`grid-gap`**: Define o espaçamento entre itens do grid.  
  Exemplo: `grid-gap: 15px;`
  
- **`place-items`**: Centraliza itens no grid.  
  Exemplo: `place-items: center;`

---

#### **7. Propriedades de Transformação e Animação**
- **`transform`**: Aplica transformações como rotação e escala.  
  Exemplo: `transform: rotate(45deg);`
  
- **`transition`**: Define transições suaves entre estados.  
  Exemplo: `transition: all 0.3s ease;`
  
- **`animation`**: Define animações personalizadas.  
  Exemplo:
  ```css
  @keyframes exemplo {
    from { opacity: 0; }
    to { opacity: 1; }
  }
  div {
    animation: exemplo 2s infinite;
  }
  ```

---

#### **8. Propriedades de Responsividade**
- **`@media`**: Define estilos condicionais para diferentes tamanhos de tela.  
  Exemplo:
  ```css
  @media (max-width: 600px) {
    body {
      background-color: lightblue;
    }
  }
  ```
  
- **`object-fit`**: Ajusta como imagens se encaixam em contêineres.  
  Valores: `cover`, `contain`, `fill`, `none`.  
  Exemplo: `object-fit: cover;`

---

#### **9. Propriedades de Sombra**
- **`box-shadow`**: Adiciona sombra ao elemento.  
  Exemplo: `box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);`
  
- **`text-shadow`**: Adiciona sombra ao texto.  
  Exemplo: `text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);`

---

#### **10. Propriedades Miscelâneas**
- **`cursor`**: Define o estilo do cursor.  
  Exemplo: `cursor: pointer;`
  
- **`overflow`**: Define o comportamento de conteúdo excedente.  
  Valores: `visible`, `hidden`, `scroll`, `auto`.  
  Exemplo: `overflow: hidden;`
  
- **`opacity`**: Define a opacidade do elemento.  
  Exemplo: `opacity: 0.8;`

---

### **Dicas Rápidas**
- Use **comentários** para organizar seu CSS: `/* Comentário */`.
- Combine seletores para economizar linhas de código: `h1, h2, h3 { margin: 0; }`.
- Prefira unidades responsivas como `em`, `rem`, `%`, `vw`, `vh` para melhor escalabilidade.
- Use variáveis CSS para consistência:  
  ```css
  :root {
    --primary-color: #3498db;
  }
  body {
    color: var(--primary-color);
  }
  ```

Já cobrimos as principais propriedades e dicas rápidas de CSS. A seguir, vou complementar com algumas ferramentas úteis e práticas avançadas para otimizar o uso de CSS.

---

### **11. Ferramentas Avançadas do CSS**
#### **Variáveis CSS**
- Variáveis CSS permitem armazenar valores reutilizáveis.  
  Exemplo:  
  ```css
  :root {
    --primary-color: #3498db;
    --secondary-color: #2ecc71;
    --font-size-base: 16px;
  }

  body {
    color: var(--primary-color);
    font-size: var(--font-size-base);
  }
  ```

#### **Pseudo-classes**
- Definem estados especiais de elementos.  
  Exemplos:  
  ```css
  a:hover { color: red; } /* Estado ao passar o mouse */
  input:focus { border-color: blue; } /* Foco em campos */
  li:nth-child(odd) { background-color: #f0f0f0; } /* Itens ímpares */
  ```

#### **Pseudo-elementos**
- Estilizam partes específicas de um elemento.  
  Exemplos:  
  ```css
  p::first-line { font-weight: bold; } /* Primeira linha */
  h1::after { content: ' 🌟'; } /* Adiciona conteúdo */
  ```

---

### **12. Técnicas de Otimização e Boas Práticas**
#### **Reset CSS**
- Remove estilos padrão do navegador para maior consistência.  
  Exemplo (reset simples):  
  ```css
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  ```

#### **Normalize.css**
- Biblioteca para normalizar estilos padrão entre navegadores.  
  Inclua com:  
  ```html
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css">
  ```

#### **Combinação de Selectores**
- Evite duplicação combinando regras semelhantes.  
  Exemplo:  
  ```css
  h1, h2, h3 { font-family: 'Arial', sans-serif; }
  ```

---

### **13. Ferramentas Responsivas**
#### **Unidades Responsivas**
- Use unidades flexíveis como:
  - `%`: Relativo ao elemento pai.
  - `em`: Relativo ao tamanho da fonte do elemento pai.
  - `rem`: Relativo ao tamanho da fonte da raiz.
  - `vw`/`vh`: Relativo à largura/altura da janela.

#### **Media Queries**
- Adapte estilos a diferentes dispositivos:  
  ```css
  @media (max-width: 768px) {
    body {
      font-size: 14px;
    }
  }
  ```

---

### **14. Animações Avançadas**
#### **Animações com `@keyframes`**
- Exemplo básico:  
  ```css
  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }

  .animado {
    animation: fadeIn 2s ease-in-out;
  }
  ```

#### **Transições**
- Adiciona suavidade às mudanças de estilo:  
  ```css
  button {
    background-color: #3498db;
    transition: background-color 0.3s ease;
  }
  button:hover {
    background-color: #2ecc71;
  }
  ```

---

### **15. Debug e Ferramentas de Desenvolvimento**
#### **Outline para Depuração**
- Use `outline` para visualizar os elementos na página:  
  ```css
  * {
    outline: 1px solid red;
  }
  ```

#### **Ferramentas do Navegador**
- Utilize o **DevTools** (F12 no Chrome/Firefox) para inspecionar e ajustar estilos em tempo real.

---

### **16. Frameworks CSS**
#### **Bootstrap**
- Framework popular para desenvolvimento rápido e responsivo.  
  Inclua com:  
  ```html
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
  ```

#### **Tailwind CSS**
- Framework utilitário para maior controle sobre os estilos.  
  Exemplo:  
  ```html
  <div class="bg-blue-500 text-white p-4 rounded-lg">Olá Mundo</div>
  ```

---

### **17. Inspiração e Recurso Extra**
#### **CSS Generators**
- Ferramentas online para gerar código CSS rapidamente:
  - **Box Shadow Generator**: Cria sombras de caixa.
  - **CSS Gradient Generator**: Facilita a criação de gradientes.
  - **Border Radius Generator**: Teste bordas arredondadas visualmente.

#### **Sites de Referência**
- [MDN Web Docs (CSS)](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS-Tricks](https://css-tricks.com/)

---

Já cobrimos as principais propriedades, técnicas avançadas e boas práticas de CSS. A seguir, vamos explorar conceitos adicionais e ferramentas que podem expandir ainda mais seu domínio sobre o CSS.

---

### **18. Conceitos Avançados**
#### **CSS Custom Properties (Variáveis) com Escopo**
- Variáveis CSS podem ser limitadas a escopos específicos.  
  Exemplo:  
  ```css
  :root {
    --main-color: #3498db;
  }

  .dark-theme {
    --main-color: #2c3e50;
  }

  body {
    background-color: var(--main-color);
  }
  ```

#### **Grid Avançado**
- Usando **grid-auto-flow** para controle automático:  
  ```css
  .container {
    display: grid;
    grid-auto-flow: dense; /* Preenche lacunas automaticamente */
    grid-template-columns: repeat(3, 1fr);
  }
  ```

- **Alinhamento no Grid**:  
  ```css
  .container {
    display: grid;
    place-items: center; /* Centraliza itens */
  }
  ```

#### **CSS Subgrid**
- Disponível em navegadores modernos, permite herdar o grid do elemento pai:  
  ```css
  .parent {
    display: grid;
    grid-template-columns: 1fr 2fr;
  }

  .child {
    display: subgrid;
  }
  ```

---

### **19. Pré-processadores CSS**
#### **SASS/SCSS**
- Ferramenta que expande as funcionalidades do CSS com aninhamento, mixins e loops.  
  Exemplo:  
  ```scss
  $primary-color: #3498db;

  body {
    color: $primary-color;

    h1 {
      font-size: 2em;
    }
  }
  ```

- **Mixins**: Reutilização de estilos.  
  ```scss
  @mixin flex-center {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .box {
    @include flex-center;
  }
  ```

#### **LESS**
- Similar ao SASS, com sintaxe mais leve.  
  Exemplo:  
  ```less
  @main-color: #3498db;

  body {
    color: @main-color;
  }
  ```

---

### **20. Acessibilidade com CSS**
#### **Foco Visível**
- Garanta que elementos focados sejam destacados:  
  ```css
  button:focus {
    outline: 2px solid #3498db;
  }
  ```

#### **Contrast Checker**
- Verifique contraste entre texto e fundo para atender às diretrizes WCAG.

#### **Preferências do Usuário**
- Respeite preferências do sistema operacional:  
  ```css
  @media (prefers-color-scheme: dark) {
    body {
      background-color: #333;
      color: #fff;
    }
  }
  ```

---

### **21. Metodologias de Organização**
#### **BEM (Block Element Modifier)**
- Ajuda a manter consistência em grandes projetos.  
  Exemplo:  
  ```html
  <div class="card card--highlighted">
    <h2 class="card__title">Título</h2>
    <p class="card__content">Conteúdo</p>
  </div>
  ```

  CSS:  
  ```css
  .card {
    border: 1px solid #ddd;
  }
  .card--highlighted {
    border-color: #3498db;
  }
  .card__title {
    font-size: 1.5em;
  }
  ```

---

### **22. Animações e Efeitos Visuais Avançados**
#### **Scroll Animations**
- Usando `scroll-behavior` para navegação suave:  
  ```css
  html {
    scroll-behavior: smooth;
  }
  ```

#### **Parallax com CSS Puro**
- Crie efeito de paralaxe simples:  
  ```css
  .parallax {
    background-image: url('imagem.jpg');
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
  }
  ```

#### **Blur e Filtros**
- Aplicando efeitos visuais com `filter`:  
  ```css
  .blurred {
    filter: blur(5px);
  }

  .grayscale {
    filter: grayscale(100%);
  }
  ```

---

### **23. Ferramentas e Extensões CSS**
#### **PostCSS**
- Transforma CSS moderno em código compatível com navegadores antigos.

#### **Autoprefixer**
- Adiciona prefixos automaticamente para garantir compatibilidade:  
  ```css
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  ```

#### **CSS Modules**
- Permite escopo local para estilos em projetos JavaScript modernos.

---

Com essa extensão da cheat-sheet, você agora tem acesso a recursos mais avançados e específicos para otimizar e modernizar o uso de CSS em seus projetos.

