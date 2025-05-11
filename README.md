# KDDTrain+ Veriseti ile Ağ Trafiği Analizi

## Proje Açıklaması

Bu proje, KDDTrain+ veri seti kullanılarak gerçekleştirilmiş bir ağ trafiği analiz uygulamasıdır. Amaç, veri seti üzerinde çeşitli ön işleme, analiz ve görselleştirme adımları gerçekleştirerek, ağ trafiğinde anomali tespiti ve istatistiksel içgörülerin elde edilmesidir.

## İçerik

Notebook içerisinde aşağıdaki adımlar gerçekleştirilmiştir:

1. **Kütüphane Yüklemeleri:**
   - `numpy`, `pandas`, `matplotlib.pyplot`, `seaborn` gibi temel veri işleme ve görselleştirme kütüphaneleri projeye dahil edilmiştir.
   - Uyarılar bastırılmış, grafik konfigürasyonları ayarlanmıştır.

2. **Veri Yükleme:**
   - `KDDTrain+.txt` isimli veri dosyası pandas kullanılarak yüklenmiştir.
   - Veri, `df` isimli DataFrame'e aktarılmıştır.

3. **Kolon Tanımlamaları:**
   - Veri setine ait sütun isimleri manuel olarak tanımlanmıştır.
   - Bu kolonlar saldırı tespiti ile ilgili birçok ağ özelliğini (örneğin: `src_bytes`, `dst_bytes`, `num_failed_logins`, `hot`, `serror_rate`, `rerror_rate`, vb.) içermektedir.

4. **Veri Görselleştirme ve İstatistiksel Analiz (Notebook'un ilerleyen hücrelerinde yer alabilir):**
   - Seaborn ve Matplotlib ile istatistiksel grafiklerin üretilmesi hedeflenmiştir.
   - Sınıfların dağılımı, saldırı tespiti ve diğer nitel analizler için uygun görseller oluşturulmuştur.

## Gereksinimler

Aşağıdaki Python kütüphanelerinin yüklü olması gerekmektedir:

```bash
pip install numpy pandas matplotlib seaborn
```
## Kullanım
  - main.ipynb dosyasını Jupyter Notebook ortamında açınız.

  - Notebook içerisindeki hücreleri sırayla çalıştırarak analizi gerçekleştirebilirsiniz.

  - Gerekirse KDDTrain+.txt dosyasının bulunduğunuz dizinde olması gerekmektedir.


## Not
Bu proje, ağ trafiği üzerinde temel düzeyde analiz gerçekleştirmek isteyen kullanıcılar için başlangıç seviyesinde bir çerçeve sunmaktadır. Daha ileri seviye analizler (örneğin makine öğrenmesi ile saldırı sınıflandırması) bu altyapı üzerine inşa edilebilir.
