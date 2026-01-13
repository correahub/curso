# **`class`** é o **atributo** que define **uma ou mais classes para um elemento**, permitindo agrupar e reutilizar estilos ou comportamentos em vários elementos.



















---

# 🎨 O que é **class** no CSS?

Imagine que você tem vários brinquedos iguais espalhados pelo quarto. Agora você quer **pintar todos eles de azul**. Mas em vez de pintar um por um, você coloca **uma etiqueta** neles com o nome “azul”.  
Pronto! Agora você diz:  
**“Todo brinquedo com a etiqueta ‘azul’, fique azul!”**

No CSS, a **class** funciona exatamente assim.

## 👉 **class é uma etiqueta que você coloca em vários elementos para aplicar o mesmo estilo.** 🎯

---

# 🧱 Como funciona na prática?

### 1️⃣ No HTML, você coloca a etiqueta (class):

```html
<p class="texto-bonito">Olá!</p>
<p class="texto-bonito">Tudo bem?</p>
<div class="texto-bonito">Eu também sou bonito!</div>
```

Todos esses elementos receberam a mesma **class**: `texto-bonito`.

---

### 2️⃣ No CSS, você cria o estilo para aquela class:

```css
.texto-bonito {
  color: blue;
  font-size: 20px;
}
```

O ponto (`.`) antes do nome significa **“isso é uma class”**.

---

# 🪄 Resultado mágico

Todos os elementos com **class="texto-bonito"** ficam **do mesmo jeitinho**, com a mesma cor e tamanho — porque eles carregam a mesma "etiqueta".

---

# 🧠 Explicação técnica simples (como você pediu)

**Class é um seletor usado para aplicar estilos a múltiplos elementos ao mesmo tempo. Ela é identificada com um ponto (.) no CSS.** 🎨✨

---
