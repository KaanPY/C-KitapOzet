# NESNE TABANLI PROGRAMLAMA ÇALIŞMA ORTAMI

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

# VİSUAL STUDIO WINDOWS FORM APP

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
