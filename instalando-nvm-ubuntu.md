# 📦 Como instalar o NVM (Node Version Manager) no Ubuntu

## ✅ Passo 1: Atualize os pacotes

```bash
sudo apt update
sudo apt install curl -y
```

---

## ✅ Passo 2: Instale o NVM

Use o script oficial do GitHub:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

> 💡 Verifique a versão mais recente em: [https://github.com/nvm-sh/nvm/releases](https://github.com/nvm-sh/nvm/releases)

---

## ✅ Passo 3: Configure o ambiente

Adicione as seguintes linhas ao final do seu arquivo de configuração do shell:

- Para **Bash**:

  ```bash
  nano ~/.bashrc
  ```

- Para **Zsh**:

  ```bash
  nano ~/.zshrc
  ```

Adicione ao final do arquivo:

```bash
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```

Depois, recarregue o terminal:

```bash
source ~/.bashrc   # ou ~/.zshrc
```

---

## ✅ Passo 4: Verifique se o NVM foi instalado corretamente

```bash
nvm --version
```

---

## ✅ Passo 5: Instale e gerencie versões do Node.js

- Instalar a versão mais recente:

  ```bash
  nvm install node
  ```

- Instalar uma versão específica:

  ```bash
  nvm install 18
  nvm use 18
  ```

- Listar versões instaladas:

  ```bash
  nvm ls
  ```

- Alternar entre versões:

  ```bash
  nvm use <versão>
  ```

---

🟢 **Pronto!** Agora você pode usar diferentes versões do Node.js facilmente com o NVM.
