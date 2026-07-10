<div align="center">  
  <a href="README-TR.md"   >   TR <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/TR.png" alt="TR" height="20" /></a>  
  <a href="README-EN.md"> | EN <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/US.png" alt="EN" height="20" /></a>  
  <a href="README-DE.md"> | DE <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/DE.png" alt="DE" height="20" /></a>  
  <a href="README.md"> | NL <img style="padding-top: 8px" src="https://raw.githubusercontent.com/yammadev/flag-icons/master/png/NL.png" alt="NL" height="20" /></a>  
</div>

# DomainNameApi Entegrasyon Dokümantasyonu (TR)

## 📦 İndirme — her zaman Releases kullanın!

⬇️ **En güncel test edilmiş sürümü buradan indirin: https://github.com/domainreseller/hostfact-dna/releases/latest**

> ⚠️ Yeşil **Code → Download ZIP** düğmesini **kullanmayın** — bu düğme ham geliştirme dalını indirir. Release paketleri sürümlendirilmiş, test edilmiş ve canlı ortama hazırdır.

## Kurulum

1.  `domainnameapi` klasörünü `Pro/3rdparty/domain/` dizinine yerleştirin veya FTP ile yükleyin.

## Kontrol Panelinde Yapılandırma

1.  `Kontrol -> Servisler -> Kayıt Operatörleri` bölümüne gidin.

    ![img1.png](img1.png)

2.  **"Kayıt Operatörü Ekle"** düğmesine tıklayın.

    ![img2.png](img2.png)

3.  API olarak **"DomainNameApi"** seçeneğini seçin.


4.  Kullanıcı adınızı ve şifrenizi girin.

    ![img3.png](img3.png)

5.  **"Kaydet"** düğmesine tıklayın.

## 🔑 API Kimlik Bilgileri — Kullanıcı Adı/Şifre mi, Reseller ID/API Key mi?

Her ikisi de desteklenir — bilgileri aynı iki modül alanına girin; modül hangi API'nin kullanılacağını otomatik olarak algılar:

| Elinizdeki bilgi | "Kullanıcı Adı" alanı | "Şifre" alanı | Kullanılan API |
|---|---|---|---|
| **Yeni panel kimlik bilgileri** (önerilen) | Reseller ID — `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` biçiminde UUID | API Key | REST |
| **Eski (legacy) kimlik bilgileri** | API kullanıcı adı | API şifresi | SOAP |

> 💡 **Reseller ID** ve **API Key** bilgilerinizi DomainNameAPI panelinizdeki **API Ayarları** bölümünde bulabilirsiniz.
> ⚠️ Bunlar **API kimlik bilgileridir** — panele giriş yaptığınız e-posta/şifre burada **ÇALIŞMAZ**; API Ayarları bölümündeki Reseller ID (UUID) ve API Key kullanılmalıdır.

Ek bir yapılandırma gerekmez — kullanıcı adı alanında bir UUID varsa modül modern REST API'yi, aksi halde klasik SOAP API'yi kullanır.

## Alan Adlarını İçe Aktarma

1.  Kayıt operatörü ayarlarını kaydettikten sonra, alan adı içe aktarma ekranına yönlendirileceksiniz.
2.  Burada istediğiniz alan adlarını seçip içe aktarabilirsiniz.

    ![img4.png](img4.png)
    ![img5.png](img5.png)

## Kullanım

1.  Yapılandırma ve içe aktarma işleminden sonra, DomainNameApi entegrasyonu aracılığıyla ürünler oluşturabilir, alan adlarını kaydedebilir ve yönetebilirsiniz.

    ![img6.png](img6.png) 