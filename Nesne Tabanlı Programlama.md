# [NESNE TABANLI PROGRAMLAMA ÇALIŞMA ORTAMI](http://meslek.eba.gov.tr/indir.php?d=U2NyRllCYWpabXp0aGJGZ0J4V1ZHSGFnbmhtK0h0QWhsclh1c1czN29vSGFGMlAzNVRuUXl4Z2kvNlZpRDIyYw==&da=NEROb3VtcjUyNGpFNFAzRW5DK243NmhqLzdVUHF4b0lwMGlubEZCaW5mbz0=&iq=bDQxb29HUUdtS3RmSWRwSXlnZkVTVHh3bWxYeXhCNjhMUnJhOCtlKzVQZHM1eEJHeGMyQ2RlNmhJYTdwMjN1QVZ1TnpQeHV5OFcrS016QUtDa3JLakE9PQ==)

- **Program Nedir?**
 
  Program, herhangi bir elektronik cihaza bir işlem yaptırmak için yazılan komutlar dizisidir.
  Programlar; bilgisiyar, cep telefonu, tablet, elektronik ev aletleri, araba ve daha bir çok yerde kullanılır.
  
  Bilgisiyar ve diğer elektronik cihazlar çalışma prensibi olarak programları kullanıp önce girilen bilgiyi alır, ardından bu bilgiyi işler ve en sonunda ortaya bir sonuç çıkarır.
  Bu sonuç bazen bir mesaj bazen de bir işlemi gerçekleştirme şeklindendir.
  
- **Programlama Nedir?**

  Programlama; bilgisiyar programlarının yazılması, test edilmesi ve bakımının yapılması sürecine verilen isimdir.
  
- **C# Programlama Dili**

  Nesne tabanlı olarak geliştirilmiş bir dildir.
 
- **Neler Yapılır?**
 
  - *Mobil uygulamalar.*
  - *Konsol uygulamaları.*
  - *Web servisleri.*
  - *Dinamik kütüphaneler(DLL).*
  - *Oyun tasarımı.*
  - *Form uygulamaları.*

- **C#  Programlama Dilinin Tercih Edilmesinin Sebepleri?**

  - *Yazılması ve anlaşılması kolay kod yapısına sahip sahiptir.*
  - *Kullanışlıdır.*
  - *Ekip çalışmasına elverişlidir.*
  - *Kullanıcıyla etkilişimlidir.*
  - *Grafik arayüzlü tasarımlar yapılabilir.*
  - *Ağ üzerinden birbiriyle uyumlu çalışabilir.*
  - Çevrimiçi veya çevrimdışı kullanılabilir.*
  - *QR kod okuyucu, kamera, yazıcı vb. cihazlarla etkileşimlidir.*
  - *Verileri depolayıp işleyerek analiz yapabilir.*
  - *Sosyal medya platformları ile etkileşimlidir.*
  - *Cep telefonu uygulamaları ile etkileşimlidir.*
  - *Yapay zeka teknolojisi kullnarak yüz tanıma, nesne tanıma, ses tanıma işlemleri yapılabilir.*
  - *Birçok özelliğe sahip farklı programları geliştirebilme imkanı sağlar.*

- **.NET Framework(Geliştirme Çatısı) Nedir?**

  Programlama dillerinden bağımsız ve farklı programlama dilleri ile ortak çalışma imkanı sağlayan bir uygulama geliştirme platformudur.
  
  Bu platform ile farklı dilleri bilen programcılar ortak bir projeyi yürütebilir.
  
  Ayrıca .NET Framework altyapısında kullanıma sunulmuş hazır kod kütüphaneleri ile kod yazma çok daha hızlı ve verimli olmaktadır.
  
- **C# Ve .NET Framework İlişkisi**

  C# bir programlama dilidir. .NET Framework ise C# dili ve birçok dilin kütüphanelerinin yüklü olduğu bir uygulama geliştirme platformudur. C# dilinde kullanılan kütüphanelerin
  tümü .NET Framework kütüphaneleridir.
  
- **.NET Framework Çalışma Mantığı Nedir?**

  Programlama dilleri ile yazılan kodlar makine için anlamlı değildir, kodların makine dilinde yazılması veya makine diline çevrilmesi gerekir. Program yazarken kullanılan 
  kodlar derlendiğinde doğrudan makine diline çevrilmez.
  
  Kodlar önce **ara dil**(Intermediate Language) koduna, ardından da **çalışma dil derleyicisine**(Just-In-Time Compiler) tarafından makine diline çevrilir. Böylelikle kodlar
sorunsuz bir şekilde çalışır. Bu işlemlerin yapılmasını .NET Framework altyapısı sağlar.
  
  ![Ekran Alıntısı](https://user-images.githubusercontent.com/77877967/133806086-7b888082-b451-4e7d-9b75-34cdf51d4d1f.PNG)

# VISUAL STUDIO WINDOWS FORM APP

- **Sık Kullandığımız Paneller**

  > **Toolbox**: Kullanılacak nesnelerin olduğu yer.
   
  > **Solution Explorer**: Proje dosyalarının olduğu yer.
   
  > **Properties**: Seçilen nesnenin özelliklerinin olduğu yer.

  *Not: Ana ekranda istenilen paneller yoksa **__view__** menüsünden seçilir.*

###### UYGULAMA-1

 *Form'a eklenen, TextBox ve Button nesnelerinden; textBox içerisine yazılan yazının button'a basıldığında label'a yazan programı yazınız.*
 
 1. **Form:**
 
 ![133820308-312e2f35-67fb-41a4-bb9c-b1a7d7e0d0c4](https://user-images.githubusercontent.com/77877967/133822653-a4b799f9-85dd-40f3-ae67-358e99d511a4.png)

 2. **Kod:**
 
 ```C#
 private void button1_Click(object sender, EventArgs e)
 {
   label1.Text = textBox1.Text;
 }
 ```
- **Form Ekranı**

  Form ekranı, programın görsel tasarımının yapıldığı yerdir.
  
- **Araç Kutusu(ToolBox)**

  Form üzerinde tasarım için kullanılabilecek nesnelerin olduğu yer. En çok tercih edilen ToolBox nesneleri.
  
  > **Button**: Programda bazı kodları çalıştırmak için kullanılan komut düğmeleridir. Button nesnesine tıklandığında içeri doğru basma efekti gerçekleştiği için tıklama(click) olayları için vazgeçilmez nesnedir.

  > **Label**: Form üzerinde bilgi vermek için kullanılan nesnedir.

  > **TextBox**: İçinde tek satır metin girişi yapılabilen nesnedir. Bilgi girişi için en çok tercih edilen nesnedir.

  > **CheckBox**: Kullanıcıya bir veya aynı anda birden çok seçeneği işaretleme imkanı sağlayan nesnedir.

  > **ComboBox**: Açılır liste ile açılan seçenekler arasında seçim yapılmasını olanak sağlayan araçtır. Listeye yeni eleman ekleme ve çıkarma işlemleri, tasarım ekranında veya program çalışırken kod ile yapılabilir.

  > **DateTimePicker**: Tarih ve saat seçme işlemlerine olanak sağlayan nesnedir.

  > **GroupBox**: Form elemanlarını kendi aralarında gruplamak için kullanılan nesnedir. Nesneler gruplar halinde olduğu için daha anlaşılır tasarımlar yapılabilir.

  > **ListBox**: Sunulacak seçeneklerin açık bir liste halinde gösterildiği nesnedir.

  > **MenuStrip**: Programda menü başlıkları ve alt başlıklar oluşturmak için kullanılan nesnedir.

  > **PictureBox**: Form üzerinde resim göstermek için kullanılan nesnedir.

  > **ProgressBar**: Yapılan bir işlemin ne kadarının tamamlandığını göstermek için kullanılan nesnedir.

  > **RadioButton**: CheckBox nesnesinden farklı olarak birçok seçenek içinde sadece birinin seçilmesine imkan sağlayan nesnedir.

  > **RichTextBox**: Birden çok satır içine metin girişi yapılabilen nesnedir.

  > **TabControl**: Form elemanlarının gruplara ayrıldığı, grupların içindeki elemanları görmek için sekmelerin kullandığı nesnedir. Her sekme, bir grubu temsil eder.

  > **Timer**: Kodların zamanlanarak çalışmasını sağlayan nesnedir.

# ÖZELLİKLER(PROPERTİES) PANELİ

  Form nesnenin ve diğer tüm nesnelerin özelliklerinin listelendiği, değiştirildiği ve ayrıca nesnelere ait olayların(events) listelendiği paneldir.
  
  Her nesnenin kendine ait benzersiz özellikleri olduğu gibi diğer nesneler ile ortak özellikleri de  bulunmaktadır.
  
  Tüm nesnelerin en temel ortak özelliği, isim(name) özelliğidir.
  
  Örneğin button1 nesnesine ait sık kullanılan bazı özellikler(diğer nesnelerde de genelde ortak özellikler) ve anlamları aşağıda verilmiştir.
  
  > **BackColor**: Nesnenin arka plan rengini değiştirir.

  > **BackgroundImage**: Nesnenin arka planına resim ekler.

  > **Font**: Nesnenin yazı tipini, boyutunu ve kalınlığını değiştirir.

  > **ForeColor**: Nesnenin yazı rengini değiştirir.

  > **Text**: Nesnenin yazı metinini değiştirir.

  > **TextAlign**: Nesnenin yazısınız hizalar.

# OLAYLAR(EVENTS) PANELİ

  Her nesnenin form üzerinde bir görevi bulunmaktadır. Bazı nesneler sadece programın işlevi ile ilgili bilgiye ve görseli yansıtmak için kullanılır. Bazı nesneler ise belli
  durumlarda(üzerine tıklandığında, bir tuşa basıldığında vs.) kod parçacıklarını çalıştırmak için kullanılır. Nesneler, kullanıcı ile etkileşimli olaylar sayesinde
  sağlamaktadır.
  
  Örneğin; butona tıklandığında şifre kontrolünün yapılması, klavyeden sağ ok tuşuna basıldığında bir sonraki resmin gösterilmesi, PictureBox nesnesinin üzerine çift tıklama yapıldığında resme ait ilgili bilgilerin MessageBox ile göstermesi vb.
  
  Örneğin button1 nesnesine ait sık kullanılan bazı olaylar(diğer nesnelerde de genelde ortak olaylar) ve anlamları aşağıda verilmiştir.
  
  > **Click**: Nesneye fare ile tıklanması veya fare nesne üzerindeyken enter tuşuna basılmasıyla devreye giren olaydır.

  > **MouseClick**: Click gibi nesnenin fare ile tıklanması olaydır. Fakat MouseClick, fareye ait koordinatlar gibi özel bilgileri de verir.

  > **KeyDown**: Klavyeden bir tuşa basılması olaydır.

  > **KeyUp**: Klavyede basılan tuşun bırakılması olaydır.

  > **MouseDown**: Farenin tuşuna basılması olaydır.
  
###### UYGULAMA-2

 *Form'a eklenen, Button nesnesinden; button'a basıldığında pop-up gösteren programı yazınız.*
 
 1. **Form:**
 
 ![133833258-47e602f9-28a1-4edf-a155-8125ae577fe4](https://user-images.githubusercontent.com/77877967/133835756-b7d7a716-1332-4174-8f3a-13b745bd2884.png)

 2. **Kod:**
 
 ```C#
 private void button1_Click(object sender, EventArgs e)
 {
   MessageBox.Show("Merhaba Dünya", "Başlık", MessageBoxButtons.YesNoCancel);
 }
 ```
# ÇÖZÜM PENCERESİ(SOLUTİON EXPLORER) PANELİ

  Proje ile ilgili tüm dosya ve klasörlerin listelenerek silme, kopylama, taşıma, isim değiştirme işlemlerinin yapıldığı paneldir.
  
  Projenin detaylı bir haritsaı gibi düşünülebilir. Çözüm penceresi ile projeye yeni sınıf(class), form ve başka öğeler eklenebilir. Veri tabanı dosyası, resim, müzik, video dosyaları projeye dahil edilebilir.
  
  Projeye eklenen her form, çözüm penceresinde ayrı ayrı listelenmektedir. Formlar kod ve tasarım olarak farklı dosyalarda oluşur.
  
  Kod veya tasarım ekranını göstermenin yolları şunlardır;
  
  1. Form ekranı üzerinde herhangi bir noktada fare sağ tuşu kullanarak açılan listede **view code**(kodu göster) tıklanarak kod ekranı, **view designer**(tasarım göster) tıklanarak tasarım ekranı görüntülenir.
  2. Klavyeden **F7** tuşuna basıldığında kod ekranı açılır. klavyede **shift+F7** tuşuna basıldığında tasarım ekranı açılır.

# HATA LİSTESİ(ERROR LİST) PANELİ

  Kod yazarken, kod derlenirken veya kod çalışırken oluşan hataların ve uyarıların listelendiği paneldir.
  
  a) **Erros(Hatalar) Bölümü**: Çok kritik ve programın çalışmasını engelleyen hatalardır. Örneğin; değişkeni tanımlamadan bir kod bloku içinde kullanmak, kod satırının sonunda noktalı virgül koymamak vb.
  
  b) **Warnings(Uyarılar) Bölümü**: Programın çalışmasını engellemeyecek düzeydeki iletilerdir. Örneğin; değişkenin tanımlanıp hiçbir zaman kullanılmaması vb.
  
###### UYGULAMA-3

 1. **Form:**
 
 ![133833258-47e602f9-28a1-4edf-a155-8125ae577fe4](https://user-images.githubusercontent.com/77877967/133835756-b7d7a716-1332-4174-8f3a-13b745bd2884.png)

 2. **Kod:**
 
 ```C#
 private void button1_Click(object sender, EventArgs e)
 {
   MessageBox.Show("Merhaba Dünya");
 }
 ```

- **MessageBox Komutu**

  MessageBox adından da anlaşılacağı gibi ekrana mesaj verdiren sınıfın adıdır. En temel kullanımı, örnek kodda verildiği gibi sadece tek bir mesaj gösterme şeklindedir.
  
  MessageBox sınıfının bazı kullanım şekilleri aşağıda verilmiştir.
  
  **Kod-1:**
  ```C#
  private void button1_Click(object sender, EventArgs e)
  {
    MessageBox.Show("Mesaj Metni", "Mesaj Başlığı");
  }
  ```
  
  **Kod-2:**
  ```C#
  private void button1_Click(object sender, EventArgs e)
  {
    MessageBox.Show("Mesaj Metni", "Mesaj Başlığı", MessageBoxButtons.YesNoCancel);
  }
  ```
  
  **Kod-3:**
  ```C#
  private void button1_Click(object sender, EventArgs e)
  {
    MessageBox.Show("Mesaj Metni", "Mesaj Başlığı", MessageBoxButtons.OkCancel);
  }
  ```
