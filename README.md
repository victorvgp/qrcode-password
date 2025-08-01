# qrcode-password

# 🛠️ CLI Tool - QR Code & Password Generator

Projeto desenvolvido como exercício de prática em **Node.js**, utilizando entrada de dados pelo terminal para gerar **QR Codes** e **senhas seguras**, com base em variáveis de ambiente e bibliotecas como `chalk`, `prompt` e `qrcode-terminal`.

---

## 📁 Estrutura de Pastas

qrcode-password/
├── index.js
├── .env # Variáveis para personalização da senha
├── package.json
├── src/
│ ├── prompts-schema/
│ │ ├── schema-main.js # Pergunta principal do menu inicial
│ │ └── schema-qrcode.js # Perguntas específicas para gerar QR Code
│ └── services/
│ ├── password/
│ │ ├── create.js # Chama o processo de geração da senha
│ │ ├── handle.js # Lógica de criação da senha
│ │ └── utils/
│ │ └── permitted-characters.js # Define os caracteres permitidos
│ └── qr-code/
│ ├── create.js # Inicia o prompt para QR Code
│ └── handle.js # Gera o QR Code no terminal

---

## 🚀 Como executar

### 1. Instale as dependências

```bash
npm install

# Clone o repositório
git clone https://github.com/victorvgp/qrcode-password.git

# Acesse a pasta do projeto
cd qrcode-password

# Execute o arquivo principal
node --watch src/index.js
```

Crie um arquivo .env na raiz do projeto e adicione as variáveis desejadas para o gerador de senhas:

PASSWORD_LENGTH=12
UPPERCASE_LETTERS=true
LOWERCASE_LETTERS=true
NUMBERS=true
SPECIAL_CHARACTERS=true
