# Site Yönetim Veritabanı Sistemi 
## Projenin Tanıtımı 
Bu proje, bir apartman sitesinin yönetimini kolaylaştırmak için bir veritabanı sistemi 
oluşturmayı amaçlar. Veritabanı, apartman kompleksi içindeki dairelerin, otoparkın, site 
güvenliğinin, kulüp/spor salonunun ve site temizlik görevlerinin yönetimini sağlayacaktır. 
Sistem, kullanıcıların bu bileşenlerle ilgili bilgilere erişmesini, güncellemesini ve takip 
etmesini kolaylaştıracak bir arayüz sunacaktır. 
### Daire Yönetimi: 
• Dairelerin numaraları, sahipleri, kiracıları, metrekareleri gibi bilgilerin kaydedilmesi.<br>
• Daire sahiplerinin ve kiracıların iletişim bilgilerinin takibi.<br>
• Dairelerin ödemelerinin takibi (aidat, elektrik, su vs.).<br> 
### Otopark Yönetimi: 
• Otoparktaki park yerlerinin kaydedilmesi ve kimin kullandığının takibi. 
### Site Güvenliği: 
• Güvenlik görevlilerinin bilgilerinin kaydedilmesi ve vardiya takibinin yapılması.<br>
• Giriş/çıkış kayıtlarının tutulması. <br>
### Kulüp/Spor Salonu Yönetimi: 
• Kulüp ve spor salonunun kullanıcılarının kaydedilmesi ve üyelik takibinin 
yapılması.<br>
• Tesis rezervasyonlarının yapılması.<br>
### Site Temizlik Görevleri: 
• Temizlik görevlilerinin bilgilerinin kaydedilmesi ve çalışma programlarının 
oluşturulması.<br>
• Temizlik görevlerinin takibi ve günlük, haftalık, aylık planların oluşturulması.<br>
## Gereksinim Analizi  
## Kullanıcı Gereksinimleri: 
## Daire Sahipleri ve Kiracılar: 
• Kullanıcı olarak sisteme giriş yapabilmeliyim.<br>
• Dairemizin bilgilerini görüntüleyebilmeliyim (numara, metrekare, sahip/kiracı 
bilgisi).<br> 
• Ödemelerimizi takip edebilmeli ve ödeme yapabilmeliyiz.<br>
## Otopark Kullanıcıları: 
• Otopark yerlerinin durumunu görebilmeli ve rezervasyon yapabilmeliyim.<br>
## Site Güvenlik Görevlileri: 
• Günlük vardiya bilgilerimi görebilmeliyim.<br>
• Giriş/çıkış kayıtlarını görebilmeliyim.<br>
## Kulüp/Spor Salonu Kullanıcıları: 
• Tesis rezervasyonu yapabilmeliyim.<br>
• Üyelik bilgilerimi ve ödemelerimi görebilmeliyim.<br> 
## Site Temizlik Görevlileri: 
• Çalışma programlarımı görebilmeli ve güncelleyebilmeliyim.<br>
• Temizlik görevlerini görebilmeli ve tamamlandı olarak işaretleyebilmeliyim.<br>
## Sistem Gereksinimleri: 
## Kullanıcı Yönetimi: 
• Kullanıcıların kaydedilmesi, güncellenmesi ve silinmesi.<br> 
• Kullanıcı yetkilendirme ve oturum yönetimi.<br>
## Daire Yönetimi: 
• Dairelerin kaydedilmesi, güncellenmesi ve silinmesi.<br> 
• Ödemelerin kaydedilmesi ve takibi.<br>
### Otopark Yönetimi: 
• Park yerlerinin kaydedilmesi ve yönetilmesi.<br>
• Rezervasyon sistemi.<br>
### Site Güvenliği: 
• Güvenlik görevlilerinin kaydedilmesi ve vardiya takibi.<br> 
• Giriş/çıkış kayıtlarının tutulması.<br>
### Kulüp/Spor Salonu Yönetimi: 
• Kulüp ve spor salonunun kaydedilmesi ve yönetilmesi.<br> 
• Üyelik bilgilerinin kaydedilmesi ve üyelik yönetimi.<br>
### Site Temizlik Görevleri: 
• Temizlik görevlerinin kaydedilmesi ve programlanması.<br>
• Temizlik görevlerinin takibi ve güncellenmesi.<br>
### Performans Gereksinimleri: 
• Sistemin hızlı ve güvenilir olması.<br>   
• Veritabanı işlemlerinin hızlı ve verimli yapılması.<br>  
• Kullanıcıların anlık güncellemelere kolayca erişebilmesi.<br>
### Güvenlik Gereksinimleri: 
• Kullanıcıların gizli bilgilerinin güvenliği (şifreleme, güvenli oturum yönetimi vb.) <br>
• Veritabanı güvenliği (yetkilendirme, yetki yönetimi, yedekleme vb.)<br> 
## İş Kuralları 
Apartman – Daireler (N:1)<br> 
Bir apartmanda birden fazla daire bulunur.<br>
Bir daire bir apartmanda bulunabilir.<br><br> 
Apartman – Apartman Yöneticisi (1:1)<br>
Bir apartmanı bir yönetici yönetir.<br>
Bir yönetici bir apartmanı yönetebilir.<br><br>
Apartman – Site Temizlik Görevi (N:M)<br>
Bir apartmanda birden fazla temizlik görevi olur.<br>
Bir temizlik görevi birden fazla apartmanda olabilir.<br><br>
Daireler – Otopark Alanı (N:M) <br>
Bir daire birden fazla otopark kullanabilir.<br>
Bir otoparkı birden fazla daire kullanır.<br><br> 
Daire Telefonları – Site Güvenliği Telefon Numaraları (1:N)<br>
Site güvenliğinde tüm telefon numaraları bulunur.<br>
Bir dairede bir telefon bulunur.<br><br>
Daireler – Araba (N:1)<br>
Bir dairede birden fazla arabaya sahip olabilir.<br>
Bir araba bir daireye sahiptir.<br><br>
Daireler – Apartman Sakinleri (N:1)<br>
Bir dairede birden fazla daire sakini oturur.<br>
Bir apartman sakini bir dairede oturur.<br><br>
Apartman Sakinleri – Apartman Yöneticisi (1:1)<br>
Bir apartman sakini yönetici olabilir<br>
Bir yönetici aynı zamanda apartman sakinidir <br><br>
Apartman Sakinleri – Kulüp Üyeleri (N:M)<br> 
Bir apartman sakini birden fazla kulübe üye olabilir.<br>
Bir kulübün birden fazla üyesi olabilir.<br><br>
Apartman Sakinleri – Spor Sahası (N:M)<br>
Bir apartman sakini birden fazla spor sahası kullanabilir.<br>
Bir spor sahasını birden fazla apartman sakini kullanabilir.<br><br>
Site Temizlik Personeli – Site Temizlik Malzemeleri (N:M)  
Bir temizlik personeli birden fazla malzeme kullanabilir.<br>
Bir malzemeyi birden fazla temizlikçi kullanabilir.<br><br> 
Site Temizlik Personeli – Site Temizlik Görevi (N:M)<br> 
Bir personel birden fazla görevi yapabilir.<br>
Bir görevi birden fazla personel yapabilir.<br><br>
Site Temizlik Görevi – Otopark (N:M)<br>
Bir otopark da birden fazla görev bulunabilir.<br>
Bir temizlik görev bir otopark da bulunur.<br><br> 
Site Temizlik Görevi – Spor Salonu (N:M)<br>
Bir spor salanında birden fazla temizlik görevi bulunabilir.<br> 
Bir temizlik görevi birden fazla spor salonunda bulunabilir.<br><br> 
Spor Sahası Personel – Spor Sahası Türü(N:M)<br> 
Bir spor personelinin birden fazla branşı olabilir.<br> 
Bir branşın birden fazla spor personeli bulunabilir.<br><br>
Site Kulüpleri – Kulüp Üyeleri (N:M) <br>
Bir kulübün birden fazla üyesi olabilir<br>
Bir üye birden fazla kulübe üye olabilir.<br><br>
Site Kulüpleri – Kulüp Yöneticisi (N:1)<br>
Bir kulübün bir yöneticisi olur.<br>
Bir yönetici birden fazla kulüp yönetebilir.<br><br>


## Varlık İlişki Modelleri Ve İlişkisel Şemalar 
### Kazayağı modeli
![](/Veri_Tabanina_Erisim/3.png)
### Chen Modeli
![](/Veri_Tabanina_Erisim/3.png)



