# Meu Site Simples - Trabalho de DevOps

Este projeto é um exemplo simples de front-end utilizando HTML, CSS e JavaScript. Ele foi criado com o objetivo de demonstrar a implementação de um pipeline de CI/CD usando **GitHub Actions** para a disciplina de **DevOps**.

---

## 🌐 Funcionalidade

Um site estático com um botão que exibe um alerta, composto por:

- `index.html`: página principal
- `styles.css`: estilo da página
- `script.js`: script JavaScript simples

---

## ⚙️ Pipeline com GitHub Actions

O pipeline está localizado em `.github/workflows/pipeline.yml` e é acionado a cada `push` na branch `main`.

### 🔧 Etapas do Pipeline:

1. **Clonar o repositório**  
   Usa a action `actions/checkout` para baixar o código.

2. **Simular build**  
   Valida os arquivos HTML, CSS e JS com comandos de terminal (`ls`, `file`).

3. **Deploy no GitHub Pages**  
   Utiliza a action `peaceiris/actions-gh-pages` para publicar o site.

---

## 🚀 Deploy

O site será publicado automaticamente em:
https://<seu-usuario>.github.io/<nome-do-repositorio>/
