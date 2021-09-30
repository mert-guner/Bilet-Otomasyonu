# Bilet-Otomasyonu
Bir firmadan otobüs bileti almanızı sağlayan bir otomasyon.
<br>
<br>
<br>
**Proje Nasıl İndirilir?**
<br>
<br>
Yeşil renkli code butonuna tıkladıktan sonra Download ZIP diyerek bilgisayarınıza indirebilirsiniz.
<br>
<br>
<br>
**Projeyi çalıştırabilmek için gerekli olan programlar?**
<br>
<br>
visual studio 2017 ve mssql13 programları kurulmalıdır. 
<br>
<br>
<br>
**Proje nasıl çalıştırılır?**
<br>
<br>
1) ZIP dosyasını indirdikten sonra içerisinde bulunan projenin kaynak dosyaları dışarı çıkarılır.<br>
2) Dışarı çıkarılan klasörü açtıktan sonra veri tabanı dosyasının içerisindeki mdf ve ldf uzantılı dosyaları mssql de DATA dosyasının içerisine atıyoruz. Videoda detaylı anlatılıyor [Youtube linki](https://www.youtube.com/watch?v=EHJHkOIMaaQ)<br>
3) Otobüs otomasyonu dosyasının içerisindeki Otomasyon.sln isimli proje açılır. <br>
4) Form1.cs açılır ve SqlConnection kısmında ki Server bilgisi kısmına bilgisayarınızın server bilgisini yazmalısınız. İlgili kod satırının ekran görüntüsü aşağıdadır.<br>

![sa](https://user-images.githubusercontent.com/91637929/135537408-24e963f7-37a5-4351-a789-d39c8e1b7f47.PNG)
<br><br><br><br><br><br><br>


## Projenin Anlatımı
<br><br>


![image1](https://user-images.githubusercontent.com/91637929/135361132-646e2ea9-1af8-41d0-874e-757b5cead3d5.png)
<br>
Giriş Formu, programı kullanacak yöneticinin giriş yaptığı bölümdür. 
<br>
<br>

Bu program için gerekli giriş bilgileri :<br>
**Kullanıcı Adı :** yonetici<br>
**Parola :** parola 
<br>
<br>

![image2](https://user-images.githubusercontent.com/91637929/135361692-86d66476-a56c-4081-b351-a46b3391e6ce.png)
<br>
<br>
Yönetici paneli formu, programa doğru şekilde giriş yapıldığında açılacak olan formdur. Bu formda yöneticinin yapabileceği tüm işlemler için erişebileceği formları açan butonlar bulunmaktadır. 
<br>
<br>

![image3](https://user-images.githubusercontent.com/91637929/135361766-50c190bd-b39a-485e-bce6-1d6ed1591f84.png)
<br>
<br>
Otobüs işlemleri formu, veri tabanında kayıtlı otobüslerle ilgili bilgilerin görüntülendiği ve otobüs işlemlerinin yapıldığı formdur.
<br>
**Bu formda yapılabilecek otobüs işlemleri ;**<br>
•	Otobüs Ekleme<br>
•	Otobüsü Silme<br>
•	Var Olan Otobüslerin Bilgilerinin Güncellenmesi
şeklindedir.
<br>
<br>
Data Grid View üzerinde RowHeaderMouseClick özelliği sayesinde tıklanan otobüs hakkında bilgiler aşağıdaki textbox’lara dolmaktadır. “Temizle” butonu sayesinde tüm textbox’lardaki bilgiler temizlenebilmektedir. Ayrıca veri tabanında “OtobusID”nin “Identity Specification” değeri “Yes” olarak ayarlanıp otomatik değer alması sağlandığı için Otobus ID label’ı karşısında yer alan textbox’ın ReadOnly özelliği “true” olarak ayarlanmış, kullanıcının otobüs ekleme veya güncelleme esnasında OtobusID değerine veri göndermesi engellenmiştir. 
<br>
<br>


![image4](https://user-images.githubusercontent.com/91637929/135361788-9989237b-c32e-4bb0-b487-8de7baa03b6f.png)
<br>
**Kayıt Ekliyoruz**
<br>
<br>
<br>
<br>
![image5](https://user-images.githubusercontent.com/91637929/135361808-e778a2a9-3f35-4b9e-aa0d-822463f5cd8e.png)
<br>
Girdiğimiz kayıtlar veri tabanına aktarılmış.
<br>
<br>
<br>
<br>
![image6](https://user-images.githubusercontent.com/91637929/135361835-7dffd672-1c4e-4f79-b070-72002decb124.png)
<br>
**Girdiğimiz kaydı siliyoruz**
<br>
<br>
<br>
<br>
![image7](https://user-images.githubusercontent.com/91637929/135361856-3f4e6088-bdb5-4551-92ec-f2cc0360ba1d.png)
<br>
**Kayıt veri tabanından silinmiş**
<br>
<br>
<br>
<br>
![image8](https://user-images.githubusercontent.com/91637929/135361868-745970a1-01ef-4591-9d10-c38c7e844fc8.png)
<br>
**ID’si 4 olan kaydın koltuk adedini 37 olarak güncelliyoruz.**
<br>
<br>
<br>
<br>
![image9](https://user-images.githubusercontent.com/91637929/135361883-e9f1079a-34e9-4544-9acd-1505034121e0.png)
<br>
**Kayıt güncellenmiş.**
<br>
<br>
<br>
<br>
![image10](https://user-images.githubusercontent.com/91637929/135361897-bace362f-4f45-4b7b-a690-206d18fdedad.png)
<br>
<br>
Sefer işlemleri formu veri tabanında kayıtlı seferlerle ilgili bilgilerin görüntülendiği ve sefer işlemlerinin yapıldığı formdur.
<br>
**Bu formda yapılabilecek sefer işlemleri ;**<br>
•	Sefer Ekleme<br>
•	Sefer Silme<br>
•	Var Olan Seferlerin Bilgilerinin Güncellenmesi
şeklindedir
<br>
<br>
Data Grid View üzerinde RowHeaderMouseClick özelliği sayesinde tıklanan sefer hakkında bilgiler aşağıdaki textbox’lara dolmaktadır. “Temizle” butonu sayesinde tüm textbox’lardaki bilgiler temizlenebilmektedir. “SeferNo”, veri tabanında otomatik değer alacak şekilde ayarlanmadığı için Sefer No label’ı karşısında yer alan textbox’a veri girişi engellenmemiştir.<br>

Sefer Tarihi, DateTimePicker ile alınıp veri tabanında da “date” olarak tutulmaktadır. <br>

Otobüs Seçimi için kullanılan combobox’a veri tabanından “Otobusler” tablosundaki “OtobusAdi” sütunu çekilmektedir.
<br>
<br>
![image11](https://user-images.githubusercontent.com/91637929/135361907-617ae810-a53e-4942-8371-ac7bf7769974.png)
<br>
<br>
Bilet rezervasyon formu, veri tabanındaki kayıtlı seferlerin görüntülendiği ve bu seferlere müşteri eklenen formdur.
<br>
**Bu formda yapılabilecek işlemler ;**<br>
•	Seferlere Müşteri Ekleme
<br>
<br>

Aynı şekilde Data Grid View üzerinde RowHeaderMouseClick özelliği sayesinde tıklanan sefer hakkında bilgiler aşağıdaki “Sefer” groupbox’ında yer alan “Koltuk No” hariç tüm textbox’lara dolmaktadır. “Koltuk No” değeri elle girilmektedir. Veri tabanında “MusteriNo”nun “Identity Specification” değeri “Yes” olarak ayarlanıp otomatik değer alması sağlandığı için “Müşteri” groupbox’ındaki “No” label’ı karşısında yer alan textbox’ın ReadOnly özelliği “true” olarak ayarlanmış, rezervasyon esnasında “MusteriNo” sütununa veri gönderilmesi engellenmiştir.<br>

“Rezervasyon Yap” butonuna tıklandığında bilgilerde hata yoksa “Sefer_Musteri” tablosuna bilgiler aktarılmaktadır.
<br>
<br>

![image12](https://user-images.githubusercontent.com/91637929/135361916-6a68af51-3a15-4eb1-9239-6f1c7db2ebad.png)
<br>
<br>
Satılan Biletler formu, veri tabanındaki kayıtlı biletlerin görüntülendiği ve bu biletlerin güncellenip silinebildiği formdur.
<br>

**Bu formda yapılabilecek işlemler ;**<br>
•	Biletlerin Güncellenmesi<br>
•	Biletlerin Silinmesi


