# 📚 Desafio 02 - GitHub Wiki em React

Este projeto foi desenvolvido durante a formação React da **DIO (Digital Innovation One)**. A aplicação consiste em uma Wiki que busca e lista repositórios públicos da API do GitHub.

---

## 🎯 O Desafio Resolvido
O objetivo principal deste desafio era implementar a lógica que estava faltando no projeto base: **a remoção de repositórios da tela**.

* **Funcionalidade desenvolvida:** Criação da função para o botão "Remover", permitindo que o usuário retire qualquer repositório da lista de exibição dinamicamente.

---

## 💻 Código Implementado

A remoção foi resolvida no arquivo `App.js` utilizando o método `.filter()` do JavaScript para gerar uma nova lista sem o repositório que foi clicado, atualizando o estado logo em seguida:

```javascript
const handleRemoveRepo = (id) => {
    console.log('Removendo registro', id);
    
    // Filtra e mantém apenas os repositórios que têm o ID diferente do clicado
    const newRepos = repos.filter(repo => repo.id !== id);
    
    // Atualiza o estado para refletir a mudança na tela
    setRepos(newRepos);
}
```

---

## 🚀 Como Rodar o Projeto Localmente

1. Abra o terminal na pasta deste desafio e instale as dependências:
   ```bash
   npm install
   ```

2. Inicie o servidor de desenvolvimento:
   ```bash
   npm start
   ```

O projeto abrirá automaticamente no endereço `http://localhost:3000`.

---

## 🧑‍💻 Autor

Desenvolvido por **Israel Monteiro**.
