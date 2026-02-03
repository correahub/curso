# conic-gradient()  é a **função que cria um gradiente que gira em volta de um ponto central**, como uma pizza 🍕 ou um gráfico de pizza





















---

# 🎯 O que é `conic-gradient`?

`conic-gradient()` cria um gradiente que gira **em volta de um ponto central**, como uma pizza 🍕 ou um gráfico de pizza.

👉 As cores são distribuídas por **ângulos**, não por distância.

---

## 🧠 Diferença visual rápida

- `linear-gradient` → linha
    
- `radial-gradient` → círculo que cresce
    
- **`conic-gradient` → rotação**
    

👉 Pense em um relógio.

---

# 📌 Sintaxe básica

```css
background: conic-gradient(red, blue);
```

Isso significa:

- começa em vermelho
    
- gira até virar azul
    
- completa **360°**
    

---

# 🔥 Controlando os ângulos (parte MAIS importante)

Você define onde cada cor começa:

```css
background: conic-gradient(
  red 0deg,
  yellow 120deg,
  blue 240deg
);
```

👉 Resultado:

- vermelho → 0° até 120°
    
- amarelo → 120° até 240°
    
- azul → 240° até 360°
    

---

## 📐 Entenda os graus

Um círculo tem:

```
360deg
```

- 90deg → direita
    
- 180deg → baixo
    
- 270deg → esquerda
    

👉 O padrão começa no **topo (12h)**.

---

# 📍 Mudando o ponto inicial

## `from`

Gira o gradiente inteiro.

```css
background: conic-gradient(from 90deg, red, blue);
```

👉 Agora começa da direita.

💡 Muito útil para:

- loaders
    
- gráficos
    
- animações
    

---

# 📌 Mudando o centro

## `at`

Igual ao radial.

```css
background: conic-gradient(at top left, red, blue);
```

👉 O giro acontece a partir do canto.

---

# 🎨 Criando divisões duras (sem transição)

Se duas cores tiverem o mesmo ponto:

```css
background: conic-gradient(
  red 0deg 90deg,
  blue 90deg 180deg
);
```

👉 Parece um gráfico de pizza real.

🔥 Muito usado em dashboards.

---

# ⚡ Exemplo MUITO usado (roda de cores)

```css
background: conic-gradient(
  red,
  yellow,
  lime,
  cyan,
  blue,
  magenta,
  red
);
```

---

# 🚨 Quando usar `conic-gradient`?

Perfeito para:

✅ gráficos de progresso  
✅ pizza charts  
✅ color pickers  
✅ loaders  
✅ efeitos modernos de UI  
✅ bordas animadas

---

# ⚠️ Erro comum

👉 Esquecer que ele trabalha com **ângulos**, não porcentagem de distância.

Mas você **pode usar % também**, porque:

```
100% = 360deg
```

Exemplo:

```css
conic-gradient(red 25%, blue 50%);
```

---

# 🧠 Resumo ultra rápido

👉 Gradiente que **gira**  
👉 Baseado em **ângulos**  
👉 Começa no topo  
👉 Pode mudar início (`from`)  
👉 Pode mudar centro (`at`)
