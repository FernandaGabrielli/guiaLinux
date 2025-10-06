# Guia de Contribuição | Contributing Guide

---

## 🇧🇷 Português

### 🎯 Como Contribuir

Obrigado pelo interesse em contribuir com o **Guia de Comandos Linux**! Seguindo estas diretrizes, garantimos que o repositório mantenha qualidade e consistência.

### 📑 Tipos de Contribuição

* **🐛 Reportar Bugs**: Encontrou um erro? Abra uma issue descrevendo o problema
* **💡 Sugerir Melhorias**: Tem ideias para novos comandos ou melhor organização?
* **📚 Adicionar Comandos**: Conhece comandos úteis que não estão na lista?
* **🔧 Corrigir Documentação**: Encontrou typos ou informações imprecisas?
* **🌐 Traduções**: Ajudar a melhorar versões em outros idiomas

### 🛠️ Processo de Contribuição

1. **Fork do Repositório**

```bash
git clone https://github.com/FernandaGabrielli/guiaLinux/
cd guiaLinux
```

2. **Crie uma Branch**

```bash
git checkout -b feature/nova-funcionalidade
# ou
git checkout -b fix/correcao-comando
# ou
git checkout -b docs/melhoria-documentacao
```

3. **Faça suas Alterações**

* Adicione comandos seguindo o formato existente
* Mantenha a consistência de markdown
* Teste os comandos antes de incluir
* Verifique a formatação

4. **Commit das Alterações**

```bash
git add .
git commit -m "feat: adiciona comandos de rede"
# ou
git commit -m "fix: corrige exemplo do comando find"
# ou
git commit -m "docs: atualiza documentação em português"
```

5. **Push e Pull Request**

```bash
git push origin feature/nova-funcionalidade
```

* Abra um Pull Request no GitHub
* Descreva claramente suas mudanças
* Referencie issues relacionadas (se houver)

### 📋 Padrões de Código

* Comandos: Use `backticks` para comandos
* Exemplos: Inclua exemplos práticos de uso
* Organização: Mantenha a categorização existente
* Linguagem: Escreva em português claro e objetivo
* Tabelas: Use formatação consistente nas tabelas
* Headers: Siga a hierarquia de headers do markdown

### 🎗️ Template para Issues

**Título:** [BUG/FEATURE/DOCS] Descrição breve

**Descrição:**

* Comando/Seção afetada:
* Problema/Sugestão:
* Comportamento esperado:
* Passos para reproduzir (para bugs):
* Screenshots (se aplicável):

### 💾 Estrutura do Projeto

```
guiaLinux/
├── README.md          # Documentação principal
├── CONTRIBUTING.md    # Este arquivo
└── LICENSE           # Licença do projeto
```

### ❗ Código de Conduta

* Respeite todos os contribuidores
* Mantenha discussões construtivas
* Seja paciente com iniciantes
* Celebre as contribuições da comunidade
* Feedback deve ser sempre respeitoso e útil

### ✅ Checklist antes de enviar PR

* Testei os comandos adicionados/modificados
* Segui os padrões de formatação
* Verifiquei por typos e erros de gramática
* Atualizei a documentação relacionada
* Meu código está em uma branch feature específica
