Acho que você quis dizer:

## 🔄 `git restore`

`git restore` é o comando usado para **desfazer alterações em arquivos**.

Ele serve para voltar o arquivo para o estado anterior.

---

## 📄 Restaurar um arquivo modificado (antes do commit)

```bash
git restore index.html
```

Isso desfaz as alterações feitas em `index.html` que ainda não foram commitadas.

---

## ➖ Remover arquivo da área de stage

```bash
git restore --staged index.html
```

Isso tira o arquivo do stage (desfaz o `git add`).

---

## 🧠 Em resumo:

- `git restore arquivo` → desfaz mudanças locais
    
- `git restore --staged arquivo` → remove do stage
    