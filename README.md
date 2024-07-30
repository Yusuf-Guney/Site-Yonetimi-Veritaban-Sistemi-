## Site Yönetim Veritabanı Sistemi 
# PROJENİN TANITIMI 
Bu proje, bir apartman sitesinin yönetimini kolaylaştırmak için bir veritabanı sistemi 
oluşturmayı amaçlar. Veritabanı, apartman kompleksi içindeki dairelerin, otoparkın, site 
güvenliğinin, kulüp/spor salonunun ve site temizlik görevlerinin yönetimini sağlayacaktır. 
Sistem, kullanıcıların bu bileşenlerle ilgili bilgilere erişmesini, güncellemesini ve takip 
etmesini kolaylaştıracak bir arayüz sunacaktır. 
Daire Yönetimi: 
• Dairelerin numaraları, sahipleri, kiracıları, metrekareleri gibi bilgilerin kaydedilmesi. 
• Daire sahiplerinin ve kiracıların iletişim bilgilerinin takibi. 
• Dairelerin ödemelerinin takibi (aidat, elektrik, su vs.). 
Otopark Yönetimi: 
• Otoparktaki park yerlerinin kaydedilmesi ve kimin kullandığının takibi. 
Site Güvenliği: 
• Güvenlik görevlilerinin bilgilerinin kaydedilmesi ve vardiya takibinin yapılması. 
• Giriş/çıkış kayıtlarının tutulması. 
Kulüp/Spor Salonu Yönetimi: 
• Kulüp ve spor salonunun kullanıcılarının kaydedilmesi ve üyelik takibinin 
yapılması. 
• Tesis rezervasyonlarının yapılması. 
Site Temizlik Görevleri: 
• Temizlik görevlilerinin bilgilerinin kaydedilmesi ve çalışma programlarının 
oluşturulması. 
• Temizlik görevlerinin takibi ve günlük, haftalık, aylık planların oluşturulması. 
Gereksinim Analizi  
Kullanıcı Gereksinimleri: 
Daire Sahipleri ve Kiracılar: 
• Kullanıcı olarak sisteme giriş yapabilmeliyim. 
• Dairemizin bilgilerini görüntüleyebilmeliyim (numara, metrekare, sahip/kiracı 
bilgisi). 
• Ödemelerimizi takip edebilmeli ve ödeme yapabilmeliyiz. 
Otopark Kullanıcıları: 
• Otopark yerlerinin durumunu görebilmeli ve rezervasyon yapabilmeliyim. 
Site Güvenlik Görevlileri: 
• Günlük vardiya bilgilerimi görebilmeliyim. 
• Giriş/çıkış kayıtlarını görebilmeliyim. 
Kulüp/Spor Salonu Kullanıcıları: 
• Tesis rezervasyonu yapabilmeliyim. 
• Üyelik bilgilerimi ve ödemelerimi görebilmeliyim. 
Site Temizlik Görevlileri: 
• Çalışma programlarımı görebilmeli ve güncelleyebilmeliyim. 
• Temizlik görevlerini görebilmeli ve tamamlandı olarak işaretleyebilmeliyim. 
Sistem Gereksinimleri: 
Kullanıcı Yönetimi: 
• Kullanıcıların kaydedilmesi, güncellenmesi ve silinmesi. 
• Kullanıcı yetkilendirme ve oturum yönetimi. 
Daire Yönetimi: 
• Dairelerin kaydedilmesi, güncellenmesi ve silinmesi. 
• Ödemelerin kaydedilmesi ve takibi. 
Otopark Yönetimi: 
• Park yerlerinin kaydedilmesi ve yönetilmesi. 
• Rezervasyon sistemi. 
Site Güvenliği: 
• Güvenlik görevlilerinin kaydedilmesi ve vardiya takibi. 
• Giriş/çıkış kayıtlarının tutulması. 
Kulüp/Spor Salonu Yönetimi: 
• Kulüp ve spor salonunun kaydedilmesi ve yönetilmesi. 
• Üyelik bilgilerinin kaydedilmesi ve üyelik yönetimi. 
Site Temizlik Görevleri: 
• Temizlik görevlerinin kaydedilmesi ve programlanması. 
• Temizlik görevlerinin takibi ve güncellenmesi. 
Performans Gereksinimleri: 
• Sistemin hızlı ve güvenilir olması.   
• Veritabanı işlemlerinin hızlı ve verimli yapılması.  
• Kullanıcıların anlık güncellemelere kolayca erişebilmesi. 
Güvenlik Gereksinimleri: 
• Kullanıcıların gizli bilgilerinin güvenliği (şifreleme, güvenli oturum yönetimi vb.) 
• Veritabanı güvenliği (yetkilendirme, yetki yönetimi, yedekleme vb.) 
İş Kuralları 
Apartman – Daireler (N:1)  
Bir apartmanda birden fazla daire bulunur. 
Bir daire bir apartmanda bulunabilir. 
Apartman – Apartman Yöneticisi (1:1) 
Bir apartmanı bir yönetici yönetir. 
Bir yönetici bir apartmanı yönetebilir. 
Apartman – Site Temizlik Görevi (N:M) 
Bir apartmanda birden fazla temizlik görevi olur. 
Bir temizlik görevi birden fazla apartmanda olabilir. 
Daireler – Otopark Alanı (N:M) 
Bir daire birden fazla otopark kullanabilir. 
Bir otoparkı birden fazla daire kullanır. 
Daire Telefonları – Site Güvenliği Telefon Numaraları (1:N) 
Site güvenliğinde tüm telefon numaraları bulunur. 
Bir dairede bir telefon bulunur. 
Daireler – Araba (N:1)  
Bir dairede birden fazla arabaya sahip olabilir. 
Bir araba bir daireye sahiptir. 
Daireler – Apartman Sakinleri (N:1) 
Bir dairede birden fazla daire sakini oturur. 
Bir apartman sakini bir dairede oturur. 
Apartman Sakinleri – Apartman Yöneticisi (1:1) 
Bir apartman sakini yönetici olabilir 
Bir yönetici aynı zamanda apartman sakinidir 
Apartman Sakinleri – Kulüp Üyeleri (N:M) 
Bir apartman sakini birden fazla kulübe üye olabilir. 
Bir kulübün birden fazla üyesi olabilir. 
Apartman Sakinleri – Spor Sahası (N:M) 
Bir apartman sakini birden fazla spor sahası kullanabilir. 
Bir spor sahasını birden fazla apartman sakini kullanabilir. 
Site Temizlik Personeli – Site Temizlik Malzemeleri (N:M)  
Bir temizlik personeli birden fazla malzeme kullanabilir. 
Bir malzemeyi birden fazla temizlikçi kullanabilir. 
Site Temizlik Personeli – Site Temizlik Görevi (N:M) 
Bir personel birden fazla görevi yapabilir. 
Bir görevi birden fazla personel yapabilir. 
Site Temizlik Görevi – Otopark (N:M) 
Bir otopark da birden fazla görev bulunabilir. 
Bir temizlik görev bir otopark da bulunur. 
Site Temizlik Görevi – Spor Salonu (N:M) 
Bir spor salanında birden fazla temizlik görevi bulunabilir. 
Bir temizlik görevi birden fazla spor salonunda bulunabilir. 
Spor Sahası Personel – Spor Sahası Türü(N:M) 
Bir spor personelinin birden fazla branşı olabilir. 
Bir branşın birden fazla spor personeli bulunabilir. 
Site Kulüpleri – Kulüp Üyeleri (N:M) 
Bir kulübün birden fazla üyesi olabilir  
Bir üye birden fazla kulübe üye olabilir. 
Site Kulüpleri – Kulüp Yöneticisi (N:1) 
Bir kulübün bir yöneticisi olur. 
Bir yönetici birden fazla kulüp yönetebilir.


### Adım 4 
Phpmyadmin de sql sekmesine tıklayın ve github sayfasında bulunan Tabloya_Veri_Ekleme.sql ve Etkinlikler.sql sorgularını çalıştırın.(Tabloya_Veri_Ekleme.sql deki sorguyu yükledikten sonra kullanici_kayit tablosuna gidin oradaki sql sekmesine tıkladıktan 
sonra Etkinlikler.sql sorgusunu çalıştırın)<br>  
![](/Veri_Tabanina_Erisim/3.png)  
![](/Veri_Tabanina_Erisim/4.png)
![](/Veri_Tabanina_Erisim/2.png)<br>
Tablolar bu şekilde gözükmelidir.<br>
![](/Veri_Tabanina_Erisim/5.png)
