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

