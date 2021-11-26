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
 
 **_Form:_**
 
 ![133820308-312e2f35-67fb-41a4-bb9c-b1a7d7e0d0c4](https://user-images.githubusercontent.com/77877967/133822653-a4b799f9-85dd-40f3-ae67-358e99d511a4.png)

 **_Kod:_**
 
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
 
  **_Form:_**
 
  ![133833258-47e602f9-28a1-4edf-a155-8125ae577fe4](https://user-images.githubusercontent.com/77877967/133835756-b7d7a716-1332-4174-8f3a-13b745bd2884.png)

  **_Kod:_**
 
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

  **_Form:_**
 
  ![133833258-47e602f9-28a1-4edf-a155-8125ae577fe4](https://user-images.githubusercontent.com/77877967/133835756-b7d7a716-1332-4174-8f3a-13b745bd2884.png)

  **_Kod:_**
 
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

###### UYGULAMA-4

  *Butona basıldığında Text alanına yazı yazan program.*
  
  **_Form:_**
 
  ![a](https://user-images.githubusercontent.com/77877967/134396042-14f2b6c1-a5fc-45ee-843c-c0106150ec34.jpg)

  **_Kod:_**
 
  ```C#
  private void button1_Click(object sender, EventArgs e)
  {
    textBox1.Text = "merhaba kaan";
  }
  ```
  
  Kod parçasına bakılırsa nesnenin bir özelliğine kod ile müdahale edildiği görülür. Nesnelerin özellikleri sadece **Properties** panelinden değiştirilmez.
  
  Programın çalışma zamanında kodla da değiştirilebilir. Örnek kodlar aşağıda verilmiştir.
  
  ```C#
   textBox1.ForeColor = Color.Green; // Yazı rengini yeşil yapar.
   
   textBox1.Enabled = false; // Nesneyi pasifleştirir. Artık metin girişi yapılmaz.
   
   textBox1.Visible = false; // Nesneyi görünmez hale getirir.
   
   textBox1.Font = new Font("Broadway",16); // Yazı tipini ve boyutunu değiştirir.
  ```

###### UYGULAMA-5

  *Sepete Ekle butonuna tıklandığında TextBox nesnesindeki değeri ListBox nesnesine aktaran Görsel
1.23’teki gibi bir tasarıma sahip programı yazınız.*
  
  **_Form:_**
 
  ![Ekran Alıntısı](https://user-images.githubusercontent.com/77877967/134575804-7b520ab5-67b6-459f-804b-418d37510be8.PNG)

  **_Kod:_**
 
  ```C#
  private void button1_Click(object sender, EventArgs e)
 {
    listBox1.Items.Add(textBox1.Text);
 }
  ```

###### UYGULAMA-6
  
  **_Form:_**
 
  ![Ekran Alıntısı](https://user-images.githubusercontent.com/77877967/134576867-1b343e4c-02f0-49a4-8c66-8bd77f15bcf5.PNG)

  **_Kod:_**
 
  ```C#
  private void button1_Click(object sender, EventArgs e)
  {
    this.BackColor = Color.Red; 
  }
  private void button2_Click(object sender, EventArgs e)
  {
    this.BackColor = Color.Green; 
  }
  private void button3_Click(object sender, EventArgs e)
  {
    this.BackColor = Color.Blue; 
  }
  private void button4_Click(object sender, EventArgs e)
  {
    this.BackColor = Color.Gray; 
  }
  ```

###### UYGULAMA-7
  
  *Adım-1: Form üzerine Görsel 1.25’te görüldüğü gibi dört tane PictureBox nesnesini üst üste olacak şekilde yerleştiriniz.*
  
  *Adım-2: PictureBox nesnelerinin “Visible” özelliğini “false” yapınız (Visible özelliği ile nesnenin görünürlüğü belirlenir.).*
  
  *Adım-3: Dört tane RadioButton nesnesi ekleyiniz ve bunları numaralandırınız.*
  
  **_Form:_**
 
  ![Ekran Alıntısı](https://user-images.githubusercontent.com/77877967/134577370-d2fae962-3f02-4733-8f54-12de9a6217b0.PNG)

  **_Kod:_**
 
  ```C#
  private void radioButton1_CheckedChanged(object sender, EventArgs e)
  {
    pictureBox1.Visible = radioButton1.Checked; 
  }
  private void radioButton2_CheckedChanged(object sender, EventArgs e)
  {
    pictureBox2.Visible = radioButton2.Checked; 
  }
  private void radioButton3_CheckedChanged(object sender, EventArgs e)
  {
    pictureBox3.Visible = radioButton3.Checked; 
  }
  private void radioButton4_CheckedChanged(object sender, EventArgs e)
  {
    pictureBox4.Visible = radioButton4.Checked; 
  }
  ```
  
# İsim Uzayları (Namespace)

  Program yazımı esnasında kullanılan metot, sınıf, değişken, sabit gibi yapıları mantıksal
olarak kategorize etme sistemidir. İsim uzayları, proje büyüdükçe kod yapısının karmaşıklığını engeller.

  .NET Framework ile gelen standart isim uzayları kullanılabileceği gibi proje yazımı esnasında sonradan
oluşturulan isim uzayları da kullanılabilir.

  İsim uzayını projeye dâhil etmek için using kodu kullanılır. Varsayılan olarak using System; kod parçacığı projelerde bulunur. Bu kod parçacığındaki using ifadesi “kullanılıyor” anlamına gelir, System ifadesi ise kullanılan isim uzayını temsil eder.
  
  Programda kişisel bir isim uzayı tanımlanarak kodların organize olması sağlanabilir. Veri tabanına kayıt yapma işlemlerini içeren bir sınıf örneği;
  
  ```C#
  namespace VeriTabani {  // Kaydet sınıfını kullanabilmek için programa using ifadesi ile isim uzayı eklenmelidir.
  public class Kaydet
   {
     //kodlarınız
   }
  }
  ```
  
# Değişkenler ve Temel Veri Türleri

  Değişkenler, programlamanın en temel kavramıdır. Program çalışması sırasında çeşitli türlerde verileri hafızada saklayan değişkenler, ihtiyaca göre tekrar tekrar kullanılan veri tutuculardır.

  Program çalıştığı sürece değişkenler RAM bellekte bulunur, program durdurulduğunda RAM bellekten silinir.
  
  Değişkenlerin içine aktarılacak verilerin türleri çeşitlilik gösterebilir. Her veri türünün RAM bellekte kapladığı alan ve değişkenin türüne göre verinin değer aralığı farklıdır.
  
  Değişkenler, RAM bellekte yer kaplar ve programda kullanılan değişken sayısı arttıkça bu durum RAM belleğin kullanılabilir hafıza kapasitesini düşürür
  
### Tam Sayı Veri Türleri
  
  ![Ekran Alıntısı](https://user-images.githubusercontent.com/77877967/135674605-3056026d-f981-468f-b134-193d2f2f879c.PNG)

### Ondalık Sayı Veri Türleri 

 ![image](https://user-images.githubusercontent.com/77877967/135674811-d41e2cf7-725e-4da6-a42f-de3d369aec00.png)

### Metinsel Veri Türleri

  ![image](https://user-images.githubusercontent.com/77877967/135674879-703202f1-9a78-41ef-8994-4a6b99b4a8c0.png)

### Mantıksal Veri Türleri

  ![image](https://user-images.githubusercontent.com/77877967/135675125-e7238bcd-fa86-453b-880d-3df6679cd99d.png)

  **Veri türlerinin doğru kullanılması programın verimliliğini arttırır.**
  
  *Not: Aynı veri türündeki değişkenler, aynı kod satırında ve _aralarına virgül_ konularak tanımlanabilir.*

**_Örnek:_**
  
  ```C#
  int sayi,deger,sonuç;
  string isim1,isim2,soyad;
  ```
  
# Değişkene Değer Atama

  **(Değişkenin Adı) = (Değişkenin Değeri);**
  
  ![image](https://user-images.githubusercontent.com/77877967/135675892-6d65fe82-74d4-45c0-8274-f100014fe077.png)

  *Not: Değişken tanımlanırken de değer atama yapılabilir.*
  
# Değişken İsimlendirme Kuralları

- **Değişken isimlerinde boşluk kullanılmaz. Boşluk yerine alt çizgi (_) kullanılabilir.**
  
  **_Örnek:_**
   
  **string** ad soyad; şeklinde kullanım yanlıştır.
   
  **string** ad_soyad; veya **string** adsoyad; şeklinde kullanım doğrudur.
  
- **?, !, :, %, +, -, . gibi özel karakterler kullanılmaz.**

  **_Örnek:_**
 
  **string** soru?; şeklinde kullanım yanlıştır.
  
  **string** soru; şeklinde kullanım doğrudur.
  
- **Değişken isimleri sayı ile başlamaz.**

  **_Örnek:_**
  
  **byte** 1not; şeklinde kullanım yanlıştır.
  
  **byte** not1; şeklinde kullanım doğrudur.
  
- **Değişken isimleri büyük ve küçük harfe duyarlıdır.**

  **_Örnek:_**
  
  **ulong** toplamTutar; şeklinde tanımlanan değişken ile *ulong* toplamtutar; veya **ulong** ToplamTUTAR şeklinde tanımlanan değişken aynı değildir.
  
- **Herhangi bir kodla aynı isimde değişken tanımlanamaz. Değişkenlerde _if_, _else_, _random_ gibi programa ait ifadeler isim olarak kullanılmaz.**

- **Zorunluluk yoktur fakat Türkçe karakterlerin (ç, ö, ü, ğ, ş vb. ) kullanılması tavsiye edilmez.**

###### Aşağıdaki soruları Doğru/Yanlış olarak değerlendiriniz. Yanlış olan değişkenin sebebini yazınız.

  ![image](https://user-images.githubusercontent.com/77877967/135678677-a7bb1c7f-213a-4562-93e1-a94b864f3b36.png)

# Değişken Veri Türü Dönüştürme (Convert) İşlemleri

  Değişkenlerin veri türlerini bazen değiştirmek gerekebilir. Sayısal bir ifade, bir nesnenin Text özelliğine
aktarılmak istendiğinde program hata verecektir. İçeriği tamamen sayı olsa da metinsel bir ifadeyi
sayısal veri türüne sahip bir değişkene aktarırken program yine hata verecektir. Bu tip durumlarda
değişkenlerin veri türlerini dönüştürmek gerekir.

  *Tür dönüşümünü sağlayacak hazır metotlar şunlardır:*
  
  **ToString()** >>>> Her türden değişkeni string türüne dönüştürür. ToString(), en sık kullanılan dönüştürme metodudur.
  
   > **Convert**.ToByte(metin)     *>>>>>* Byte’a çevirir.
  
   > **Convert**.ToInt16(metin)    *>>>>>* Short’a çevirir.
  
   > **Convert**.ToInt32(metin)    *>>>>>* Int’e çevirir.
  
   > **Convert**.ToInt64(metin)    *>>>>>* Long’a çevirir.
  
   > **Convert**.ToSingle(metin)   *>>>>>* Float’a çevirir.
  
   > **Convert**.ToDouble(metin)   *>>>>>* Double’a çevirir.
  
   > **Convert**.ToDecimal(metin)  *>>>>>* Decimal’a çevirir.
  
   > **Convert**.ToChar(metin)     *>>>>>* Char’a çevirir.
  
   > **Convert**.ToBoolean(metin)  *>>>>>* Bool’a çevirir.

  **__Örnek:__**
  
  ```C#
  int sayi1=100;
  string deger;
  deger=sayi1; //Program bu noktada convert type ‘int’ to ‘string’ şeklinde hata verecektir.
  ```
  
  **__Örnek:__**
  
  ```C#
  int sayi1=100;
  string deger;
  deger=sayi1.ToString(); //Program artık hata vermeyecektir çünkü veri türleri uyumludur.
  ```
###### UYGULAMA-8

  *Şekildeki gibi girilen iki sayıyı hesaplayan programı yazınız*
  
  **_Form:_**
  
  ![image](https://user-images.githubusercontent.com/77877967/136709142-22d32e7a-2039-4107-8e0f-b6bc2459b31e.png)

  **_Kod:_**
  
  ```C#
  private void button1_Click(object sender, EventArgs e) {
    int number, number2, total;
    
    number = Convert.ToInt16(textBox1.Text);
    number2 = Convert.ToInt16(textBox2.Text);
    total = number + number2;
    
    textBox3.Text = total.ToString(); 
  }
  ```

###### UYGULAMA-9

  *Not:  Programlama dillerinde toplama operatörü sadece sayıları toplamak için kullanılmaz. Metinsel veri türüne sahip değişkenlerin arasına **artı (+)** operatörü konularak string değerlerini birleştirmek için de toplama operatörü kullanılır.*
  
  *Form üzerine iki button, iki textBox koyarak aşağıdaki örnek kodları deneyiniz.*
  
  **_Kod-1:_**
  
  ```C#
  string ad, soyad,topla;
  ad = "Kaan";
  soyad = "Tek";
  topla = ad +" "+ soyad;
  MessageBox.Show(topla);
  ```
  
  **_Kod-2:_**
  
  ```C#
  textBox1.Text="30";
  textBox2.Text="50";
  textBox3.Text= textBox1.Text + textBox2.Text;
  ```
  
###### UYGULAMA-10
  
  *Şekildeki gibi tasarlanan forma girilen sayının karesini alıp mesaj verdiren programı yapınız.*
  
  **__Form:__**
  
  ![image](https://user-images.githubusercontent.com/77877967/136709474-dcc17735-4dce-4d46-a537-15a8025a1215.png)

  **__Kod:__**
  
  ```C#
  private void button1_Click(object sender, EventArgs e)
  {
    int number = Conver.ToInt32(textBox1.Text);
    int kare = number * number;
    
    MessageBox.Show(number.ToString() + " Sayısının karesi = " + kare.ToString());
  }
  ```
  
# İşlem Önceliği

  Matematiksel bir ifade yazılan kod satırında birden fazla aritmetiksel operatör kullanılabilir.
  
  Kodlar çalıştırılırken öncelikle varsa parantez içindeki işlemler, daha sonra parantez dışındaki işlemler
yapılır. Çarpma, bölme ve mod alma işlemleri kendi aralarında, toplama ve çıkarma işlemleri de kendi
aralarında aynı önceliğe sahiptir. Kendi aralarında aynı önceliğe sahip operatörlerin olduğu ifadelerde
ise sırasıyla soldan sağa doğru işlem yapılır.

  **__Örnek-1:__**
  
  *4*3+15/3-1 işlemini yapınız.*
  
  **__Çözüm:__**
  
  ```C#
  =12+5-1 -->Önce çarpma sonra bölme işlemi yapılır.
  =17-1 -->Toplama işlemi ve sonrasında
  çıkarma işlemi yapılır.
  =16
  ```
  
  **__Örnek-2:__**
  
  *(3+4-2)*(10/5*2)-4 işlemini yapınız.*
  
  **__Çözüm:__**
  
  ```C#
  =5*4-4 -->Önce parantez içindeki işlemler yapılır.
  =20-4 -->Çarpma işlemi toplama işleminden öncelikli
  olarak yapılır.
  =16
  ```
  
####### Sıra Sizde
  
  **Soru**           **Cevap**
  
  ```C#
  • 7*5-3            ..........
  
  • 20+30-4*10       ..........
  
  • 9/3+2*2-5+1      ..........
  
  • (5*4)-(3+9)      ..........
  
  • (5*8/4)+3-5*2    ..........
  ```
























