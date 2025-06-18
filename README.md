# 🧠 Introdução ao Processamento de Linguagem Natural (PLN) com Python

Este projeto é uma prática introdutória ao **Processamento de Linguagem Natural (PLN)**, usando Python e o Google Colab. A proposta é ler um corpus textual (`Ubirajara.txt`), analisar seu conteúdo e buscar palavras com contexto.

---

## 🎯 Objetivos

- Ler e interpretar um corpus de texto.
- Criar uma função de busca por palavras com contexto.
- Contar quantas vezes a palavra aparece.
- Trabalhar com tratamento de erros e boas práticas em manipulação de arquivos.

---

## 📚 Tecnologias e Conceitos Utilizados

- **Python 3**
- **Google Colab** (ou VS Code)
- Manipulação de strings (`.lower()`, `.replace()`, `.find()`)
- Leitura de arquivos `.txt`
- Tratamento de exceções (`try`, `except`)
- Busca case-insensitive com retorno de contexto

---

## 📁 Estrutura do Projeto

- `ler(arquivo)`: Função que lê um arquivo `.txt` com tratamento de erros.
- `buscador(alvo, texto)`: Função que busca uma palavra e exibe os trechos do texto onde ela aparece.
- Uso de `files.upload()` para fazer upload de arquivos no Google Colab.

---

## ✅ Exemplo de Uso

```python
from google.colab import files
uploaded = files.upload()

texto = ler('Ubirajara.txt')
ocorrencias, resumo = buscador('peito', texto)

for trecho in ocorrencias:
    print(trecho)

print(resumo)
```

---

## 📌 Saída Esperada

```
...em seu peito ardia um sentimento nobre...
...ferido no peito, caiu ao chão...
--- A palavra 'peito' se repetiu 2 vezes. ---
```

---

## 🛠️ Etapas Futuras (conforme o roteiro)

- **Limpeza do Corpus**: remoção de pontuações, números e stopwords.
- **Tokenização e Análise de Frequência**: calcular quais são as palavras mais comuns.
- **Vocabulário e Riqueza Textual**: avaliar a diversidade linguística do texto.

---

## 📌 Requisitos

- Ter um arquivo `.txt` como entrada (ex: `Ubirajara.txt`)
- Python 3 (Google Colab já vem pronto)


