# Projeto LangFlow + Ollama + ChromaDB

## 📌 Descrição
Este projeto tem como objetivo:

- Extrair dados de arquivos PDF

- Transformar e indexar os textos usando embeddings locais

- Permitir que uma IA local responda perguntas sobre os documentos

- Tudo é executado localmente utilizando LangFlow, Ollama e ChromaDB.

## 🛠 Tecnologias utilizadas

LangFlow — Interface para criar fluxos de IA visualmente

Ollama — Execução de modelos LLM localmente

ChromaDB — Armazenamento vetorial para embeddings

PyMuPDF — Leitura e extração de texto de PDFs

# 📂 Estrutura de Arquivos
.
├── requirements.txt     # Dependências do projeto
├── README.md            # Documentação
└── fluxos/              # Arquivos exportados do LangFlow (.json)

# Como Rodar o Projeto

## 1. Criar ambiente virtual

python -m venv venv

source venv/bin/activate  # Mac/Linux

venv\Scripts\activate     # Windows

## 2. Instalar dependências

pip install -r requirements.txt

## 3. Instalar e iniciar o Ollama

siga as instruções: https://ollama.com/download

ollama serve

## 5. Baixar os modelos necessários

ollama pull gemma3:4b

ollama pull nomic-embed-text

## 5. Rodar o LangFlow

langflow run

O Localhost vai aparecer no terminal ou LangFlow abrirá no navegador.

Carregue o fluxo (.json) clicando em "upload a flow " e execute o projeto.

## 6. Dentro do LangFlow

Inserir os PDFs desejados no bloco "File", executar o ChromaDB

Iniciar o chat clicando em "Playground"

