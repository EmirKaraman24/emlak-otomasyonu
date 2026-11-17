<div align="center">

# 🏠 Emlak Otomasyonu — PHP & MySQL

[![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)](#)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](#)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](#)

Saf **PHP**, **HTML/CSS** ve **MySQL** kullanılarak geliştirilmiş emlak ilan, müşteri/danışman yönetimi, randevu ve teklif takip otomasyonu.

</div>

---

## ✨ Öne Çıkan Özellikler

* **🔐 Kimlik Doğrulama & Rol Ayrımı**
  * Danışman kayıt (`kayit.php`) ve giriş (`giris.php`)
  * Müşteri kayıt (`müşterikayit.php`) ve giriş (`müşterigiriş.php`)
  * Oturum tabanlı erişim kontrolü ve çıkış (`cikis.php`)
* **🏘️ İlan Yönetimi (CRUD)**
  * Danışman panelinden modal tabanlı ilan ekleme, düzenleme ve silme (`mulkler.php`, `ilan_duzenle.php`, `ilan_sil.php`)
  * Genel ilan kataloğu ve detay sayfası (`index.php`, `detay.php`)
* **📅 Teklif, Randevu ve Satış Takibi**
  * İlanlara teklif verme ve yönetme (`teklifler.php`)
  * Gösterim randevusu oluşturma (`randevular.php`)
  * Veritabanı tetikleyicisi (`trigger`) destekli satış/kiralama sonuçlandırma (`satislar.php`)
* **📊 Danışman Kontrol Paneli**
  * Özet KPI kartları, son müşteriler ve yaklaşan randevular (`acilis.php`)
  * Profil yönetimi (`profil.php`)

---

## 📂 Proje Yapısı

```text
emlak-otomasyonu/
├── Database/
│   ├── realestate.sql              # Tablolar, indeksler, view ve trigger içeren MySQL dökümü
│   ├── realestate-ER-diagram.png   # Veritabanı ER diyagramı
│   └── realestate.pdf              # Veritabanı dokümantasyonu
├── Website/
│   ├── index.php                   # Ana ilan kataloğu
│   ├── detay.php                   # İlan detay sayfası
│   ├── acilis.php                  # Danışman kontrol paneli
│   ├── mulkler.php                 # İlan yönetimi (CRUD)
│   ├── teklifler.php               # Teklif takibi
│   ├── randevular.php              # Randevu yönetimi
│   ├── satislar.php                # Satış kayıtları
│   ├── profil.php                  # Profil ayarları
│   ├── baglanti.php                # Veritabanı bağlantısı
│   ├── css/ & img/                 # Arayüz stilleri ve görseller
└── 118_rapor.pdf                   # Proje raporu
```

---

## 🚀 Kurulum (XAMPP / Yerel Sunucu)

1. Depoyu XAMPP'in `htdocs/` klasörüne klonlayın:
   ```bash
   git clone https://github.com/EmirKaraman24/emlak-otomasyonu.git
   ```
2. **phpMyAdmin** üzerinden yeni bir veritabanı oluşturun ve `Database/realestate.sql` dosyasını içe aktarın.
3. `Website/baglanti.php` içindeki MySQL bağlantı bilgilerini kendi ortamınıza göre güncelleyin.
4. Tarayıcıdan projeyi açın:
   ```text
   http://localhost/emlak-otomasyonu/Website/
   ```

---

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) altında sunulmaktadır.
