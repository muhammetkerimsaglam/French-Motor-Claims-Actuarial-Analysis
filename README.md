# Fransa Motorlu Araç Sigorta Hasarları Raporu (French Motor Claims Report)

Bu proje, Fransa motorlu araç sigortaları pazarını temsil eden 678.013 poliçelik veri seti üzerinde aktüeryal risk analizi, tarife modellemesi ve istatistiksel hipotez testlerini içermektedir.

## 🚀 Proje Yapısı
* **1. Aşama (Python):** Keşifçi Veri Analizi (EDA), veri görselleştirme ve portföyün Sıfır Yığılmalı (Zero-Inflated) yapısının saptanması.
* **2. Aşama (R Studio):** Ki-Kare Bağımsızlık Testleri, Poisson GLM, Aşırı Dağılım (Overdispersion) Testi, Negatif Binom Regresyonu ve Olasılık Oranı Testleri (Likelihood Ratio Test).

## 📊 Öne Çıkan Bulgular ve Aktüeryal Çıkarımlar
* Veri setinde varyansın ortalamadan büyük olduğu ($dispersion = 1.3049$) kanıtlanmış ve standart Poisson model yerine **Negatif Binom Regresyon** modeline geçilmiştir.
* Poliçe sürelerinin (`offset(log(Exposure))`) modele dahil edilmesinin model uyumunu ve açıklama gücünü radikal biçimde artırdığı ($Chisq = 854.03$) ispatlanmıştır.
* Poisson modelinde anlamlı çıkan araç yakıt türü değişkeninin, çok değişkenli Negatif Binom modelinde diğer risk faktörleri kontrol edildiğinde anlamsızlaştığı saptanmıştır.

## 🛠️ Kullanılan Teknolojiler
* **Python:** Pandas, Matplotlib, Seaborn
* **R kütüphaneleri:** MASS, pscl, lmtest, AER

---
*Detaylı analiz adımlarına ve grafik yorumlarına repository içerisindeki **French Motor Claims Report.pdf** dosyasından ulaşabilirsiniz.*
