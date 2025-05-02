# ☁️ Instalação e Configuração Rápida do AWS CLI no Ubuntu (via Snap)

## ✅ Passo 1: Instale o AWS CLI usando Snap

```bash
sudo snap install aws-cli --classic
```

---

## ✅ Passo 2: Configure o AWS CLI

Execute o comando:

```bash
aws configure
```

Preencha os dados quando solicitado:

- **AWS Access Key ID**: `<id>`
- **AWS Secret Access Key**: `<key>`
- **Default region name**: `sa-east-1`
- **Default output format**: `json`

---


## ✅ Passo 3: Teste se está funcionando

Comando para verificar usuário autenticado:

```bash
aws sts get-caller-identity
```

---


## ✅ Passo 4: Teste se está funcionando

Execute um comando básico, como listar os buckets S3:

```bash
aws s3 ls
```

---

🟢 **Pronto!** O AWS CLI está instalado e configurado no Ubuntu usando Snap.
