# 🧠 Sentinela Neural

Um chatbot jurídico-operacional com IA generativa treinado para orientar policiais militares com base no manual oficial da PMMG.

---

## 📌 Sobre o Projeto

**Sentinela Neural** é um assistente virtual construído com IA generativa (Gemini 2.0) e busca semântica (FAISS), capaz de interpretar perguntas feitas por policiais militares e responder com base no conteúdo do documento institucional da PMMG, como o **DIAO – Diretriz de Ações Operacionais**.

O projeto foi desenvolvido na [Imersão IA 2025](https://www.alura.com.br) (Alura + Google), com foco em demonstrar uma aplicação prática, ética e de impacto social do uso de modelos de linguagem (LLMs) no apoio a agentes públicos em campo.

---

## ⚙️ Tecnologias Utilizadas

- 🤖 [Google Gemini 2.0 Flash](https://ai.google.dev/)
- 🔎 FAISS (Facebook AI Similarity Search)
- 🧠 HuggingFace Embeddings (`all-MiniLM-L6-v2`)
- 🧱 LangChain (RAG Pipeline)
- 📄 PyMuPDF (leitura e extração de PDF)
- 🐍 Python 3 (executável via Google Colab)

---

## 🚨 O que o Sentinela Neural faz?

✅ Recebe uma pergunta livre (ex: “Quais os procedimentos quando a vítima é uma mulher em situação de violência doméstica?”)  
✅ Consulta um documento institucional real da PMMG (DIAO)  
✅ Encontra os blocos mais relevantes com FAISS  
✅ Gera uma resposta clara, técnica e fundamentada com Gemini  
✅ Adiciona complementos automáticos em temas críticos (como ameaça vs. vias de fato)  
✅ Mantém o **contexto da conversa** para responder perguntas encadeadas

---

## ▶️ Como Executar

1. Acesse o notebook `SENTINELA-NEURAL.ipynb` via Google Colab  
2. O script automaticamente:
   - Baixa o documento institucional (PDF)
   - Processa os blocos temáticos
   - Indexa o conteúdo com FAISS
   - Inicia um chat interativo via terminal

3. Digite sua pergunta e receba uma resposta com base na legislação e diretrizes da PMMG.

🔐 Requisito

Antes de executar, crie uma variável de ambiente chamada:
GOOGLE_API_KEY
Essa variável deve conter sua chave de API do Google AI Studio, necessária para utilizar o modelo Gemini 2.0.

---

## 🧪 Exemplos de Perguntas

- O que fazer quando há um menor envolvido em tráfico?
- Qual natureza é mais grave, ameaça ou vias de fato?
- Em caso de violência doméstica, qual o procedimento?
- A desobediência é crime? E se for um civil?
- Quando a PM pode lavrar TCO?

---

## 📂 Estrutura do Projeto

```
📁 sentinela-neural/
├── SENTINELA-NEURAL.ipynb   # Notebook principal
├── DIAO.pdf                 # Documento institucional indexado
├── README.md                # Este arquivo
```

---

## 💡 Inspiração

Minha noiva Priscilla é policial militar há mais de 15 anos e recentemente foi promovida à sargento. Por ser uma policial muito dedicada, estudiosa e responsável, seus colegas sempre recorrem a ela para saber como proceder em diversas situações operacionais.

Agora que foi promovida, essas dúvidas dos colegas ficaram ainda mais frequentes — especialmente por parte dos novos recrutas que são subordinados a ela.

O **Sentinela Neural** foi criado para tornar mais eficiente o trabalho desses profissionais que são tão importantes para a sociedade. É essencial esse apoio operacional, pois em diversas situações de pressão o policial ainda assim deve seguir diretrizes e protocolos oficiais.

Oferecer uma ferramenta que ajude o policial a fazer seu trabalho com segurança jurídica não só reduz o tempo de decisão em campo, como também evita punições indevidas ou erros operacionais que possam comprometer o cumprimento da missão.

---

## 🏁 Criado por

**Luann**  
Projeto desenvolvido na Imersão IA 2025 — Alura + Google

---

## 📜 Licença

Este projeto é livre para fins educacionais. O uso da base institucional (DIAO) respeita os limites da transparência pública e não substitui a orientação jurídica oficial.
