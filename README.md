# :sound: Deep Fake Voice Detection
---

<br/>
<i>Bu çalışma, aiseclab.org bünyesinde <b>tech-titan</b> ekibi projesi olarak geliştirilmiştir.</i>

# :sound: Amaç
---

* Derin öğrenme yöntemleri kullanılarak sahte ses dosyalarının tespit edilmesi sağlanacaktır. Kullanılan veri setlerine aşağıdaki bağlantılardan ulaşabilirsiniz.<br/><br/>
1. [DEEP-VOICE: DeepFake Voice Recognition](https://www.kaggle.com/datasets/birdy654/deep-voice-deepfake-voice-recognition)<br/>
2. [ASVspoof 2019](https://www.kaggle.com/datasets/awsaf49/asvpoof-2019-dataset)
<br/>

# :sound: Ekip Üyeleri
---

**Danışman**: [Atakan AK](https://github.com/akatakan)
<br/>

1. [İrem Uslu](https://github.com/irem6142)
2. [Gülzade Evni](https://github.com/GulzadeEvni)
3. [Kübra Arslan](https://github.com/kbrars)
4. [Mustafa Yavuz](https://github.com/mstkyvz)
<br/>

# :sound: Gerekli Kütüphaneler
---

* Kullanılan kütüphaneler ve versiyon bilgileri aşağıda belirtilmiştir.

```shell
librosa==0.10.1
matplotlib==3.8.0
numpy==1.23.1
opendatasets==0.1.22
pandas==1.5.3
resampy==0.4.2
scikit_learn==1.4.0
seaborn==0.13.0
tensorflow==2.15.0
transformers==4.37.2
```
<br/>

# :sound: Kurulum
---

* Gerekli paketleri kurduktan sonra uygulamayı kullanmaya başlayabilirsiniz.

```python3
# Gerekli kütüphaneleri kurmak için
pip install -r requirements.txt
# Ana uygulamayı çalıştırmak için
cd flaskappvoice
python3 as.py
```
<br/>

# :sound: Modeller
---

* Problemi çözmek için LSTM, CNN ve Wav2Vec modelleri kullanılmıştır. Kullanılam modellere ait veriler aşağıda belirtilmiştir.

| Model | Dataset | Train Accuracy | Train Loss | Val Accuracy | Val Loss | 
| ----- | ------- | -------------- | ---------- | ------------ | -------- |
| LSTM  | DEEP-VOICE | 93.23% | 18.17% | 89.58% | 26.53% |
| CNN   | DEEP-VOICE | 98.96% | 15.38% | 66.67% | 62.35% |
| Wav2Vec | Pretrained | Pretrained | Pretrained | Pretrained | Pretrained |
