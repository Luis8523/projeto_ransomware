# 🔐 Projeto: Criptografia de Arquivos com Python 

Este projeto implementa um sistema de **criptografia e descriptografia de arquivos** usando a biblioteca `cryptography` com o algoritmo simétrico `Fernet`. Foi desenvolvido como prática de segurança digital, manipulação de arquivos e uso de chave única para proteção de dados confidenciais.

---

## 🧠 Funcionalidades

- ✔️ Geração automática de chave criptográfica (`key.key`)
- ✔️ Criptografia de arquivos dentro da pasta `arquivos/`
- ✔️ Descriptografia dos arquivos usando a mesma chave
- ✔️ Verificação se o conteúdo foi criptografado ou decifrado com sucesso
- ✔️ Ignora pastas internas e trata arquivos válidos individualmente
- ✔️ Mensagens de feedback no terminal para cada operação

---


---

## 🛠️ Instalação da biblioteca necessária

Antes de executar os scripts, instale o pacote `cryptography`:


pip install cryptography
# ou, se necessário:
pip3 install cryptography


🚀 Como usar
1. Crie a pasta de arquivos e adicione uma mensagem original
mkdir -p arquivos
nano arquivos/dados.txt
No editor nano, digite sua mensagem sensível e salve com:
- CTRL + O → Enter
- CTRL + X

2. Execute o criptografador

python3 encrypter.py
Isso irá gerar a chave key.key, criptografar os arquivos dentro de arquivos/, e exibir uma mensagem para cada arquivo:
✅ Arquivo 'dados.txt' criptografado com sucesso!

3. Verifique se o conteúdo está cifrado

cat arquivos/dados.txt

Se aparecer algo como:
gAAAAAB... (base64 cifrado)

A criptografia foi aplicada com sucesso!

4. Execute o descriptografador

python3 decrypter.py
ira aparecer :
✅ Arquivo 'dados.txt' decifrado com sucesso!

5. Verifique a recuperação da mensagem original

cat arquivos/dados.txt
Agora aparecerá novamente o texto legível que foi salvo inicialmente.

📌 Detalhes técnicos
- Linguagem: Python 3
- Biblioteca: 
- Algoritmo: Fernet (AES 128 com autenticação embutida)
- Tipo de chave: Simétrica, codificada em base64 (key.key)
- Segurança: A chave key.key é essencial para recuperar os arquivos — proteja-a como ouro 💎


🕵️‍♂️ Mensagem criptografada


![Minha Imagem](https://github.com/user-attachments/assets/6a44e003-c8f5-48b8-9966-1965ca138855)


🔓 Mensagem descriptografada

<img width="409" height="53" alt="Image" src="https://github.com/user-attachments/assets/71dcaf5c-f20a-43a1-897d-e5bbc14e254e" />
