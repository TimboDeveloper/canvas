
# Aprendendo Canvas

Aprendendo como utilizar o canvas


## Sumário

 * [Context](#context)
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
## Créditos

[@TimboDeveloper](https://github.com/TimboDeveloper)