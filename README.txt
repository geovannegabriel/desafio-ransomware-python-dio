Arquivos do Projeto

- `encrypter.py`: criptografa todos os arquivos da pasta atual (exceto os próprios scripts e a chave).
- `decrypter.py`: descriptografa os arquivos da mesma pasta, usando a chave salva.
- `key.key`: chave gerada automaticamente na primeira execução e utilizada para criptografia e descriptografia.

---

## Como Funciona

1. O script `encrypter.py` verifica se existe uma chave:
   - Se não existir, gera uma nova (`key.key`)
   - Criptografa todos os arquivos do diretório

2. O script `decrypter.py` usa essa mesma chave para reverter o processo.

---

## ▶ Executando o Projeto

1. Certifique-se de ter a biblioteca `cryptography` instalada:
```bash
pip install cryptography
```

2. Execute o encriptador:
```bash
python encrypter.py
```

3. Para descriptografar:
```bash
python decrypter.py
```
