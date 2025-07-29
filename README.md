## 🧠 Workflow 1: AI Agent (RAG ile Cevap Üretimi)

AI Agent Workflow

- **Webhook**: Kullanıcıdan POST ile soru alır
- **AI Agent**: Mistral Chat Model + Pinecone + Memory ile RAG yapar
- **Mistral Cloud Chat Model**: Chat LLM olarak kullanılır
- **Pinecone Vector Store**: Embed edilmiş dokümanları tarar
- **Respond to Webhook**: Cevap dış dünyaya döner

## 🗃️ Workflow 2: Dokümanları Embedding ile Vektör Veritabanına Aktarma



- **Google Drive**: Belgeleri arar ve indirir
- **Recursive Text Splitter**: Uzun metinleri parçalara ayırır
- **Embeddings Mistral Cloud**: Her parçayı embed eder
- **Pinecone Vector Store**: Embed'leri vektör veritabanına kaydeder

## 🚀 Nasıl Kullanılır

1. n8n kur (self-hosted ya da cloud)
2. `workflows/` klasöründeki JSON dosyalarını n8n'e içe aktar
3. API Key'lerini gir:
   - Mistral API Key
   - Pinecone API Key
   - ElevenLabs API Key
4. Google Drive'dan verileri yükle
5. Voice agent'ı çalıştırarak test et!

🧠 **Not**: Proje restoran verileriyle yapılmıştır, farklı sektörlere uyarlamak oldukça kolaydır.
