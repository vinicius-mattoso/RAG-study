# 📚 Métodos de busca vetorial para RAG

## 🔎 1️⃣ O que são embeddings?

- Embeddings são representações vetoriais de textos, permitindo medir similaridade semântica.
- Modelos comuns: `sentence-transformers`, `OpenAI embeddings`, `HuggingFace embeddings`.

---

## 🛠️ 2️⃣ Métodos populares de recuperação

### ⚡ FAISS
- Biblioteca open-source da Meta (Facebook).
- Alta performance para busca vetorial local.
- Bom para protótipos e produção em ambientes controlados.

### 🌐 Pinecone
- Serviço gerenciado de indexação vetorial.
- Suporte a escalabilidade e alta disponibilidade.
- Ideal para grandes volumes e produção.

### 📦 ElasticSearch com vetores
- ElasticSearch 8+ suporta vetores e busca por similaridade.
- Útil se já usa ElasticSearch como base de dados.

### 🔗 Weaviate
- Banco de dados vetorial open-source.
- Integração com LLMs e APIs de embeddings.
- Bom para aplicações de IA escaláveis.

---

## 📝 3️⃣ Casos de uso e comparativo

| Método      | Melhor para                     | Facilidade de uso | Escalabilidade     |
|-------------|---------------------------------|-------------------|--------------------|
| FAISS       | Protótipos locais               | Alta              | Baixa-média        |
| Pinecone    | Produção em nuvem               | Alta              | Alta               |
| Elastic     | Quando já usa ElasticSearch     | Média             | Alta               |
| Weaviate    | Banco vetorial + LLM integrado  | Alta              | Alta               |

---

## 🧪 Próximos passos

✅ Crie um notebook básico (`notebooks/02_faiss_basics.ipynb`) para:  
1. Gerar embeddings de pequenos textos.  
2. Indexar e recuperar dados usando FAISS.  
3. Visualizar a similaridade entre consultas e resultados.

✅ Depois, compare com outras opções (Pinecone, Elastic, Weaviate).

---

## 🔗 Referências úteis

- [FAISS Documentation](https://faiss.ai)  
- [Pinecone Docs](https://docs.pinecone.io)  
- [ElasticSearch Vector Search](https://www.elastic.co/guide/en/elasticsearch/reference/current/dense-vector.html)  
- [Weaviate Docs](https://weaviate.io/developers/weaviate)  

---
