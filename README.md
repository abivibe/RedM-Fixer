<div align="center">

# 🔫 REDM FIXER
### RedM Sunucu Önbelleği Temizleyici ve Vulkan Çökme Çözücü
*RedM Server Cache Cleaner & Vulkan Crash Fixer*

[![Release](https://img.shields.io/badge/S%C3%BCr%C3%BCm-v1.0.0-E53935?style=for-the-badge&logo=windows&logoColor=white)](../../releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%2F%2011%20(64--bit)-0078D6?style=for-the-badge&logo=windows11&logoColor=white)](../../releases/latest)
[![License](https://img.shields.io/badge/Lisans-Freeware%20%2F%20Closed--Source-555555?style=for-the-badge)](LICENSE)
[![Security](https://img.shields.io/badge/Defender%20Scan-100%25%20CLEAN-success?style=for-the-badge&logo=shield&logoColor=white)](#-g%C3%BCvenlik-ve-vir%C3%BCs-taramas%C4%B1)

[![Buy Me A Coffee](https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png)](https://buymeacoffee.com/vibeabi)

---

**[🇹🇷 Türkçe](#-türkçe) • [🇬🇧 English](#-english) • [⬇️ İndir / Download](../../releases/latest)**

</div>

---

# 🇹🇷 Türkçe

## 📌 RedM Fixer Ne İşe Yarar?
**RedM Fixer**, Red Dead Redemption 2'nin multiplayer modu olan RedM'de sıkça karşılaşılan önbellek bozulmalarını, sunucuya bağlanırken yaşanan sonsuz yükleme takılmalarını ve Vulkan grafik çökmelerini tek tıkla çözen pratik bir onarım aracıdır.

### 🛠️ Çözdüğü Hatalar
- **Sunucu & NUI Önbellek Hataları:** Sunucuya bağlanırken yaşanan sonsuz yükleme takılmaları (*Downloading Resources* döngüsü), `Failed to fetch resource` hataları ve bozuk envanter/menü arayüzleri.
- **Vulkan & Başlangıç Çökmeleri:** Oyun açılırken karşılaşılan **`ERR_GFX_STATE`** hatası ve Vulkan API render çökmeleri.

---

## 🔘 Seçenekler

### 1. Server Cache Temizliği (*Server Cache Clean*)
- **Ne Yapar?** `data` alt klasöründeki geçici sunucu önbelleklerini (`server-cache`, `cache`, `nui`, `nui-storage`) temizler.
- **Ne Zaman Kullanılır?** Sunucuya bağlanırken indirme takıldığında, harita/envanter açılmadığında veya sunucu güncellemelerinden sonra. Oyunun ana sistem dosyalarına dokunmaz.

### 2. Vulkan Error Fix
- **Ne Yapar?** `crashes`, `logs`, `citizen` ve `bin` klasörleri ile grafik önbelleklerini sıfırlar. RedM'in bir sonraki açılışta temiz çalışma dosyalarını resmi sunuculardan tekrar indirmesini sağlar.
- **Ne Zaman Kullanılır?** RedM açılırken `ERR_GFX_STATE` veya Vulkan grafik hatası verip kapandığında.

---

## 📥 Kullanım
1. **[Releases](../../releases/latest)** sayfasından **`RedMFixer.rar`** arşivini indirin ve klasöre çıkartın.
2. **`RedMFixer.exe`** dosyasını çalıştırın.
3. Sorununuza göre **Server Cache Temizliği** veya **Vulkan Error Fix** seçeneğini seçip **TEMİZLE** butonuna basın.
4. Temizlik bittiğinde **"Evet, Başlat"** diyerek oyuna girebilirsiniz.

*(.NET 8 Runtime programın içine gömülüdür, ek hiçbir kurulum gerektirmez).*

---

# 🇬🇧 English

## 📌 What Does RedM Fixer Do?
**RedM Fixer** is a straightforward utility designed to resolve cache corruptions, infinite loading loops, and Vulkan render crashes in RedM (Red Dead Redemption 2 multiplayer).

### 🛠️ Errors It Resolves
- **Server & NUI Cache Issues:** Infinite loading screens (*Downloading Resources* loop), `Failed to fetch resource` errors, and broken/freezing in-game UI.
- **Vulkan & Launch Crashes:** The **`ERR_GFX_STATE`** crash and Vulkan API initialization errors on launch.

---

## 🔘 Cleaning Options

### 1. Server Cache Clean
- **What it does:** Safely wipes temporary server cache files (`server-cache`, `cache`, `nui`, `nui-storage`) in the `data` folder.
- **When to use:** When stuck joining a server, experiencing broken UI/inventory, or after server updates. Core game files remain untouched.

### 2. Vulkan Error Fix
- **What it does:** Wipes `crashes`, `logs`, `citizen`, `bin`, and shader cache files, prompting RedM to pull clean binaries from the official CDN on the next boot.
- **When to use:** When RedM crashes on startup with `ERR_GFX_STATE` or graphics device initialization errors.

---

## 📥 How to Use
1. Download **`RedMFixer.rar`** from **[Releases](../../releases/latest)** and extract it.
2. Run **`RedMFixer.exe`**.
3. Select **Server Cache Clean** or **Vulkan Error Fix** and click **CLEAN**.
4. Once completed, click **"Yes, Launch"** to jump into RedM.

*(Standalone portable binary with embedded .NET 8 runtime—no extra dependencies needed).*

---

## 🛡️ Güvenlik ve Virüs Taraması

| Kontrol | Değer |
| :--- | :--- |
| **Dosya** | `RedMFixer.rar` |
| **Boyut** | `48.7 MB` |
| **Tarama** | ✅ Microsoft Defender: **TEMİZ (0 Tehdit)** |
| **SHA-256** | `C0203F6D32C6CF9E0BD7CC51B2E93EE8555D8D6678DF4E909670D7A84B33DA6B` |

---

<div align="center">

**Crafted by [@abivibe](https://github.com/abivibe)**

</div>
