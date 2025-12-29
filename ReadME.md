# Project Name

Bu projeDE, Ses verileri işlenerek stress analizi yapılmış daha sonrada finetune edilmiş llm modeliyle strese uygun chatbot geliştirilmiştir.LLM uygulamasıdır.

## 🎯 Amaç
- Veri üzerinden anlamlı örüntüler çıkarmak
- Model eğitimi ve değerlendirme sürecini gerçekleştirmek
- Sonuçları görselleştirmek

## 🗂️ Proje Yapısı
- **data/**: Ham ve işlenmiş veriler
- **notebooks/**: Deneysel çalışmalar (EDA, eğitim)
- **src/**: Temiz ve modüler Python kodları
- **outputs/**: Model çıktıları ve grafikler

## 📊 Kullanılan Teknolojiler
- Python 3.x
- NumPy, Pandas
- Scikit-learn / PyTorch / TensorFlow
- Matplotlib, Seaborn
- Jupyter Notebook



## 📁 Proje Dosya Yapısı (Önerilen)


```text

├── data/
│   ├── dataset.csv        # Türkçe fine-tune verisi
│   └── README.md          # Veri seti açıklaması
│
├── notebooks/
│   └── LLMSpeech.ipynb    # Asıl eğitim notebook'u
│
├── model/
│   ├── model.safetensors  # Ana model ağırlığı
│   └── tokenizer.pkl     # Tokenizer veya ek objeler
│
└── .gitignore
