# 📚 Sistema RAG: Consulta Inteligente de Documentos
### Pesquisa e Desenvolvimento em LLMs - Laboratório TRIL (Embrapii)

Este repositório contém a implementação de um sistema de **Geração Aumentada por Recuperação (RAG)**. O projeto permite carregar documentos técnicos em PDF (como manuais ou livros), processá-los semanticamente e realizar perguntas e respostas baseadas exclusivamente no conteúdo fornecido.

---

## 🚀 Funcionalidades
* **Extração Inteligente**: Leitura de PDFs utilizando `PyMuPDF` para maior fidelidade de dados.
* **Processamento de Texto**: Divisão de documentos em *chunks* de 600 caracteres com sobreposição de 200 para manter o contexto.
* **Banco de Dados Vetorial**: Persistência local de embeddings utilizando o **ChromaDB**.
* **Integração com LLM**: Uso do modelo `GPT-3.5 Turbo` da OpenAI para síntese de respostas.
* **Prevenção de Alucinações**: O prompt é instruído a responder apenas com base no conhecimento recuperado do banco.

## 🛠️ Tecnologias Utilizadas
* [LangChain](https://python.langchain.com/) (Orquestração)
* [OpenAI API](https://openai.com/api/) (LLM & Embeddings)
* [ChromaDB](https://docs.trychroma.com/) (Vector Store)
* [PyMuPDF](https://pymupdf.readthedocs.io/) (Parsing de PDF)

## 📋 Pré-requisitos e Instalação

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
   cd seu-repositorio
