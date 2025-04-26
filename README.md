# 📚 Git Cheat Sheet Completo e Explicado (Português)

---

## 🛠️ Configurações Iniciais

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```
> Identificação do autor dos commits.

---

## 📦 Começando um projeto

| Comando | Descrição |
|:--------|:----------|
| `git init` | Inicializa um repositório vazio localmente |
| `git clone <url>` | Clona um repositório remoto |

---

## 📝 Trabalhando com arquivos

| Comando | Descrição |
|:--------|:----------|
| `git status` | Verifica o status dos arquivos |
| `git add <arquivo>` | Adiciona arquivo à área de staging |
| `git add .` | Adiciona todos os arquivos modificados |
| `git commit -m "mensagem"` | Cria um commit com uma mensagem |

---

## 📆 Atualizando o repositório

| Comando | Descrição |
|:--------|:----------|
| `git pull` | Baixa alterações do repositório remoto |
| `git push` | Envia alterações para o repositório remoto |

---

## 🌱 Trabalhando com Branches

| Comando | Descrição |
|:--------|:----------|
| `git branch` | Lista as branches locais |
| `git branch <nome>` | Cria nova branch |
| `git checkout <nome>` | Troca para a branch |
| `git checkout -b <nome>` | Cria e troca para nova branch |
| `git branch -d <nome>` | Deleta uma branch local |
| `git push origin <nome>` | Envia uma branch para o remoto |
| `git push origin --delete <nome>` | Deleta uma branch remota |

---

## 🧹 Stash (Guardar alterações temporariamente)

| Comando | Descrição |
|:--------|:----------|
| `git stash` | Guarda alterações temporárias |
| `git stash list` | Lista stashes guardados |
| `git stash apply` | Aplica o último stash sem removê-lo |
| `git stash pop` | Aplica e remove o stash |

---

## 👀 Visualizar histórico e diferenças

| Comando | Descrição |
|:--------|:----------|
| `git log` | Mostra o histórico de commits |
| `git log --oneline` | Histórico resumido |
| `git log --graph --oneline` | Histórico visual de branches |
| `git diff` | Mostra diferenças de arquivos |
| `git diff branch1 branch2` | Diferença entre branches |

---

## 🔥 Desfazendo mudanças

| Comando | Descrição |
|:--------|:----------|
| `git reset <arquivo>` | Remove arquivo do staging |
| `git checkout -- <arquivo>` | Desfaz mudanças no arquivo |
| `git reset --hard` | Descarta todas alterações |
| `git reset --soft <commit>` | Volta para commit sem apagar mudanças |
| `git revert <commit>` | Cria um commit revertendo um commit anterior |

---

## 🎫 Tags (Marcar versões)

| Comando | Descrição |
|:--------|:----------|
| `git tag v1.0` | Cria uma tag simples |
| `git tag -a v1.0 -m "mensagem"` | Cria uma tag anotada |
| `git push origin v1.0` | Envia uma tag específica |
| `git push origin --tags` | Envia todas as tags |

---

## 🔍 Comandos úteis para troubleshooting

| Comando | Descrição |
|:--------|:----------|
| `git reflog` | Lista todas as mudanças recentes (inclusive commits perdidos) |
| `git blame <arquivo>` | Mostra quem editou cada linha |
| `git bisect start` | Inicia busca binária para encontrar bug |

---

# 💡 Dicas Rápidas

- Faça commits pequenos e frequentes.
- Sempre execute `git pull` antes de trabalhar.
- Utilize branches para novas funcionalidades.
- Escreva mensagens de commit claras.

---

# 📂 Fluxo de Trabalho Sugerido

1. Atualizar o repositório:
   ```bash
   git pull origin main
   ```

2. Criar uma branch:
   ```bash
   git checkout -b feature/nova-funcionalidade
   ```

3. Fazer alterações e commitar:
   ```bash
   git add .
   git commit -m "Implementa nova funcionalidade X"
   ```

4. Enviar a branch para o servidor:
   ```bash
   git push origin feature/nova-funcionalidade
   ```

5. Abrir um Pull Request (PR) para revisão.

---

> Feito com ❤️ para ajudar a dominar Git!
