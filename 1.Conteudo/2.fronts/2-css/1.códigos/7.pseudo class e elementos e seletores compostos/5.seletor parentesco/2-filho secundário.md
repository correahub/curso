# **`+`** é um **seletor de parentesco** que define **o elemento irmão imediatamente seguinte a outro elemento**, aplicando estilos apenas ao próximo irmão.

















```css
main h3 + p {
  color: blue;
}
```

E eu vou explicar como se você fosse uma criança 🧒, com exemplos fáceis de entender e imaginar.

---

## 🧠 O que significa `h3 + p`?

Esse seletor quer dizer:

> “Pinte de azul o **parágrafo (`p`) que vem logo depois** de um `h3`, dentro do `main`.”

### É como dizer:

> “Só quero mexer no irmão **que vem logo depois**!”

---

## 👨‍👦 Imaginando como uma historinha:

Pense que você tem um **quarto (`main`)** onde tem **várias pessoas sentadas** (elementos). Um deles é o **irmão mais velho `h3`**, e o outro é o **irmão mais novo `p`**, que está **sentado bem ao lado dele, sem ninguém no meio**.

Você só quer **dar um presente (mudar a cor)** pro irmão que está **logo ao lado**. Se tiver alguém no meio, você não dá o presente!

---

## 📦 Exemplo prático:

### HTML:

```html
<main>
  <h3>Título da seção</h3>
  <p>Texto que será azul</p>

  <h3>Outro título</h3>
  <div>Algo no meio</div>
  <p>Esse parágrafo NÃO será azul</p>
</main>
```

---

### CSS:

```css
main h3 + p {
  color: blue;
}
```

---

### ✅ O que vai acontecer?

1. O primeiro `<p>` **vai ficar azul**, porque ele está **logo depois do `h3`** ✅.
    
2. O segundo `<p>` **não vai mudar**, porque tem um `<div>` no meio ❌.
    

---

## 🧸 Como se fosse brinquedos:

- Dentro da caixa `main`, tem:
    
    - Um brinquedo `h3`
        
    - Logo ao lado dele, colado, está um `p` → esse vai ser colorido.
        
    - Mas se entre o `h3` e o `p` tiver outro brinquedo (tipo um `div`), o `p` não vai ser colorido.
        

---

## 🧪 Outro exemplo:

### HTML:

```html
<section>
  <h2>Subtítulo</h2>
  <p>Texto depois do h2</p>
  <p>Outro parágrafo</p>
</section>
```

### CSS:

```css
h2 + p {
  font-weight: bold;
}
```

➡️ Só o **primeiro `<p>` depois do `h2`** ficará em **negrito**.

---

## 📌 Resumo para guardar:

|Seletor|O que faz|
|---|---|
|`main h3 p`|Alvo: qualquer `p` DENTRO de `h3` dentro de `main`|
|`main h3 + p`|Alvo: o `p` que vem LOGO DEPOIS do `h3` dentro do `main` ✅|

---

Se quiser, posso mostrar também o `~` (irmão geral), que pega **todos os irmãos seguintes**, não só o que vem logo depois. Quer?