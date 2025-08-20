# 🍦 Dogi Soft Ice Cream Teknik Destek Sistemi

<div align="center">

![Dogi Logo](https://dogisofticecream.com.tr/wp-content/uploads/2025/02/dogilogo.png)

**AI Destekli 7/24 Teknik Destek Platformu**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)

</div>

## 📖 Proje Hakkında

Bu proje, **Doğuş Otomat** şirketi için geliştirilmiş, **Dogi Soft Ice Cream** makinalarına özel AI destekli teknik destek sistemidir. Google Gemini AI teknolojisi kullanarak 7/24 kesintisiz teknik destek hizmeti sunar.

### ✨ Özellikler

- 🤖 **AI Destekli Teknik Destek** - Google Gemini 2.0 Flash modeli ile güçlendirilmiş
- 🔧 **Kapsamlı Hata Kodu Veritabanı** - 40+ hata kodu ve çözümü (00-42, 240)
- 📱 **Responsive Tasarım** - Tüm cihazlarda mükemmel görüntü
- 🎨 **Modern UI/UX** - Glass morphism efektleri ve animasyonlar
- 🔒 **Güvenli API Yönetimi** - Yerel depolama ve şifreli bağlantılar
- 🌟 **Gerçek Zamanlı Chat** - Anlık teknik destek deneyimi
- 🔍 **Detaylı Tanı Sistemi** - Adım adım sorun giderme rehberleri

### 🎯 Desteklenen Hata Kodları

| Kod Aralığı | Açıklama | Örnek |
|-------------|----------|-------|
| **00-04** | Reçel & Dondurma Sistemi | `00` Reçel Eksikliği, `01` Dondurma Yanıt Vermeme |
| **05-07** | Koruma Kapağı Motoru | `05` Açık Devre, `06` Kısa Devre |
| **08-11** | Y Motoru Sistemi | `08` Başlangıç Noktası, `09` Açık Devre |
| **12-15** | X Motoru Sistemi | `12` Konum Sensörü, `13` Elektrik Bağlantısı |
| **16-19** | Bardak Sistemi | `16` Düşme Sensörü, `18` Dağıtıcı |
| **20-25** | Kapı & Mekanik | `20` Kapı Motoru, `22` Yuvarlama |
| **26-29** | Z Motoru | `26` Zaman Aşımı, `27` Açık Devre |
| **30-36** | Reçel Motoru & Valf | `30` Motor Açık Devre, `35` Aşırı Akım |
| **37-42** | Robot & Kilit Sistemi | `37` Robot Kolu, `40` Kapı Kilidi |
| **240** | Memory Hatası | EEPROM Depolama Sorunu |

## 🚀 Kurulum ve Kullanım

### Gereksinimler
- Modern web tarayıcısı (Chrome, Firefox, Safari, Edge)
- Google Gemini API anahtarı
- İnternet bağlantısı

### Adımlar

1. **Repository'yi klonlayın:**
```bash
git clone https://github.com/yourusername/dogi-teknik-destek.git
cd dogi-teknik-destek
```

2. **HTML dosyasını tarayıcıda açın:**
   - `dogi_icecream_websiteMK2.html` (Ana versiyon - Önerilen)
   - `dogi_icecream_website (1).html` (Gelişmiş özelliklerle)
   - `dogiicream.html` (Basit versiyon)

3. **Google Gemini API Anahtarı alın:**
   - [Google AI Studio](https://makersuite.google.com/app/apikey) sayfasına gidin
   - "Create API Key" butonuna tıklayın
   - Oluşturulan anahtarı kopyalayın

4. **Sistemi başlatın:**
   - API anahtarınızı girin
   - "Teknik Desteği Başlat" butonuna tıklayın
   - Hata kodunuzu veya sorununuzu yazın

## 📁 Dosya Yapısı

```
dogi-teknik-destek/
├── dogi_icecream_websiteMK2.html    # Ana versiyon (Önerilen)
├── dogi_icecream_website (1).html   # Gelişmiş özellikler
├── dogiicream.html                  # Basit versiyon  
├── placeholder.html                 # Placeholder sayfa
├── README.md                        # Bu dosya
└── docs/                           # Dokümantasyon (opsiyonel)
```

## 🎨 Tasarım Özellikleri

### Teknolojiler
- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Styling:** Tailwind CSS, Custom CSS
- **AI Integration:** Google Gemini 2.0 Flash API
- **Fonts:** Inter, Poppins (Google Fonts)

### Görsel Özellikler
- 🌈 **Gradient Backgrounds** - Modern renk geçişleri
- 💎 **Glass Morphism** - Cam efekti tasarım
- ✨ **Floating Particles** - Dinamik arka plan animasyonları
- 🎭 **Smooth Animations** - Akıcı geçiş efektleri
- 📱 **Mobile First** - Mobil öncelikli responsive tasarım

## 🛠️ Teknik Detaylar

### API Entegrasyonu
```javascript
// Google Gemini API çağrısı
const response = await fetch(`https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${API_KEY}`, {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({
        contents: chatHistory,
        generationConfig: {
            temperature: 0.7,
            topK: 40,
            topP: 0.95,
            maxOutputTokens: 2048,
        }
    })
});
```

### Güvenlik Özellikleri
- 🔐 **Yerel API Depolama** - API anahtarları sadece tarayıcıda saklanır
- 🛡️ **HTTPS Bağlantıları** - Tüm API çağrıları şifreli
- 🔒 **Password Masking** - API anahtarı girişi gizli
- ✅ **Input Validation** - Güvenli veri doğrulama

## 📊 Performans

- ⚡ **Hızlı Yükleme** - CDN kullanımı ile optimize edilmiş
- 💾 **Hafif Boyut** - Minimal bağımlılık
- 🔄 **Real-time Response** - Anlık AI yanıtları
- 📱 **Mobile Optimized** - Tüm cihazlarda mükemmel performans

## 🤝 Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/yeni-ozellik`)
3. Commit yapın (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'i push edin (`git push origin feature/yeni-ozellik`)
5. Pull Request oluşturun

## 📄 Lisans

Bu proje **Doğuş Otomat** şirketi için geliştirilmiş özel bir uygulamadır. Ticari kullanım için izin gereklidir.

## 📞 İletişim

- **Şirket:** Doğuş Otomat
- **Website:** [dogisofticecream.com.tr](https://dogisofticecream.com.tr)
- **E-mail:** info@dogisofticecream.com.tr

---

<div align="center">

**Made with ❤️ for Doğuş Otomat**

*Powered by Google Gemini AI • Güvenli ve Hızlı Çözümler*

</div>