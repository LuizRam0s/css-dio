# CSS - DIO RESUMO

CSS é uma linguagem que usamos para estilizar um documento HTML, css significa folhas de estilo em cascata

### Por que usar CSS?

CSS é usado para definir estilos para suas páginas da web, incluindo design, layout e variações de exibição para diferentes dispositivos e tamanhos de tela

---

## Ordem em Cascata

Qual estilo será usado quando houver mais de um estilo especificado para um elemento HTML?

1. Estilo embutido (dentro de um elemento HTML)
2. Folhas de estilo externas e internas (na seção head)
3. Padrão do navegador

# Seletores CSS

Os seletores CSS são usados para “encontrar” (ou selecionar) os elementos HTML que você deseja estilizar.

Podemos dividir os seletores CSS em cinco categorias:

- Seletores simples (selecione elementos com base no nome, id, classe)
- [Seletores combinadores](https://www.w3schools.com/css/css_combinators.asp)
  
    (selecionam elementos com base em um relacionamento específico entre eles)
    
- [Seletores de pseudoclasse](https://www.w3schools.com/css/css_pseudo_classes.asp)
  
    (selecionam elementos com base em um determinado estado)
    
- [Seletores de pseudoelementos](https://www.w3schools.com/css/css_pseudo_elements.asp)
  
    (selecionam e estilizam uma parte de um elemento)
    
- [Seletores de atributos](https://www.w3schools.com/css/css_attribute_selectors.asp)
  
    (selecionam elementos com base em um atributo ou valor de atributo)
    

## Cores

Podemos definir as cores pelos seguintes métodos:

*Hexadecimal:

```css
p{color: #ff004d;} 
```

ff defini o qual vermelho terá, 00 será o verde e 4d o azul

*Rgb e rgba: defini a cor por numeração, de 0 a 255 sendo que para cada número colocado será pra o quanto de cor terá sendo três o red, Green e blue. O rgba é uma extensão de rgb sendo o a Alpha que defini a opacidade da cor de 0.0 a 1.0

```css
h1{color: rgba(200, 167, 100, 0.6);}
```

*Hsl e hlsa: defini a cor através da matriz, saturação e leveza, sendo matriz de 0 a 360, saturação e leveza de 0% a 100%. O hsla é uma extensão do hsl colocando um Alpha para a opacidade

```css
p {color: hsla(240, 50%, 60% 0.4);}
```

### ⚠️⚠️Propriedade Apreviada

Para encurtar o código, também é possível especificar todas as propriedades de fundo em uma única propriedade

** background APREVIADA

```css
body { background: #ffffff url("img_tree.png") no-repeat right top; }
/*ordem pra apreviar é: color, image, repeat, attachment e position*/
```

**border APREVIADA

```css
div{border: 5px solid red}
/*ordem: width, style, color*/
```

**margin APREVIADA

```css
div{margin: 5px 8px 15px 10px}
/*margem superior, direita, inferiro e esquerda*/
```

**padding APREVIADA

```css
div{padding: 10px 15px 16px 18px}
/*margem superior, direita, inferiro e esquerda*/
```

## Bordas

Propriedade resposanvel poe adicionar o formado, expessura e cor da nossa porda.

*border-style propriedade especifica que tipo de borda exibir. A propriedade pode ter de um a quatro valores (para borda superior, borda direita, borda inferior e borda esquerda).

*border-width defini a expessura das bordas

Pode possuir os seguintes valores:

*border-color propriedade usada para definir a cor das quatro bordas.

*border-radius propriedades usadas para adicionar bordas arrendondadas a um elemento.

```css
exe{
border-style: dotted; /*Defini uma borda pontilhada*/
border-width: 5px; /*Defini uma borda de expessura de 5px de todos os lados*/
border-color: red;
}
```

```css
exe1{
border-style: dashed;/*Defini uma borda tracejada*/
border-width:medium; /*Defini uma borda media*/
border-color:#f5f5f5;
}
```

```css
exe2{
border-style: solid;/*Defini uma borda solida*/
border-width:thick; /*defini uma borda grossa*/
border-color: #ff55f8 #d5d5d5; /*defini as cores superior e inferior com #ff55f8 e as dos lados como #d5d5d5*/
}
```

```css
exe3{
border-style: double;/*Defini uma borda dupla*/
border-width: 5px 10px;/*defini uma borda de 5px pra parte superior e inferior e 10px nas laterais*/
border-color: #ff55f8 #d5d5d5 blue red; /*defini cada lado de uma cor que foi definido seguindo o relogio*/
}
```

```css
exe4{
border-style: groove;/*Define uma borda ranhurada 3D. O efeito depende do valor da cor da borda*/
border-width: 2px 5px 10px 15px; /*defini uma borda de cada expessura seguindo um relogio*/
}
```

```css
exe5{
border-style: ridge;/*Define uma borda estriada 3D. O efeito depende do valor da cor da borda*/
border-width: 2px;
border-radius: 5px;/*Defini qual o grau de curvatura das bordas*/
}
```

```css
exe6{border-style: inset;}/*Define uma borda estriada 3D. O efeito depende do valor da cor da borda*/
```

```css
exe7{border-style:outset ;}/*Define uma borda estriada 3D. O efeito depende do valor da cor da borda*/
```

```css
exe8{border-style: none;}/*Não defini borda*/
```

```css
exe9{border-style: hidden;}/*Defini uma borda oculta*/
```

# Background #

Defini o fundo do elemento podendo ser cores ou imagens.

*background-color propriedade especifica a cor de fundo de um elemento.

```css
body{
background-color: #f9f9f9 /*Defini a cor*/
opacity: 0.4; /*defini a opacidade de 0.0 a 1.0*/			
;}
```

⚠️⚠️podemos definir opacidade em propriedades background, opacidade è dado por um valor de 0 0 a 1.0

*background-image propriedade especifica uma imagem a ser usada como plano de fundo de um elemento.
Por padrão, a imagem é repetida para cobrir todo o elemento.

```css
div {
background-image: url(passarLocalizacao);
} 
```

*background-repeat defini como uma imagem deve se repetir. Possui alguns valores como:

```css
body{background-repeat: repeat-x;}
/*repete na horizontal*/
```

```css
body{background-repeat: repeat-y;}
/*repete na vertical*/
```

```css
body{background-repeat: no-repeat;}
/*não repete*/
```

*background-position: defini a posicao da imagem de fundo, possui valores como top, right, left e bottom 

```css
div{background-position: top left;} 
```

*background-attachment propriedade especifica se a imagem de fundo deve rolar ou ser fixa (não rolará com o resto da página).

```css
div{background-attachment: fixed;}
/*defini que o fundo fique fixo*/
```

```css
body{background-attachment: scrool;}
/*a imagem deve rolar com a página*/ 
```

*background-clip defini até que ponto o fundo deve se  estender dentro de um elemento

```css
.exemplo1{background-clip: padding-box;}
/*Valor padrão imagens vai ate o final da borda*/
```

```css
.exemplo2{padding-box}
/*O plano de fundo se estende até a borda interna da borda.*/
```

```css
.exemplo3{background-clip: content-box;}
/*O plano de fundo se estende até a borda da caixa de conteúdo*/
```

*background-origin propriedade especifica a posição de origem (a área de posicionamento do plano de fundo) de uma imagem de plano de fundo.

```css
body {background-origin: padding-box ;}
/*imagem começa no canto superior esquerdo da borda de preenchimento*/
```

```css
body {background-origin: border-box ;}
/*A imagem de fundo começa no canto superior esquerdo da borda.*/
```

```css
body {background-origin: content-box ;}
/*A imagem de fundo começa no canto superior esquerdo do conteúdo*/
```

*background-size defini o tamanho de uma imagem de fundo em px ou auto.

```css
div{background-size: auto}
/*Imagem de fundo exibido no seu tamanho original*/
```

```css
div{background-size:320px 240px}
/*imagem exibido conforme o tamanho passado em px*/
```

```css
div{background-size: cover} /*Dimensione a imagem (quanto preserve sua proporção) para o menor tamanho possível para caber no contêiner (ou seja: tanto a altura quanto o comprimento cobrem completamente o contêiner)*/
```

```css
div{background-size: contain}
/*Dimensione a imagem o máximo possível dentro do seu contêiner sem cortar ou estender a imagem.*/
```

## Margens

As margens são usadas para criar espaço ao redor dos elementos, fora de quaisquer bordas definidas. Existem propriedades para definir a margem para cada lado de um elemento (superior (margin-top), direito(margin-right), inferior (margin-bottom) e esquerdo(margin-left) ‼️ Valores negativos são permetidos.

```css
p {margin-top: 100px;
margin-bottom: 100px;
margin-right: 150px;
margin-left: 80px;}
```

Valor auto 

```css
div{margin: auto;/*centralizar horizontalmente o elemento dentro de seu contêiner.*/} 
p{margin: inherit; /*permite que a margem seja herdada do elemento pai*/}
```

‼️Colapso da margem,  faz com que a margem superior e inferior de dois elementos diferentes se sobreboem, fazendo assim a margem maior ser o valor real.

## Padding

O padding é usado para criar espaço ao redor do conteúdo de um elemento, dentro de quaisquer bordas definidas. Existem propriedades para definir a margem para cada lado de um elemento (superior (padding-top), direito(padding-right), inferior (padding-bottom) e esquerdo(padding-left) ‼️ Valores negativos são permetidos

```css
div{
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}
```

# Box-sizing

Isto faz com que o elemento mantenha sua largura real; se você aumentar o preenchimento, o espaço de conteúdo disponível diminuirá. Use a propriedade box-sizing para manter a largura em 300px, independentemente da quantidade de preenchimento:

```css
div {
  width: 300px;
  padding: 25px;
  box-sizing: border-box;
}
```