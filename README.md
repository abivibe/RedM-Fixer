<div align="center">

# 🔫 REDM FIXER
### RedM Sunucu Önbelleği Temizleyici ve Vulkan Çökme Çözücü
*RedM Server Cache Cleaner & Vulkan Crash Fixer*

[![Release](https://img.shields.io/badge/S%C3%BCr%C3%BCm-v1.0.0-E53935?style=for-the-badge&logo=windows&logoColor=white)](../../releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%2F%2011%20(64--bit)-0078D6?style=for-the-badge&logo=windows11&logoColor=white)](../../releases/latest)
[![License](https://img.shields.io/badge/Lisans-Freeware%20%2F%20Closed--Source-555555?style=for-the-badge)](LICENSE)
[![Vibe Coding](https://img.shields.io/badge/%E2%9C%A8%20Crafted%20with-VIBE%20CODING-8A2BE2?style=for-the-badge)](https://github.com/abivibe/RedM-Fixer)
[![Security](https://img.shields.io/badge/Defender%20Scan-100%25%20CLEAN-success?style=for-the-badge&logo=shield&logoColor=white)](#-g%C3%BCvenlik-ve-vir%C3%BCs-taramas%C4%B1--security--virus-scan)

[![Buy Me A Coffee](https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png)](https://buymeacoffee.com/vibeabi)

---

**[🇹🇷 Türkçe](#-türkçe-rehber) • [🇬🇧 English](#-english-guide) • [⬇️ İndir / Download](../../releases/latest)**

</div>

---

## ⚡ Vibe Coding Ruhunun Ürünü | *Born from Vibe Coding*

> **🇹🇷 Türkçe:**  
> **RedM Fixer**, karmaşık klasör yolları ve manuel dosya silme çilesinin ötesinde, tamamen **✨ Vibe Coding** felsefesiyle hayata geçirildi. Sıkıcı komut satırları yerine; sezgisel akış, dinamik artan glow estetiği, zarif ilerleme çubuğu ve sıfır hata toleranslı akıllı hedefleme mimarisiyle tasarlandı.
>
> **🇬🇧 English:**  
> **RedM Fixer** was crafted beyond tedious folder navigation and manual cache purging—brought to life entirely through the **✨ Vibe Coding** philosophy. Designed with intuitive flow, an elegant dynamic glow aesthetic, a sleek progress bar, and smart fail-safe target detection!

---

# 🇹🇷 Türkçe Rehber

## 🔫 RedM Fixer Nedir?
Red Dead Redemption 2'nin popüler çok oyunculu istemcisi **RedM** oynarken sunucuya bağlanırken takılmalardan, bitmek bilmeyen yükleme ekranlarından veya aniden masaüstüne fırlatan Vulkan render hatalarından sıkılmadınız mı?

**RedM Fixer**, oyuncuların karşılaştığı tüm önbellek, NUI ve Vulkan başlatma sorunlarını saniyeler içinde çözen; **Obsidian Koyu Temalı**, ultra zarif ve bağımsız (portable) bir onarım aracıdır.

---

## 🛠️ Hangi Hataları Çözer?

1. **Sunucu & NUI Önbellek Bozulmaları:**
   - Sunucuya bağlanırken sonsuz yükleme döngüsünde (*Infinite Loading / Downloading Resources*) kalma.
   - `Failed to fetch resource`, `Resource download failed` veya eksik sunucu varlıkları.
   - NUI depolama çakışmaları nedeniyle envanter, harita ve oyun içi kullanıcı arayüzlerinin açılmaması veya donması.

2. **Vulkan & Render Başlangıç Çökmeleri:**
   - Oyun açılırken karşılaşılan meşhur **`ERR_GFX_STATE`** çökmesi.
   - RedM başlatılırken meydana gelen Vulkan API ve grafik başlatma hataları.
   - Bozuk `citizen`, `bin` veya `crashes` kütüphanelerinin sebep olduğu başlatılamama durumu.

3. **Yönetici Yetkisi Çakışması (*Elevated Privileges* Hatası):**
   - RedM'in *"RedM does not support running under elevated privileges. Please change your Windows settings to not run RedM as administrator. The game will exit now."* uyarısı vererek kapanmasını engeller.
   - Temizlik sonrası oyunu başlatırken Windows Explorer'ın standart kullanıcı (*Medium Integrity*) güvenlik belirtecini kopyalar ve oyunu yönetici yetkisi olmadan kusursuz başlatır.

4. **Hedef Bulunamama & Yanlış Klasör Problemleri:**
   - `citizen` veya `bin` klasörleri silinmiş olsa dahi `CitizenFX.ini`, `RedM.installroot`, `CitizenGame.dll` ve kayıt defteri belirteçleriyle kurulum dizinini **%100 kesinlikle** otomatik bulur.
   - Doğrulama sağlandığında kullanıcıya görsel kanıt sunmak için klasörü Windows Gezgini'nde açar ve 3 saniye sonra otomatik olarak kapatır.

---

## 🔘 Seçenekler Ne İşe Yarar?

### 1. Server Cache Temizliği (*Server Cache Clean*)
- **Ne Yapar?** `data` alt klasörü içerisindeki `server-cache`, `server-cache-priv`, `cache`, `nui` ve `nui-storage` klasörlerini güvenli bir şekilde siler.
- **Ne İşe Yarar?** Oyunun ana sistem ve çalışma dosyalarına dokunmaz; yalnızca sunuculardan indirilmiş bozulmuş, çakışan veya güncelliğini yitirmiş geçici dosyaları sıfırlar. Sunucuya bir sonraki girişinizde varlıklar temiz olarak baştan indirilir.
- **Ne Zaman Kullanılmalı?** Sunucuya bağlanırken indirme takıldığında, oyun içi menüler bozulduğunda veya sunucu paket güncellemelerinden sonra.

### 2. Vulkan Error Fix
- **Ne Yapar?** Ana dizindeki `crashes`, `logs`, `citizen` ve `bin` klasörleri ile `data` altındaki `cache` ve `nui-storage` klasörlerini tamamen sıfırlar.
- **Ne İşe Yarar?** Bozuk grafik shader önbelleklerini ve hasar görmüş çalışma kütüphanelerini temizler. RedM bir sonraki açılışında `citizen` ve `bin` kütüphanelerini resmi CitizenFX sunucularından en güncel ve sağlam halleriyle otomatik olarak baştan indirir.
- **Ne Zaman Kullanılmalı?** RedM açılırken hata verip çöktüğünde, Vulkan API başlatma hatası veya `ERR_GFX_STATE` uyarısı aldığınızda. *(Eğer sorun devam ederse ekran kartı sürücülerinizi ve Windows güncellemelerinizi kontrol etmeniz önerilir).*

---

## 🌟 Öne Çıkan Özellikler

- **💫 Dinamik Artan Glow & Zarif Progress Bar:** Temizlik aşaması ilerledikçe (%0 → %100) parlaklığı ve etki alanı dinamik olarak artan RedM kırmızısı glow efekti ve degrade dolgulu pürüzsüz ilerleme çubuğu.
- **🛡️ Sade ve Temiz Arayüz:** Temizlik sırasında karmaşık dosya yolları gösterilmez; işlem bitiminde kaç adet dosyanın silindiği rozet olarak gösterilir (*Örn: `1.428 dosya başarıyla temizlendi`*).
- **🌓 Koyu / Aydınlık Tema:** Başlık çubuğundaki interaktif butonla tek tıkla Deep Obsidian Koyu Tema (`🌙`) ile Modern Aydınlık Tema (`☀️`) arasında anında geçiş.
- **🌐 Çift Dil Desteği:** Türkçe ve İngilizce dil seçenekleri.
- **🚀 Sıfır Bağımlılık (Standalone):** .NET 8 Desktop Runtime doğrudan exe içerisine gömülüdür. Kullanıcının bilgisayarında herhangi bir ek runtime veya kütüphane kurulu olmasına gerek yoktur; tek tıkla çalışır.

---

## 📥 Nasıl İndirilir ve Kullanılır?

1. Sağ taraftaki **[Releases](../../releases/latest)** bölümünden en güncel **`RedMFixer-v1.0.0-win-x64.zip`** arşivini indirin.
2. Arşiv içeriğini masaüstüne veya dilediğiniz bir klasöre çıkartın.
3. **`RedMFixer.exe`** dosyasını çalıştırın.
4. Program RedM kurulum dizininizi otomatik olarak algılayıp onaylayacaktır.
5. İhtiyacınıza göre **Server Cache Temizliği** veya **Vulkan Error Fix** seçeneğini işaretleyip **TEMİZLE** butonuna basın.
6. Temizlik bittiğinde **"Evet, Başlat"** diyerek RedM'i yönetici hatasına takılmadan doğrudan başlatabilirsiniz.

---

# 🇬🇧 English Guide

## 🔫 What is RedM Fixer?
Tired of infinite loading screens, corrupted asset downloads, or sudden Vulkan render crashes while trying to play **RedM**?

**RedM Fixer** is an ultra-fast, minimalist, and portable utility designed to wipe out cache corruption, NUI storage conflicts, and Vulkan engine startup errors in seconds.

---

## 🛠️ Which Errors Does It Solve?

1. **Server & NUI Cache Corruption:**
   - Getting stuck on the infinite loading screen (*Downloading Resources* loop).
   - `Failed to fetch resource` and missing server stream assets.
   - NUI storage conflicts causing in-game menus, UI, and inventories to freeze or fail to render.

2. **Vulkan & Render Startup Crashes:**
   - The infamous **`ERR_GFX_STATE`** crash on game launch.
   - Vulkan API initialization and pipeline state object (PSO) failures.
   - Broken `citizen`, `bin`, or `crashes` binaries preventing RedM from booting.

3. **Elevated Privileges Conflict:**
   - Bypasses the strict *"RedM does not support running under elevated privileges"* block.
   - Duplicates the standard Windows Explorer user token (*Medium Integrity*) to launch RedM safely without administrative elevation errors.

4. **Directory Detection Failures:**
   - Accurately detects the RedM installation directory via deep registry scanning and critical markers (`CitizenFX.ini`, `RedM.installroot`, `CitizenGame.dll`), even if `citizen` or `bin` were previously deleted.
   - Flashes the detected folder in Windows Explorer for 3 seconds as visual proof before returning to the app.

---

## 🔘 What Do The Options Do?

### 1. Server Cache Clean
- **What it does:** Safely purges `server-cache`, `server-cache-priv`, `cache`, `nui`, and `nui-storage` inside the `data` directory.
- **Why use it:** Resets cached server downloads and UI states without touching core game files. Fresh assets will be automatically re-downloaded upon reconnecting.
- **When to use:** When stuck joining a server, experiencing broken UI/NUI menus, or after server-side updates.

### 2. Vulkan Error Fix
- **What it does:** Completely purges `crashes`, `logs`, `citizen`, and `bin` folders, along with `cache` and `nui-storage` inside `data`.
- **Why use it:** Clears corrupted shader caches and runtime assemblies. On the next launch, RedM automatically pulls fresh, pristine binaries from the official CitizenFX CDN.
- **When to use:** When RedM crashes on startup, throws `ERR_GFX_STATE`, or fails Vulkan device initialization.

---

## 🛡️ Güvenlik ve Virüs Taraması | Security & Virus Scan

*The release archive (`RedMFixer-v1.0.0-win-x64.zip`) is verified 100% clean prior to publication.*

| Kontrol / Check | Değer / Value | Detay / Details |
| :--- | :--- | :--- |
| **Arşiv Adı / File Name** | `RedMFixer-v1.0.0-win-x64.zip` | Windows 64-bit Taşınabilir Paket (Standalone) |
| **Dosya Boyutu / File Size** | `57.6 MB` (`60,471,542 bytes`) | .NET 8 Desktop Runtime Gömülü / Self-Contained |
| **Microsoft Defender Antivirus** | ✅ **TEMİZ / CLEAN (0 Tehdit)** | Özel Tam Dosya Taraması (`MpCmdRun`) |
| **SHA-256 Doğrulama / Hash** | `C49891A8EFEB29D059D53649587BB553A2B79DACE2F1AD58092D0128EADA926D` | `CertUtil -hashfile RedMFixer-v1.0.0-win-x64.zip SHA256` |

---

## 🔒 Kapalı Kaynak Dağıtım Bildirimi | Closed Source Notice

> **🇹🇷 Türkçe:**  
> RedM Fixer, güvenli ve bağımsız bir freeware araç olarak dağıtılmaktadır. Kaynak kodları kapalıdır. İndirme ve kullanım tamamen ücretsizdir.
>
> **🇬🇧 English:**  
> RedM Fixer is distributed as a secure, standalone freeware utility. The source code is closed-source. Free for personal, non-commercial use.

---

<div align="center">

**Crafted with 🖤 & ✨ Vibe Coding by [@abivibe](https://github.com/abivibe)**

</div>
