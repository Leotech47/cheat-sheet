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

