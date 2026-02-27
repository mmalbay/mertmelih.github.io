[Ana Sayfa](index.html) | **[Projelerim](projects.html)**
---

# Projelerim
## Derin Öğrenme Tabanlı Optik İnceleme ve Görsel Kusur Tespit Modülü
Modül, derin öğrenme mimarileri (YOLO) ve bilgisayarlı görü (OpenCV) tekniklerini kullanarak, PCB üzerindeki elektronik bileşenleri (direnç, diyot, MOSFET, entegre vb.) gerçek zamanlı olarak tanımlamak ve görsel kusurları otonom bir şekilde saptamayı amaçlamaktadır. Bu birim; eksik parça, yanlış dizilim, lehim köprüleri ve korozyon gibi fiziksel anomalileri yüksek çözünürlüklü görüntüler üzerinden analiz ederek, manuel gözle kontrol süreçlerini tamamen dijitalleştirmeyi ve hata tespitindeki insan faktörlü hata payını minimize etmeyi hedefler.  

<span class="proje-vurgu">Veri Seti Yönetimi ve Etiketleme:</span> Modelin başarımı için özgün bir veri seti oluşturulmuş; PCB bileşenleri (direnç, diyot, entegre, MOSFET vb.) manuel olarak etiketlenerek yüksek doğruluklu bir eğitim havuzu hazırlanmıştır.  
  

<span class="proje-vurgu">Veri Artırımı (Data Augmentation):</span> Modelin farklı ışık koşulları, perspektif açıları ve gürültü seviyelerinde kararlı çalışmasını sağlamak amacıyla; döndürme, parlaklık değişimi ve ölçeklendirme gibi artırım teknikleri uygulanarak modelin genelleme yeteneği (Robustness) optimize edilmiştir.  

<span class="proje-vurgu">YOLO ve OpenCV Entegrasyonu:</span> Gerçek zamanlı nesne tespiti için YOLO mimarisi kullanılmış; kamera verileri OpenCV kütüphanesi ile ön işleme (gürültü giderme, kontrast iyileştirme) adımlarından geçirilerek analiz verimliliği en üst seviyeye taşınmıştır.  

<span class="proje-vurgu">Otonom Kusur Tespiti:</span> Temassız analiz yöntemiyle; eksik parça, hatalı dizilim ve lehim anomalileri otonom olarak saptanarak teşhis süreci dijitalleştirilmiştir.  

-Sistem Performansı: Nesne Algılama ve Hata Saptama Verileri  

<img src="assets/002png.png" width="600" height="300">

<img src="assets/001.png" width="600">  

## CNC-Probe: 3 Eksenli Robot ile Termal ve Elektriksel PCB Analiz Cihazı  
Cihaz, 3 eksenli hareket edebilen robotik bir platform yardımıyla PCB üzerinde detaylı fiziksel kontroller gerçekleştirmeyi amaçlar. İlk aşamada yapay zekânın belirlediği şüpheli noktaları referans alarak kartı termal olarak haritalandırır; bu sayede çıplak gözle görülmeyen kısa devre ve aşırı ısınma bölgelerini anında saptar. Aynı zamanda otonom prob ucuyla otomatik elektriksel ölçümler yaparak, arızanın yerini milimetrik hassasiyetle belirler ve teşhis sürecini kesin bir raporla tamamlar.  

-Projenin İş Akış Diyagramı  

<img src="assets/Otomatik Optik İnceleme.png" width="700" height="400">  

-Sistem Çalışma Prensibi  

<span class="proje-vurgu">1.Eşzamanlı Görsel ve Termal Tarama:</span> Sabit konumlandırılmış yüksek çözünürlüklü optik kamera ve MLX90640 termal kamera, eşzamanlı olarak çalışarak tek seferde tüm PCB'nin genel görüntüsünü ve global ısı haritasını çıkarır.  

<span class="proje-vurgu">2.Yapay Zekâ ile Optik Analiz:</span> Eğitilmiş YOLO modeli, optik görüntü üzerinden kartı tarayarak eksik, hatalı veya şüpheli bileşenlerin piksel koordinatlarını saptar.
Termal Doğrulama ve Veri Çakıştırma: Optik görüntüde saptanan şüpheli pikseller, genel termal harita üzerindeki ilgili bölgelerle eşleştirilir. O bölgedeki sıcaklık verisi analiz edilerek olası kısa devre veya aşırı ısınma durumu yazılımsal olarak doğrulanır.  

<span class="proje-vurgu">3.Mekanik Koordinat Dönüşümü:</span> Optik ya da termal olarak onaylanan hatalı bölgenin piksel koordinatları, kalibrasyon matrisi (Homografi) kullanılarak CNC mekanizmasının gideceği milimetrik X-Y koordinatlarına çevrilir.  

<span class="proje-vurgu">4.Otonom Elektriksel Test:</span> 3 eksenli kol, ucundaki ölçüm probunu doğrudan hesaplanan bu milimetrik koordinata yönlendirir ve bileşen üzerinde fiziksel voltaj/süreklilik ölçümlerini gerçekleştirir.  

<span class="proje-vurgu">5.Veri Füzyonu ve Raporlama:</span> Optik tespit, termal ısı verisi ve elektriksel ölçüm sonuçları merkezi yazılım (PyQt5 GUI) üzerinde birleştirilerek kullanıcıya nihai arıza teşhis raporu sunulur.  

-Ölçüm Platform Karkası  
<img src="assets/CNC KARKASI - 2D(2)_page-0001.jpg" width="600"> 


## Düşük Genlikli Sinyaller için Yüksek SNR’li Amfi  
Bu proje, mikrofonlar veya düşük çıkışlı enstrüman manyetiklerinden gelen zayıf analog ses sinyallerini, devrenin kendi elektriksel ve termal gürültüsüne maruz bırakmadan optimum seviyeye yükselten yüksek performanslı bir ön yükseltici (pre-amplifier) tasarımıdır. Sistemin temel amacı, düşük gürültülü bileşenler ve hassas empedans eşleme teknikleriyle sesin doğal dinamiklerini korumak, maksimum sinyal-gürültü oranı (SNR) elde etmek ve böylece yüksek sadakatli (Hi-Fi) kayıt ile dinleme sistemleri için berrak, kayıpsız ve distorsiyonsuz bir ses altyapısı sunmaktır.

## Dinamik Yük Koşullarında Senkron Jeneratör Karakteristiklerinin MATLAB GUI ile İncelenmesi  
Bu interaktif MATLAB uygulaması, belirli bir senkron jeneratör probleminin değişken güç faktörü koşulları altındaki performans karakteristiklerini görselleştirmek ve analiz etmek amacıyla tasarlanmıştır. Bir kaydırma çubuğu (slider) yardımıyla güç faktörünü dinamik olarak ayarlayabilir; elektriksel parametrelerin (giriş torku, endüklenen tork, fazör diyagramı, verim, terminal gerilimi ve gerilim regülasyonu) ve sistem davranışının bu değişime nasıl tepki verdiğini gözlemleyebiliriz.  
![Proje Demosu](assets/abc.gif)

[Çalışmanın youtube video kaydı](https://www.youtube.com/watch?v=nGcnPR7hnCM)



