# 🧠 Kitapsepeti Otomasyon Test Projesi

Bu proje, **Cypress** kullanılarak hazırlanmış otomasyon testlerini içermektedir.  
Amaç, **Kitapsepeti** web sitesindeki temel kullanıcı akışlarını (giriş, arama, sepet, ödeme vb.) uçtan uca test etmektir.  

---

## 🧩 Test Senaryoları (User Story Bazlı)

| **User Story** | **Acceptance Criteria (AC)** | **Test Dosyası** | **Durum** |
|----------------|------------------------------|------------------|------------|
| **US01 - Kullanıcı Girişi** | AC1–AC4: Giriş sayfası, alan kontrolleri ve başarılı login | `US01AC1-4-login.cy.js` | ✅ Pass |
| | AC5–AC7: Hatalı giriş kontrolleri | `US01AC5-7-login-negative.cy.js` | ✅ Pass |
| | AC8: Çok fazla hatalı giriş limiti | `US01AC8-repeat.cy.js` | ✅ Pass |
| | AC9: Şifremi unuttum akışı | `US01AC9-sifremi-unuttum.cy.js` | ✅ Pass |
| **US02 - Arama ve Ürün Listeleme** | AC1–AC9: Arama, filtreleme, sıralama ve sonsuz kaydırma | `US02-arama-ve-listeleme.cy.js` | ✅ Pass |
| **US03 - Sepete Ürün Ekleme** | AC1–AC4: Ürün ekleme, popup, sepet yönlendirme | `US03-sepete-ürün-ekleme.cy.js` | ✅ Pass |
| **US04 - Sepet Yönetimi ve Kontrolü** | AC1–AC5: Sepete erişim, fiyat kontrolü, adet güncelleme, ürün silme | `US04-sepet-yönetimi.cy.js` | ✅ Pass |
| | AC6–AC7: Boş sepet ve mesaj kontrolleri | `US04AC6-7-boş-sepet.cy.js` | ✅ Pass |
| | AC9–AC10: Ana sayfadan sepete yönlendirme | `US04AC9-10-anasayfadan-sepete.cy.js` | ✅ Pass |
| **US05 - Ödeme ve Sipariş Onayı** | AC1–AC8: Adres, kargo, ödeme ekranı, form alanları | `US05-ödeme-ve-sipariş-onayı.cy.js` | ✅ Pass |
| **US06 - Misafir Olarak Satın Alma** | AC1–AC6: Üye olmadan satın alma akışı | `US06-misafir-olarak-satın-alma.cy.js` | ✅ Pass |

---

## ⚙️ Kullanılan Teknolojiler
- **Cypress v14.0.3**
- **Node.js v18**
- **JavaScript (ES6)**
- **Page Object Model (POM) yapısı**
- **GitHub Actions CI/CD pipeline**

---

## 📊 Test Çıktıları
- Tüm testler local ortamda **PASS** durumunda tamamlanmıştır.  
- GitHub Actions pipeline’ında testler otomatik olarak çalışmaktadır.  
- Video ve ekran görüntüleri `cypress/videos/` ve `cypress/screenshots/` klasörlerinde tutulur.

---

[Videoları buradan indirilebilir](https://drive.google.com/file/d/1DPuqwLURehG7oTaos6HjFJf6lmx219bX/view?usp=sharing))
