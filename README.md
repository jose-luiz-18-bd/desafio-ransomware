# 🔐 Desafio Ransomware (Projeto Educacional)

Este projeto simula o funcionamento básico de um ransomware com propósitos **exclusivamente educacionais**. Ele realiza a **criptografia** de um arquivo de texto e sua posterior **descriptografia** usando o algoritmo AES em modo CTR com a biblioteca `pyaes`.

> ⚠️ **Aviso**: Este projeto é apenas para fins de aprendizado. Nunca use este tipo de técnica para fins maliciosos ou ilegais.

---

## 🗂 Estrutura do Projeto

```
DESAFIO-RANSOMWARE/
│
├── test.txt               # Arquivo de texto original, legível
├── encrypter.py           # Script que criptografa o arquivo
├── decrypter.py           # Script que descriptografa o arquivo
└── README.md              # Este arquivo de documentação
```

---

## 🔧 Requisitos

- Python 3.x
- Biblioteca `pyaes`

### Instalando o `pyaes`:

```bash
pip install pyaes
```

---

## 🔒 Como funciona

### 1. Criptografia (`encrypter.py`)

- Lê o conteúdo do arquivo `test.txt`
- Remove o arquivo original
- Criptografa os dados com AES/CTR
- Salva o conteúdo criptografado em `test.txt.ransomwaretroll`

### 2. Descriptografia (`decrypter.py`)

- Lê o conteúdo do arquivo `test.txt.ransomwaretroll`
- Remove o arquivo criptografado
- Descriptografa os dados com a mesma chave
- Salva o conteúdo original de volta em `test.txt`

---

## 📜 Exemplo de Conteúdo

### Antes da criptografia (`test.txt`):
```
Este Arquivo está legível
Hello World
Uma Vez Flamengo, sempre Flamengo!!!
```

### Após a criptografia (`test.txt.ransomwaretroll`):
```
(dados binários criptografados, ilegíveis)
```

### Após a descriptografia (`test.txt`):
```
Este Arquivo está legível
Hello World
Uma Vez Flamengo, sempre Flamengo!!!
```

---

## 🔑 Sobre a chave de criptografia

A chave usada é:

```python
key = b"testersansomwares"
```

> A chave deve ser **idêntica** nos dois scripts para que a descriptografia funcione corretamente.

---

## ⚠️ Aviso Legal

Este código **não deve ser utilizado em ambientes de produção** ou em computadores de outras pessoas. Seu propósito é unicamente demonstrar, de forma controlada, como funciona a criptografia de arquivos.

---

## 🧠 Aprendizado

Este projeto pode te ajudar a entender:

- Conceitos básicos de criptografia simétrica
- Como manipular arquivos binários em Python
- Como aplicar o modo CTR com AES usando a biblioteca `pyaes`
- Boas práticas de segurança e ética em cibersegurança

---

## 📄 Licença

Distribuído sob a licença MIT. Consulte `LICENSE` para mais detalhes.
