# 🚀 Chad-DevStudy LMS

Uma plataforma educacional interativa, 100% client-side e sem servidor, projetada para transformar o aprendizado de programação em uma experiência gamificada e segura.

## 📂 Estrutura do Projeto

```text
chad-devstudy/
├── css/               # Estilos Vanilla CSS (Glassmorphism & Design System)
├── js/                # Lógica da aplicação, Pyodide worker e Banco de Dados (data.js)
├── assets/            # Imagens, ícones e arquivos estáticos
├── index.html         # Ponto de entrada da aplicação (SPA)
├── LICENSE            # Licença MIT
└── README.md          # Documentação principal
```

## ✨ Funcionalidades Principais

* ⚡ **Arquitetura Serverless:** 100% no navegador. Dados em JSON nativo para latência zero.
* 📚 **Renderização Markdown:** Aulas ricas com snippets de código e diagramas via `marked.js`.
* 🧠 **Retenção Ativa:** Flashcards 3D, Quizzes Inline e o método "Palácio da Memória".
* 🐍 **Python no Browser:** Terminal integrado via **WebAssembly** (`Pyodide`) rodando em Web Workers.
* 🛡️ **Segurança Avançada:** Sanitização via `DOMPurify` e políticas de CSP estritas.
* ⏳ **Foco (Pomodoro):** Timer integrado para sessões de estudo profundo.

## 🚀 Como Rodar Localmente

Este projeto não possui dependências de Node.js ou processos de build.

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/Neguchads/chad-devstudy.git
   ```
2. **Abra no navegador:**
   - Basta abrir o arquivo `index.html`.
   - *Recomendado:* Use um servidor estático simples para evitar bloqueios de CORS:
     ```bash
     python -m http.server 3000
     ```

## 🤝 Contribuição e Comunidade

Nós encorajamos contribuições! Para manter uma comunidade saudável e produtiva, siga estas diretrizes:

### Como Contribuir

1. Faça um **Fork** do projeto.
2. Crie uma **Branch** para sua funcionalidade ou correção (`git checkout -b feature/MinhaNovaFuncionalidade`).
3. Faça o **Commit** das suas alterações (`git commit -m 'Feat: Adiciona MinhaNovaFuncionalidade'`).
4. Faça o **Push** para a branch (`git push origin feature/MinhaNovaFuncionalidade`).
5. Abra um **Pull Request**.

### Regras da Comunidade

* **Respeito:** Seja gentil e profissional com todos os contribuidores.
* **Clareza:** Escreva mensagens de commit e descrições de Pull Requests de forma descritiva e direta.
* **Qualidade de Código:** Garanta que seu código siga padrões de Vanilla JS e CSS limpo.
* **Issues:** Antes de iniciar uma mudança arquitetural ou adicionar uma funcionalidade muito grande, abra uma *Issue* para discutirmos a abordagem.

## 🛡️ Segurança

Levamos a segurança a sério.

* **Validação:** A aplicação utiliza `DOMPurify` para sanitização de entradas e prevenção de XSS (Cross-Site Scripting).
* **Isolamento:** A execução de scripts Python ocorre em um Web Worker isolado para prevenir travamentos e ataques de negação de serviço local (DoS).
* **Relatando Vulnerabilidades:** Se você encontrar alguma falha de segurança, por favor **NÃO** abra uma issue pública. Entre em contato diretamente com os mantenedores.

## ⚖️ Licença

Este projeto é distribuído sob a licença **MIT**. Veja o arquivo `LICENSE` para mais detalhes.

---

<div align="center">
  <i>"Não existe perfeito — existe lançado."</i><br>
  Criado por <strong>Gustavo (Chad-DevStudy)</strong>
</div>
