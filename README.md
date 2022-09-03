# Aprendendo Canvas

Aprendendo como utilizar o canvas


## Sumário

 * [Context](#context)
 * [fillStyle, fillRect](#fillrect-fillstyle)
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
const canvas = document.querySelector("canvas") // Para obter o canvas
const context = canvas.getContext('2d') // Para obter o context
```
![split](https://github.com/TimboDeveloper/canvas/raw/main/media/split.png)

## FillRect, FillStyle
 - fillStyle: define um preenchimento de cor.
 - fillRect: cria um retângulo e já aplica o preenchimento.
 [Arquivo: canvas_01.html](https://github.com/TimboDeveloper/canvas/blob/main/canvas_01.html)
```javascript
context.fillStlye = "#00f" // Azul
context.fillRect(0, 0, 100, 100) // context.fillRect(X, Y, Width, Height)
```
<img src="https://github.com/TimboDeveloper/canvas/blob/main/media/fillstyle-fillrect.gif" alt="example fillstyle and fillrect gif" width="888" height="481.63" />

![split](https://github.com/TimboDeveloper/canvas/raw/main/media/split.png)
## Créditos

[@TimboDeveloper](https://github.com/TimboDeveloper)