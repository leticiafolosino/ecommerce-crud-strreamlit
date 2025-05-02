
# 🛒 E-Shop Brasil – CRUD com MongoDB e Streamlit

Este projeto é uma aplicação CRUD desenvolvida para a disciplina *Advanced Databases and Big Data*, com foco em soluções modernas de visualização e gerenciamento de dados utilizando **MongoDB**, **Docker** e **Streamlit**.

---

## 📌 Descrição

A aplicação simula o sistema interno da empresa fictícia **E-Shop Brasil**, permitindo o gerenciamento de dados de produtos (Cadastro, Leitura, Atualização e Exclusão) de forma interativa e escalável, com suporte a grandes volumes de dados.

---

## 🚀 Tecnologias Utilizadas

- Python 3.10+
- MongoDB
- Streamlit
- Docker & Docker Compose
- Faker (para geração de dados falsos)
- Pymongo (integração com MongoDB)

---

## 🧱 Estrutura do Projeto

```
ecommerce-crud-streamlit-main/
│
├── app.py                  # Interface principal com Streamlit
├── db/
│   └── database.py         # Funções de conexão e operações com MongoDB
├── utils/
│   └── inserir_dados.py    # Script de inserção de 1 milhão de produtos com Faker
├── Dockerfile
├── docker-compose.yml      # Configuração dos containers MongoDB
└── README.md               # Este arquivo
```

---

## 🐳 Como Executar com Docker

1. **Clone o projeto**:
```bash
git clone https://github.com/seu-usuario/ecommerce-crud-streamlit-main.git
cd ecommerce-crud-streamlit-main
```

2. **Execute os containers:**
```bash
docker-compose up --build
```

3. Acesse o Streamlit no navegador:
```
http://localhost:8501
```

---

## 📥 Inserir 1 Milhão de Dados

Após iniciar o MongoDB com Docker:

```bash
pip install faker pymongo
python utils/inserir_dados.py
```

Esse script gerará 1.000.000 de produtos fictícios com `Faker` e inserirá no MongoDB.

---

## 📹 Demonstração (Vídeo)

➡️ [Link do vídeo explicativo no YouTube](https://youtu.be/seu-video)

*O vídeo demonstra a execução dos contêineres, navegação na aplicação e uso das funções CRUD.*

---

## ✅ Funcionalidades

- [x] Cadastro de produtos
- [x] Listagem de produtos
- [x] Atualização de informações
- [x] Exclusão de produtos
- [x] Inserção massiva de dados com Faker
- [x] Containerização com Docker

---

## 🧑‍💻 Autor

**Jhonatan Oliveira**

Projeto acadêmico desenvolvido para a UNIFecaf – Abril de 2025.
