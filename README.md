# Aprendendo Canvas

Aprendendo como utilizar o canvas


## Sumário

 * [Context](#context)
 * [fillStyle, fillRect](#fillrect-fillstyle)
 * [rect, fill, clearRect](#rect-fill-clearrect)
 * [moveTo, lineTo, Stroke](#moveto-lineto-stroke)
## Context

### HTML
Para começar a utilizar o canvas primeiro declare ele na sua página HTML:
```html
<canvas width="500" height="500">
  <h1>Canvas</h1>
  <h3>Seu browser não possui suporte ao canvas</h3>
  <!-- Essa mensagem só será renderizada quando o browser não possuir suporte ao canvas. -->
</canvas>
```
### JavaScript
Crie uma tag script e utilize o seguinte coódigo:
```javascript
// Para obter o canvas
const canvas = document.querySelector("canvas")

// Para obter o context
const context = canvas.getContext('2d')
```
![split](https://github.com/TimboDeveloper/canvas/raw/main/media/split.png)

## FillRect, FillStyle
 - fillStyle: define um preenchimento de cor
 - fillRect: cria um retângulo e já aplica o preenchimento
 
 [Arquivo: canvas_01.html](https://github.com/TimboDeveloper/canvas/blob/main/canvas_01.html)
```javascript
// Define uma cor
context.fillStlye = "#00f" // Azul

// Cria retângulo 100x100 e já preenche com a cor definida
context.fillRect(0, 0, 100, 100) // (X, Y, Width, Height)
```
<img src="https://github.com/TimboDeveloper/canvas/blob/main/media/fillstyle-fillrect.gif" alt="example fillstyle and fillrect gif" width="888" height="481.63" />

![split](https://github.com/TimboDeveloper/canvas/raw/main/media/split.png)

## Rect, Fill, ClearRect
 - rect: define um retângulo e não aplica o preenchimento
 - fill: aplica o preenchimento em todos os elementos da tela
 - clearRect: apaga uma área específica do canvas

 [Arquivo: canvas_02.html](https://github.com/TimboDeveloper/canvas/blob/main/canvas_02.html)
 ```javascript
// Define uma cor
context.fillStyle = "#00f" // Azul

// Cria retângulo 100x100 sem preenchimento
context.rect(0, 0, 100, 100) // (X, Y, Width, Height)

// Preenche todos os retângulos com cor
context.fill() 

// Apaga o retângulo criado
context.clearRect(0, 0, 100, 100) // (X, Y, Width, Height)
 ```

### Não funciona

```javascript
// Define uma cor
context.fillStyle = "#00f" // Azul

// Cria retângulo 100x100 e já preenche com a cor definida
context.fillRect(0, 0, 100, 100) // (X, Y, Width, Height)

// Define uma nova cor
context.fillStyle = "#f00" // Red

// Não preenche retângulo com a nova cor
context.fill()
```
<img src="https://github.com/TimboDeveloper/canvas/blob/main/media/rect-fill-clearrect.gif" alt="example fillstyle and fillrect gif" width="888" height="481.63" />

![split](https://github.com/TimboDeveloper/canvas/raw/main/media/split.png)

## MoveTo, LineTo, Stroke

 - moveTo: Move o ponteiro do desenho para uma posição específica do canvas
 - lineTo: Adiciona uma linha a partir do ponteiro inicial até uma posição específica do canvas e substitui a posição inicial pela posição final

[Arquivo: canvas_03.html](https://github.com/TimboDeveloper/canvas/blob/main/canvas_03.html)
```javascript
// Adiciona ponteiro em X=0 Y=0
context.moveTo(0, 0) // (X, Y)

// Cria linha até X=250 Y=250
context.lineTo(250, 250) // (X, Y)

// Desenha a linha no canvas
context.stroke()
```

<img src="https://github.com/TimboDeveloper/canvas/blob/main/media/moveto-lineto-stroke.gif" alt="example moveTo lineTo stroke gif" width="888" height="481.63" />

![split](https://github.com/TimboDeveloper/canvas/raw/main/media/split.png)
## Créditos

[@TimboDeveloper](https://github.com/TimboDeveloper)