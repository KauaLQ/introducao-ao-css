<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0165f4&height=120&section=header"/>

# introducao-ao-css <img width='70' heigth='70' src="https://github.com/user-attachments/assets/9a53faa3-f642-4386-a814-8219e38ffc5b"/>
#### Olá, _WebDev's_!  Este repositório contém meus primeiros estudos sobre CSS, parte da residência em TIC oferecida pela UECE em parceria com o Instituto Atlântico. Aqui você encontrará desde fundamentos básicos de estilização até exemplos práticos que explorei no curso.

#### Além disso, incluí o resultado da segunda oficina prática: uma página web construída com HTML e CSS com o tema "Um lugar que eu gostaria de conhecer". O projeto ficou muito legal! Ele possui um menu interativo e uma estrutura bem organizada, buscando aplicar os conceitos de layout e estilização aprendidos até agora. Espero que gostem e aproveitem para explorar e contribuir com sugestões!

#

#### CSS (Cascading Style Sheets) é a linguagem de estilo usada para definir a aparência visual de uma página web estruturada em HTML. Com CSS, você pode controlar cores, fontes, tamanhos, espaçamentos, layouts e até criar animações, separando o estilo da estrutura da página.

### Estrutura Básica do CSS
#### CSS pode ser aplicado de três formas principais:
- CSS Inline: Estilo aplicado diretamente em uma tag HTML com o atributo `style`.
- CSS Interno: Estilo definido dentro de uma tag `<style>` no `<head>` do HTML.
- CSS Externo: Arquivo `.css` separado, vinculado ao HTML com a tag `<link>`, recomendado para projetos maiores.

#### Exemplo de arquivo CSS externo:
```css
/* Arquivo styles.css */
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
}

h1 {
    color: #333;
    text-align: center;
}

p {
    font-size: 16px;
    line-height: 1.5;
}
```

#### Para aplicar o CSS externo em um HTML:
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Exemplo com CSS</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Bem-vindo ao CSS!</h1>
    <p>Este é um exemplo básico de como aplicar estilos.</p>
</body>
</html>
```

### Tags (Seletores) mais Utilizados no CSS
#### 1. Seletores de Tipo
#### Selecionam todas as tags de um tipo específico, como `h1`, `p`, `div`, aplicando estilo em todas essas ocorrências.

#### Exemplo:
```css
p {
    color: #555;
    font-size: 18px;
}
```

#### 2. Seletores de Classe
#### Utilizam `.` para aplicar estilos a elementos com uma classe específica. Classes permitem estilizar grupos de elementos específicos sem afetar o restante.

#### Exemplo:
```html
<p class="destaque">Texto destacado.</p>
```
```css
.destaque {
    background-color: yellow;
    font-weight: bold;
}
```

#### 3. Seletores de ID
#### Utilizam `#` para aplicar estilo a um único elemento com ID específico, pois IDs devem ser únicos em uma página.

#### Exemplo:
```html
<h1 id="titulo-principal">Título Principal</h1>
```
```css
#titulo-principal {
    font-size: 32px;
    color: #0073e6;
}
```

#### 4. Seletores de Atributo
#### Permitem estilizar elementos com base em um atributo específico, como links `target="_blank"`.

#### Exemplo:
```css
a[target="_blank"] {
    color: red;
}
```

#### 5. Seletores Descendentes
#### Estilos aplicados a elementos dentro de um contêiner específico, permitindo estilos contextuais.

#### Exemplo:
```html
<div class="container">
    <p>Este parágrafo será azul.</p>
</div>
```
```css
.container p {
    color: blue;
}
```

### Palavras Reservadas do CSS para Estilização
#### No CSS, propriedades específicas definem a estilização dos elementos em uma página web. Essas propriedades controlam desde a organização do layout até o estilo de fontes, cores e tamanhos. Vamos explorar algumas das propriedades mais utilizadas, com exemplos para melhor compreensão.

#

#### 1. Margin
#### A propriedade `margin` controla o espaço externo entre um elemento e outros ao seu redor. Ela pode ser ajustada em quatro direções: `top`, `right`, `bottom` e `left`.

#### Exemplo:
```css
div {
    margin: 10px; /* Aplica uma margem de 10px em todos os lados */
}
```
#### Valores específicos para cada lado:
```css
div {
    margin-top: 10px;
    margin-right: 20px;
    margin-bottom: 10px;
    margin-left: 20px;
}
```

#### 2. Padding
#### `Padding` define o espaço interno entre o conteúdo de um elemento e suas bordas. Funciona da mesma maneira que `margin`, com valores para os quatro lados.

#### Exemplo:
```css
div {
    padding: 15px; /* Aplica 15px de espaçamento interno em todos os lados */
}
```

#### 3. Display
#### A propriedade `display` controla como um elemento é exibido no layout. Alguns dos valores mais comuns incluem:
- `block`: O elemento ocupa toda a largura disponível (como `<div>`).
- `inline`: O elemento não quebra a linha (como `<span>`).
- `inline-block`: Combina comportamentos de `inline` e `block`.
- `none`: Esconde o elemento.
#### Exemplo:
```css
span {
    display: block; /* Exibe o elemento como bloco */
}
```

#### 4. Text-align
#### `text-align` é usada para alinhar o texto dentro de um elemento. Seus valores comuns incluem:
- `left`: Alinhado à esquerda.
- `center`: Centralizado.
- `right`: Alinhado à direita.
- `justify`: Justifica o texto (alinha o texto entre as margens esquerda e direita).
#### Exemplo:
```css
p {
    text-align: center;
}
```

#### 5. Font-size
#### Define o tamanho da fonte do texto. Pode ser especificado em pixels (`px`), pontos (`px`), ou como uma porcentagem (`%`).

#### Exemplo:
```css
h1 {
    font-size: 24px;
}
```

#### 6. Color
#### Define a cor do texto de um elemento. Pode usar valores em nome de cores (`red`), hexadecimal (`#ff0000`), ou valores RGB/RGBA (`rgb(255, 0, 0)` ou `rgba(255, 0, 0, 0.5)`).

#### Exemplo:
```css
p {
    color: #333333;
}
```

#### 7. Background-color
#### Define a cor de fundo do elemento. Aceita os mesmos formatos de cor que a propriedade `color`.

#### Exemplo:
```css
div {
    background-color: #f0f0f0;
}
```

#### 8. Width e Height
#### `width` e `height` definem a largura e altura de um elemento, respectivamente. Podem ser definidos em pixels, porcentagem, `vh` (viewport height) e `vw` (viewport width).

#### Exemplo:
```css
div {
    width: 100px;
    height: 200px;
}
```

#### 9. Border
#### Define a borda ao redor de um elemento. Pode ser personalizada com espessura, estilo e cor.
#### Exemplo:
```css
div {
    border: 2px solid #333;
}
```

#### 10. Position
#### `position` controla o posicionamento de um elemento. Valores comuns incluem:
- `static`: Padrão, sem posicionamento específico.
- `relative`: Posicionado em relação à sua posição normal.
- `absolute`: Posicionado em relação ao seu contêiner mais próximo.
- `fixed`: Fixa o elemento na tela, independente do scroll.
```css
div {
    position: absolute;
    top: 50px;
    left: 20px;
}
```

#### 11. Align-items e Justify-content
#### Usadas principalmente em layouts `flex` e `grid`, controlam o alinhamento dos elementos filhos:
- `align-items`: Alinha os itens no eixo vertical.
- `justify-content`: Alinha os itens no eixo horizontal.
```css
.container {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
```

#

### Conclusão
#### CSS é fundamental para definir a aparência de uma página, facilitando a criação de layouts organizados e atraentes. Com a estrutura modular dos arquivos CSS e o uso de seletores, desenvolvedores podem manter uma consistência visual e aplicar estilos de forma eficiente em projetos de qualquer escala.

---

### _Gostou do meu perfil? Você pode saber mais sobre mim em:_ &nbsp;&nbsp;[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kaualimaq/)
### _Ou me contatar através do:_ &nbsp;&nbsp;[![Gmail](https://img.shields.io/badge/Gmail-333333?style=for-the-badge&logo=gmail&logoColor=red)](mailto:limakaua610@gmail.com)
