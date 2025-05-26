# 📖 Modelos baseados em prompt vs. Fine-tuning

---

## 1️⃣ Modelos baseados em prompt

**Zero-shot learning:**  
- O modelo recebe apenas o prompt com a tarefa, sem exemplos adicionais.  
- Exemplo:  

```
Resuma este texto em 3 linhas: [texto]
```

**Few-shot learning:**  
- O prompt inclui alguns exemplos para ajudar o modelo a entender o formato de saída esperado.  
- Exemplo: 

```
Resuma o texto a seguir em 3 linhas.
Exemplo 1:
Texto: "Exemplo de texto"
Resumo: "..."
Agora, Texto: "..."
```

✅ **Vantagens:**  
- Simples e rápido para criar protótipos.  
- Não exige dados rotulados para treinamento.  
- Ideal para MVPs ou tarefas gerais.

❌ **Limitações:**  
- Limite de tokens no prompt/contexto.  
- Tarefas muito especializadas podem gerar respostas imprecisas.

---

## 2️⃣ Modelos customizados (fine-tuning ou instrução)

**Fine-tuning:**  
- Ajusta um modelo pré-treinado com exemplos rotulados específicos para a tarefa ou domínio.  
- Necessita de um dataset robusto e balanceado.

**Modelos de Instrução:**  
- Alguns LLMs são otimizados para "seguir instruções" (ex.: GPT-3.5 Instruct, Llama 2 Chat, Mistral Instruct).  
- Muitas vezes, basta escrever um prompt claro para resultados superiores.

✅ **Vantagens:**  
- Melhor performance em tarefas específicas.  
- Respostas mais coerentes e adaptadas ao domínio.

❌ **Desvantagens:**  
- Requer mais recursos (GPU, dados, etc.).  
- Risco de overfitting se o fine-tuning for mal calibrado.

---

## 🔄 Comparativo rápido

| Abordagem         | Vantagens                                    | Desvantagens                     | Melhor uso                |
|--------------------|----------------------------------------------|-----------------------------------|---------------------------|
| Prompt-based       | Rápido, sem necessidade de dados rotulados   | Contexto limitado, menos preciso | Prototipagem, MVPs       |
| Fine-tuning        | Altamente adaptável ao domínio               | Demanda dados e infra            | Tarefas complexas e específicas |

---

## 🔗 Recursos úteis

- [OpenAI Cookbook](https://github.com/openai/openai-cookbook)
- [HuggingFace Transformers](https://huggingface.co/docs/transformers/index)
- Artigos sobre zero-shot e few-shot learning.