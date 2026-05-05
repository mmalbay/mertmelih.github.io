---
layout: default
title: Projelerim - Mert Melih Albay
---

<p>
  <a href="index.html">Ana Sayfa</a> | 
  <strong><a href="projects.html">Projelerim</a></strong> | 
  <a href="en/projects.html">EN</a>
</p>

<hr>

<h2 style="color: #2e81b7;">Derin Öğrenme Tabanlı Optik İnceleme ve Görsel Kusur Tespit Modülü</h2>
<p>
  Modül, derin öğrenme mimarileri (YOLO) ve bilgisayarlı görü (OpenCV) tekniklerini kullanarak, PCB üzerindeki elektronik bileşenleri (direnç, diyot, MOSFET, entegre vb.) gerçek zamanlı olarak tanımlamak ve görsel kusurları otonom bir şekilde saptamayı amaçlamaktadır. Bu birim; eksik parça, yanlış dizilim, lehim köprüleri ve korozyon gibi fiziksel anomalileri yüksek çözünürlüklü görüntüler üzerinden analiz ederek, manuel gözle kontrol süreçlerini tamamen dijitalleştirmeyi ve hata tespitindeki insan faktörlü hata payını minimize etmeyi hedefler.
</p>

<p>
  <span class="proje-vurgu">Veri Seti Yönetimi ve Etiketleme:</span> Modelin başarımı için özgün bir veri seti oluşturulmuş; PCB bileşenleri manuel olarak etiketlenerek yüksek doğruluklu bir eğitim havuzu hazırlanmıştır.
</p>

<p>
  <span class="proje-vurgu">Veri Artırımı (Data Augmentation):</span> Modelin farklı ışık koşulları ve perspektif açılarında kararlı çalışması amacıyla; döndürme, parlaklık değişimi ve ölçeklendirme teknikleri uygulanarak modelin genelleme yeteneği (Robustness) optimize edilmiştir.
</p>

<p>
  <span class="proje-vurgu">YOLO ve OpenCV Entegrasyonu:</span> Gerçek zamanlı nesne tespiti için YOLO mimarisi kullanılmış; kamera verileri OpenCV kütüphanesi ile ön işleme adımlarından geçirilerek analiz verimliliği en üst seviyeye taşınmıştır.
</p>

<p>
  <span class="proje-vurgu">Otonom Kusur Tespiti:</span> Temassız analiz yöntemiyle; eksik parça, hatalı dizilim ve lehim anomalileri otonom olarak saptanarak teşhis süreci dijitalleştirilmiştir.
</p>

<h4 style="color: #2e81b7;">- Sistem Performansı: Nesne Algılama ve Hata Saptama Verileri</h4>
<img src="assets/002png.png" width="600" height="300">
<img src="assets/001.png" width="600">

<hr>

<h2 style="color: #2e81b7;">CNC-Probe: 3 Eksenli Robot ile Termal ve Elektriksel PCB Analiz Cihazı</h2>
<p>
  Cihaz, 3 eksenli hareket edebilen robotik bir platform yardımıyla PCB üzerinde detaylı fiziksel kontroller gerçekleştirmeyi amaçlar. İlk aşamada yapay zekânın belirlediği şüpheli noktaları referans alarak kartı termal olarak haritalandırır; bu sayede çıplak gözle görülmeyen kısa devre ve aşırı ısınma bölgelerini anında saptar. Aynı zamanda otonom prob ucuyla otomatik elektriksel ölçümler yaparak, arızanın yerini milimetrik hassasiyetle belirler.
</p>  
<br>

<div style="margin: 30px 0; text-align: center;">
  <img src="assets/Video%20Project%2055.gif" alt="Proje Tanıtım GIF" style="width: 100%; max-width: 700px; border-radius: 5px;">
</div>

<br>

<h4 style="color: #2e81b7;">- Projenin İş Akış Diyagramı</h4>
<img src="assets/Otomatik Optik İnceleme.png" width="700" height="400">

<h4 style="color: #2e81b7;">- Sistem Çalışma Prensibi</h4>
<p>
  <span class="proje-vurgu">1. Eşzamanlı Görsel ve Termal Tarama:</span> Yüksek çözünürlüklü optik kamera ve MLX90640 termal kamera, eşzamanlı çalışarak PCB'nin genel görüntüsünü ve ısı haritasını çıkarır.
</p>
<p>
  <span class="proje-vurgu">2. Yapay Zekâ ile Optik Analiz:</span> Eğitilmiş YOLO modeli, optik görüntü üzerinden kartı tarayarak şüpheli bileşenlerin piksel koordinatlarını saptar.
</p>
<p>
  <span class="proje-vurgu">3. Termal Doğrulama ve Veri Çakıştırma:</span> Saptanan şüpheli pikseller, termal harita üzerindeki bölgelerle eşleştirilir. Sıcaklık verisi analiz edilerek kısa devre veya aşırı ısınma durumu yazılımsal olarak doğrulanır.
</p>
<p>
  <span class="proje-vurgu">4. Mekanik Koordinat Dönüşümü:</span> Onaylanan hatalı bölgenin piksel koordinatları, kalibrasyon matrisi (Homografi) kullanılarak CNC mekanizmasının gideceği milimetrik X-Y koordinatlarına çevrilir.
</p>
<p>
  <span class="proje-vurgu">5. Otonom Elektriksel Test:</span> 3 eksenli kol, ölçüm probunu doğrudan hesaplanan bu koordinata yönlendirir ve fiziksel ölçümleri gerçekleştirir.
</p>

<h4 style="color: #2e81b7;">- Ölçüm Platform Karkası</h4>
<img src="assets/CNC KARKASI - 2D(2)_page-0001.jpg" width="600">  

<p>
  <a href="https://www.youtube.com/watch?v=8iHnph1PgWU" target="_blank">▶️ Projenin YouTube Video Kaydı</a>
</p>



<hr>

<h2 style="color: #2e81b7;">Düşük Genlikli Sinyaller için Yüksek SNR’li Amfi</h2>
<p>
  Bu proje, zayıf analog ses sinyallerini, devrenin kendi gürültüsüne maruz bırakmadan optimum seviyeye yükselten yüksek performanslı bir ön yükseltici tasarımıdır. Temel amaç, düşük gürültülü bileşenlerle sesin doğal dinamiklerini korumak ve maksimum sinyal-gürültü oranı (SNR) elde etmektir.
</p>
<div style="text-align: center; margin: 20px 0;">
  <img src="assets/fotott.jpg" alt="Proje Görseli" style="width: 100%; max-width: 600px; border-radius: 8px;">
</div>
<hr>

<h2 style="color: #2e81b7;">Dinamik Yük Koşullarında Senkron Jeneratör Karakteristiklerinin MATLAB GUI ile İncelenmesi</h2>
<p>
  Bu interaktif MATLAB uygulaması, senkron jeneratör performans karakteristiklerini görselleştirmek amacıyla tasarlanmıştır. Slider yardımıyla güç faktörü ayarlanabilir; giriş torku, verim ve gerilim regülasyonu gibi parametrelerin değişimi anlık olarak gözlemlenebilir.
</p>

<p>
  <img src="assets/abc.gif" alt="Proje Demosu">
</p>
<p>
  <a href="https://www.youtube.com/watch?v=nGcnPR7hnCM" target="_blank">▶️ Çalışmanın YouTube Video Kaydı</a>
</p>

<hr>

<h2 style="color: #2e81b7;">Kapsamlı İç Mekan Elektrik Tesisatı ve Yük Dağıtım Yönetimi</h2>
<p>
  Bu çalışma, modern bir konut yapısının elektrik altyapı gereksinimlerini mühendislik standartlarına uygun olarak ele alır. Mimari analiz, yük tahminleri ve teknik hesaplamaların entegrasyonuna odaklanarak güvenli ve verimli bir enerji dağıtım sistemi kurgulanmıştır.
</p>

<h4 style="color: #2e81b7;">- AutoCAD Ortamında Modellenen 2D Kat Planı</h4>
<img src="assets/IlluminationFinalProject.jpg" width="600">

<h3 style="color: #2e81b7;">Gerçekleştirilen Teknik Çalışmalar</h3>  


Apartman dairesi mimari planı ve genel bina hiyerarşisi (katlar ve daireler dahil) AutoCAD ortamında teknik standartlara uygun olarak projelendirilmiştir. Tesisatın güvenli ve sürdürülebilir çalışması adına her bir hat (linye) için ayrı ayrı yüzde gerilim düşümü (%e) hesaplamaları gerçekleştirilmiştir. Sistemin enerji ihtiyacını, akım kapasitesini ve dengesini analiz etmek amacıyla uluslararası standartlarda bir Yük Tablosu oluşturulmuştur. Her oda için gerekli aydınlık düzeyini sağlamak amacıyla Zijl Metodu kullanılarak detaylı ışık kaynağı hesaplamaları yapılmış ve armatür yerleşimleri bu verilere göre tamamlanmıştır.  


<h4 style="color: #2e81b7;">- Güç Dağılımı ve Yük Tablosu Analizi</h4>
<img src="assets/loadingTabel.png" width="600">
<p>
  Toplam kurulu güç 80.504 W olarak hesaplanmış; ancak sistemin gerçek zamanlı çalışma karakteristiğini yansıtmak amacıyla eşzamanlılık katsayısı (simultaneity factor) uygulanarak talep gücü 36.226,8 W seviyesine normalize edilmiştir.  
Konut içindeki yüksek güç tüketen ekipmanlar için özel linyeler tasarlanmıştır. Örneğin; 1. kat dairelerde yer alan çamaşır makinesi, bulaşık makinesi ve fırın gibi yüklerin yanı sıra bodrum katta yer alan araç şarj istasyonu hatları ayrı ayrı projelendirilmiştir.  
Ana dağıtım panosu için 63 A sigorta seçimi yapılmış; alt linyelerde ise yük tipine göre 10 A, 16 A ve 35 A değerlerinde koruma elemanları ve röleler konumlandırılmıştır.  
Ana besleme hattında %0.31 gibi düşük ve güvenli bir gerilim düşümü değeri elde edilerek sistem verimliliği tescil edilmiştir. 
</p>

<p>
  <a href="https://youtu.be/-xOm79f4XDA" target="_blank">▶️ Detaylı YouTube Video Kaydı</a>
</p>
