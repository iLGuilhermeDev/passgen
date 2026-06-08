# 🔐 PassGen – Gerador de Senhas Seguro

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![Tkinter](https://img.shields.io/badge/GUI-Tkinter-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

**PassGen** é uma ferramenta desktop com interface gráfica para gerar senhas fortes, avaliar sua força e armazenar senhas de forma local (codificada em Base64). Ideal para quem busca praticidade e segurança no dia a dia.

![Screenshot do PassGen](https://via.placeholder.com/700x400?text=PassGen+Interface+Preview)  
*(Substitua por uma imagem real do seu programa depois de executar)*

---

## ✨ Funcionalidades

- ✅ Geração personalizada de senhas:
  - Comprimento entre 4 e 50 caracteres
  - Escolha entre letras maiúsculas, minúsculas, números e símbolos
- 🔍 Avaliação automática da força (FRACA / MÉDIA / FORTE)
- 💾 Salvamento local de senhas por serviço/site
- 📋 Visualização de todas as senhas salvas com data/hora
- 🖥️ Interface simples e intuitiva (abas separadas)
- 🔒 Ofuscação das senhas salvas usando Base64

---

## 📦 Instalação

### Pré‑requisitos
- Python 3.7 ou superior (com Tkinter incluso – já vem no Python padrão)

### Passos
1. Clone o repositório (ou baixe o arquivo `passgen.py`):
   ```bash
   git clone https://github.com/seu-usuario/passgen.git
   cd passgen
Execute o programa:

bash
python passgen.py
Nenhuma biblioteca externa é necessária – tudo funciona com a biblioteca padrão do Python.

🚀 Como usar
Gerar senha: Acesse a aba Gerar Senha, configure os critérios e clique em Gerar Senha.

Salvar uma senha: Após gerar, digite o nome do serviço/site e clique em Salvar Senha.

Ver senhas salvas: Vá para a aba Senhas Salvas e clique em Atualizar Lista.

🛡️ Segurança
As senhas são armazenadas localmente no arquivo senhas.dat codificadas em Base64.

Atenção: Base64 não é criptografia – serve apenas como uma ofuscação leve. Para ambientes sensíveis, substitua por uma criptografia real (ex: cryptography.fernet com uma senha mestra).

Nunca compartilhe o arquivo senhas.dat publicamente (ele está automaticamente ignorado pelo .gitignore).

📂 Estrutura do projeto
text
passgen/
├── passgen.py          # Código principal com interface Tkinter
├── senhas.dat          # Banco de senhas (criado automaticamente)
├── README.md           # Este arquivo
└── .gitignore          # Ignora senhas.dat e outros arquivos temporários
🧪 Exemplo de uso
text
Opções: comprimento 12, maiúsculas, minúsculas, números, símbolos.
Senha gerada: aB3#kL9$mQ2@
Força: FORTE
Salvando para "GitHub" → OK.

