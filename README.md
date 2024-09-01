# Müşteri Segmentasyonu ve CLTV Hesaplama Projesi

Bu proje, E-Customer Data veri seti üzerinde müşteri segmentasyonu sağlamak ve müşteri yaşam boyu değerini (CLTV) hesaplamak amacıyla gerçekleştirilmiştir. Proje, Python kullanarak veri analizi, RFM (Recency, Frequency, Monetary) analizi ve CLTV hesaplama adımlarını içermektedir.

## İçindekiler
- [Proje Hakkında](#proje-hakkında)
- [Veri Seti](#veri-seti)
- [Kullanılan Kütüphaneler](#kullanılan-kütüphaneler)
- [Adımlar](#adımlar)
- [Sonuçlar ve Yorumlar](#sonuçlar-ve-yorumlar)
- [Kurulum](#kurulum)
- [Katkıda Bulunanlar](#katkıda-bulunanlar)

## Proje Hakkında
Bu projede, müşteri davranışlarını analiz ederek segmentasyon yapılmış ve her segment için tahmini müşteri yaşam boyu değeri hesaplanmıştır. Segmentasyon, RFM analizi ile gerçekleştirilmiştir ve müşteri grupları oluşturulmuştur. CLTV hesaplamaları ise Beta-Geometrik / Gamma-Gamma modeli kullanılarak yapılmıştır.

## Veri Seti
Veri seti, müşterilerin alışveriş geçmişini içermektedir. Her bir işlem, fatura numarası, müşteri kimliği, ürün miktarı, ürün birim fiyatı ve işlem tarihi gibi bilgileri içermektedir.

## Kullanılan Kütüphaneler
Projede kullanılan başlıca Python kütüphaneleri:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `lifetimes`

## Adımlar
1. **Veri Temizleme:** Eksik veriler çıkarıldı, iptal edilen siparişler ve anormal değerler temizlendi.
2. **RFM Analizi:** Müşterilerin son işlem tarihi, işlem sayısı ve toplam harcama tutarına göre segmentasyon yapıldı.
3. **CLTV Hesaplama:** Beta-Geometrik / Gamma-Gamma modeli ile müşteri yaşam boyu değeri hesaplandı.
4. **Segmentasyon:** RFM ve CLTV değerlerine göre müşteriler segmentlere ayrıldı.

## Sonuçlar ve Yorumlar
- **RFM Segmentasyonu:** Müşteriler farklı RFM skorlarına göre segmentlere ayrılmıştır. Örneğin, "Champions" segmentinde yer alan müşteriler en yüksek değere sahiptir.
- **CLTV Hesaplamaları:** CLTV değerlerine göre müşteriler 4 farklı segmentte gruplandırılmıştır: A (En yüksek değer), B, C, D (En düşük değer).
- **Genel Yorum:** Proje, müşteri segmentasyonu ve CLTV hesaplamaları konusunda önemli içgörüler sağlamıştır. Yüksek CLTV değerine sahip müşterilere yönelik stratejiler geliştirilerek, şirketin gelir potansiyeli artırılabilir.

## Kurulum
Projeyi yerel bilgisayarınızda çalıştırmak için aşağıdaki adımları takip edebilirsiniz:

1. Bu depoyu klonlayın: `git clone https://github.com/kullanici_adiniz/musteri-segmentasyonu-cltv`
2. Gerekli kütüphaneleri yükleyin: `pip install -r requirements.txt`
3. Jupyter Notebook veya başka bir IDE üzerinde `main.ipynb` dosyasını çalıştırın.

## Katkıda Bulunanlar
Bu projeyi geliştiren: [Adınız Soyadınız](https://www.linkedin.com/in/kullanici-adiniz)
