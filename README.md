# SEYAHAT VE VİZE REHBERİ: RAG UYGULAMASI

Bu proje, PDF belgelerindeki metinlerden bilgi çıkarmak ve sorgulama ile benzer içerikleri hızlı bir şekilde elde etmek için LangChain kütüphanesini ve HuggingFace embedding modellerini kullanmaktadır. Proje, PDF dosyalarından veri çekip, bu verileri vektörleştirerek bir veritabanında saklar. Ardından, kullanıcının sorgularına yanıt veren bir RAG (Retrieval-Augmented Generation) zinciri kurar.

## Kullanılacak Platformlar

- **Google Colab**: Kodların çalıştırılması ve kaynakların sağlanması için Google Colab kullanılmıştır.
- **Python**: Python 3.x kullanılır.
- **Google Drive**: PDF dosyalarını yüklemek ve saklamak için Google Drive kullanılmıştır.


### Python Kütüphaneleri

Bu proje için aşağıdaki Python kütüphanelerine ihtiyaç vardır:

- **langchain**: LangChain kütüphanesini kullanarak metinleri işlemeye olanak sağlar.
- **sentence-transformers**: Metin vektörleri için kullanılan model.
- **chromadb**: Vektör veritabanını yönetmek için kullanılır.
- **llama-cpp-python**: LlamaCpp API'si ile LLM (Language Model) kullanımı.
- **pypdf**: PDF dosyalarını okumak için kullanılır.
- **transformers**: HuggingFace modellerini kullanabilmek için gereklidir.
- **textwrap**: Metin biçimlendirme ve düzenleme için kullanılır.

  ## Versiyonlar

- **langchain**: 0.0.200
- **sentence-transformers**: 2.2.0
- **chromadb**: 0.3.5
- **llama-cpp-python**: 0.1.13
- **pypdf**: 3.0.1
- **transformers**: 4.24.0
- **textwrap**: Python standard library (varsayılan olarak yüklü)

Gerekli kütüphaneleri yüklemek için aşağıdaki komutu kullanabilirsiniz:

```bash
!pip install langchain sentence-transformers chromadb llama-cpp-python langchain_community pypdf transformers
```

## API Anahtarları
HuggingFace API Key: HuggingFace modellerini kullanabilmek için geçerli bir HuggingFace API anahtarına sahip olmanız gereklidir. API anahtarınızı aşağıdaki adımlarla alabilirsiniz:
HuggingFace hesabınızı oluşturun: https://huggingface.co/
API anahtarınızı profil sayfanızdan alın.
Anahtarınızı güvenli bir şekilde HUGGINGFACE_API_KEY olarak ortam değişkeninde ayarlayabilirsiniz.






