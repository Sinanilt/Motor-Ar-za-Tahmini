# Motor-Ar-za-Tahmini
Gerçek verilerle motor arıza süresi tahmin projesi
# Motor Arıza Tahmin Projesi

Bu projede, NASA'nın CMAPSS veri seti kullanılarak uçak motorlarının ne zaman arızalanacağını tahmin etmeye yönelik bir makine öğrenmesi modeli geliştirildi.  
Amaç, sensör verileri üzerinden motorun kalan ömrünü (RUL - Remaining Useful Life) tahmin etmek.

---

## Kullanılan Yöntem ve Araçlar

- Python (Google Colab)
- Pandas, Numpy (veri işleme)
- Scikit-learn (makine öğrenmesi)
- Matplotlib (grafik çizimi)
- Random Forest Regressor (tahmin modeli)

---

## Veri Seti

NASA tarafından sağlanan CMAPSS veri seti:
- `train_FD001.txt`: Eğitim verisi
- `test_FD001.txt`: Test motorları
- `RUL_FD001.txt`: Gerçek kalan ömür verisi

---

## Proje Adımları

1. Veri yükleme ve temizleme
2. Sensörlerin analizi ve normalizasyonu
3. RUL (Remaining Useful Life) hesaplama
4. Model eğitimi (Random Forest)
5. Test verisiyle tahmin
6. Gerçek ve tahmin karşılaştırması

---

## Örnek Sonuçlar

| Motor | Gerçek RUL | Tahmin Edilen RUL |
|-------|------------|-------------------|
| 1     | 112        | 170               |
| 2     | 98         | 153               |
| 3     | 69         | 58                |

Ortalama mutlak hata (MAE): ~29 cycle  
R² skoru: 0.62

---

## Nasıl Çalıştırılır?

1. Colab ortamında `.ipynb` dosyasını açın  
2. Eğitim ve test verilerini yükleyin  
3. Kod bloklarını sırasıyla çalıştırın  
4. Tahminleri ve model performansını inceleyin

---

## Not

Veri seti bağlantısı:  
[https://www.kaggle.com/datasets/behrad3d/nasa-cmapss](https://www.kaggle.com/datasets/palbha/cmapss-jet-engine-simulated-data?resource=download)
