# **`z-index`** é o **atributo** que define **a ordem de empilhamento de um elemento** posicionado, controlando quais elementos aparecem à frente ou atrás quando eles se sobrepõem.























---

# 👶 Explicação como para uma criança

Imagina que você tem vários **papéis coloridos** na mesa.  
Agora você começa a colocar **um papel por cima do outro**.

- O papel que está **mais no topo** fica **mais visível** 👀
    
- O que está **embaixo** fica **escondido** 🙈
    

No CSS funciona igual!  
O **z-index** é como um **número mágico** que diz:

> “Este elemento deve ficar mais **em cima** ou mais **embaixo** do que os outros!”

---

# 🔢 Como funciona?

- Quanto **maior** o número do z-index ➜ mais **em cima** o elemento fica.
    
- Quanto **menor** ➜ mais **embaixo** ele fica.
    
- Exemplo:
    
    - `z-index: 10` fica **na frente** de `z-index: 5`.
        
    - `z-index: 0` fica **atrás** de `z-index: 50`.
        

---

# ⚠️ Mas tem um detalhe muito importante…

Para o **z-index funcionar**, o elemento precisa ter uma propriedade chamada **position** diferente de `static`.

Ou seja, precisa ser:

- `position: relative`
    
- `position: absolute`
    
- `position: fixed`
    
- `position: sticky`
    

Sem isso, o z-index **não funciona**, igual tentar flutuar sem balão 🎈😆.

---

# 🧱 Exemplo bem simples

```html
<div class="caixa1"></div>
<div class="caixa2"></div>
```

```css
.caixa1 {
  width: 200px;
  height: 200px;
  background: red;
  position: relative;
  z-index: 1;
}

.caixa2 {
  width: 200px;
  height: 200px;
  background: blue;
  position: relative;
  margin-left: -100px;
  margin-top: -100px;
  z-index: 2; /* essa fica na frente */
}
```

A caixa azul tem `z-index: 2`, então ela fica **na frente** da vermelha 💙➡️❤️.

---

# 🎯 Resumo rápido com emojis

- **z-index** ➜ controla o **nível de empilhamento** 🧱
    
- 🎚️ Número maior ➜ fica **na frente**
    
- 🎚️ Número menor ➜ fica **atrás**
    
- Precisa de **position** diferente de `static` ⚠️
    
- Funciona como **cartas empilhadas** 🃏
    

---
