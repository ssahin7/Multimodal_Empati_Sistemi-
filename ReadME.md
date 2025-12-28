🎧 Multimodal Empatik Chatbot
📖 Proje Hakkında

Bu proje, ses tabanlı duygu tanıma ve doğal dil işleme (LLM) tekniklerini birleştiren bir multimodal empatik chatbot sistemidir.
Sistem, kullanıcıdan alınan ses verisini analiz ederek duygu durumunu tahmin eder ve ardından empatik yanıtlar üretir.

Sistem üç temel aşamadan oluşur:

🎤 Ses Analizi: Kullanıcının ses verisi SVM tabanlı model ile analiz edilir ve duygu sınıfı belirlenir.

📝 Metin Üretimi: Duygu sınıfına göre LLM (LoRA ile fine-tuned GPT-2) kullanılarak yanıtlar üretilir.

📊 Performans Ölçümü: Üretilen yanıtların empati skoru, kelime çeşitliliği ve uzunluğu ölçülür, görselleştirilir.

✨ Özellikler

🎧 Ses Tabanlı Duygu Tanıma: RAVDESS veri seti ile SVM tabanlı sınıflandırma.

💬 Empatik Yanıt Üretimi: LoRA ile fine-tuned GPT-2 modelinden duyguya uygun yanıtlar.

🔗 Multimodal Analiz: Ses ve metin verileri birlikte değerlendirilir.

📈 Performans Görselleştirmesi: Empati skoru, kelime uzunluğu, kelime çeşitliliği grafiklerle sunulur.

🛠 Kurulum
Gereksinimler

Python 3.10+

GPU önerilir (Colab üzerinden CUDA destekli GPU kullanılabilir)

Kütüphaneler:
pip install torch torchvision torchaudio transformers peft scikit-learn pandas numpy matplotlib seaborn tqdm gradio

Veri Seti

RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song) kullanılmıştır.

Sebep: Dengeli, etiketlenmiş ve farklı duygular için kaliteli ses örnekleri içerir.

Model

Base Model: ytu-ce-cosmos/turkish-gpt2-large

Fine-Tuning: LoRA (Low-Rank Adaptation)

Sebep: Model boyutu ve eğitim maliyetini düşürürken performansı korur.

🔧 Proje Modülleri ve Kullanım Sebepleri

🐍 Python: Kodun ana dili, veri işleme ve ML kütüphaneleri için uygun.

⚡ PyTorch: Derin öğrenme modelleri ve LoRA için GPU desteği.

🤗 Transformers & PEFT: LLM ve fine-tuning işlemleri.

📊 Scikit-Learn: SVM tabanlı ses duygu sınıflandırması.

📈 Matplotlib & Seaborn: Performans grafiklerinin görselleştirilmesi.

⏳ TQDM: İşlem ilerleme çubuğu ile kullanıcı deneyimi.

🌐 Gradio: Basit web arayüzü ile model demo ve test.
📊 Model Performansı

Örnek performans değerleri:

Ortalama Empati Skoru: 0.154

Ortalama Kelime Sayısı: 101.2

Ortalama Benzersiz Kelime: 55.0

Kelime Çeşitliliği: 0.543

Not: Modelin performansı, mevcut veri ve LoRA ile yapılan fine-tuning sayesinde sınırlı maliyet ile oldukça tatmin edicidir.

🔮 Gelecek Çalışmalar (Future Works)

Daha büyük ve çeşitli veri setleri ile empati ve çeşitlilik artırılabilir.

Görsel verilerle multimodal destek (yüz ifadeleri).

LoRA yerine QLoRA veya PEFT optimizasyonları ile performans iyileştirmesi.

Güçlü GPU/TPU altyapısı ile latency ve yanıt kalitesinin artırılması.

Kullanıcı geri bildirimi ile empati skoru optimize edilerek model adaptasyonu.



Veri Seti aşağıdaki linkte verilmiştir .

Not:https://drive.google.com/drive/folders/1-Twl4GiWAPNwNpNnLgzeHdYYDhd2aA7v?usp=sharing
Github Link:https://github.com/ssahin7/Multimodal_Empati_Sistemi-
