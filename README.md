# 🏰 Lords Realm - 3D Prosedural Krallıq Xəritəsi (Lords Mobile Style)

Üçölçülü (3D) RTS və strategiya oyunları üçün hazırlanmış, toxum (seed) əsaslı prosedural dünya xəritəsi mühərriki.

![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=flat-square&logo=three.js)
![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange?style=flat-square&logo=html5)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla_ES6+-yellow?style=flat-square&logo=javascript)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)

---

## 🌟 Xüsusiyyətlər

- **Düz 2D Zəmin & 3D Stilizə Obyektlər**:
  - Zəmin düz relyef müstəvisidir (`Y = 0`), üzərində isə stilizə edilmiş 3D aşağı poliqonlu (low-poly) ağaclar, dağlar, qayalar və resurs yataqları yerləşir.
- **Təbii Landşaft & Biomlar**:
  - **Münbit Yaşıllıq**: Zümrüd, təzə ot və günəşli çəmən çalarları.
  - **Qıvrılan Təbii Cığırlar**: Heç bir süni düz xətt və ya "X" kəsişməsi olmadan, Catmull-Rom əyriləri ilə relyef boyunca axan qədim daş və torpaq cığırları.
  - **Dinamik Çay & Sahillər**: Hər toxumda (seed) fərqli axan, lakin eyni toxum daxilində tam stabil qalan prosedural çay və qumlu sahillər.
  - **Qızıl Səhra & Münbit Torpaq Zonaları**: Dyunlar və zəngin torpaq sahələri.
  - **Qarlı Zirvəli Dağlar & Qayalıqlar**: Təbii qaya daşları və qarlı zirvələr.
- **Stilizə 3D Resurs Obyektləri**:
  - Qızıl mədənləri (parlaq kristal yatağı)
  - Daş karxanaları (təbii qaya yığını)
  - Meşə düşərgəsi (odun kütükləri)
  - Təbii ferma və taxıl dəyirmanı
  - Fıstıq, şam və səhra palma ağacları
- **RTS Kamera Nəzarəti**:
  - Sol kliklə xəritəni rahat sürükləmə (pan)
  - Siçan təkəri (scroll) ilə yaxınlaşdırma / uzaqlaşdırma (zoom)
  - `Q` / `E` və ya düymələrlə yalnız Y oxu ətrafında 360° üfüqi fırlanma (ekranın tərsinə çevrilməsinin qarşısı tam alınıb)
- **Taktiki Radar (Mini-xəritə)**:
  - Real vaxt rejimində mövqeyi və təbii relyefi göstərən dinamik radar.
- **Ərazi Detektor Kartı**:
  - Xəritədəki istənilən koordinata klikləyərək biom məlumatlarını və resursları yoxlamaq imkanı.

---

## 🚀 Necə İşə Salmaq Olar?

Heç bir xarici asılılıq quraşdırmağa ehtiyac yoxdur.

1. Layihəni klonlayın:
   ```bash
   git clone https://github.com/fred0128/oyunn.git
   cd oyunn
   ```
2. `index.html` faylını birbaşa istənilən müasir brauzerdə açın və ya yerli server ilə başladın:
   ```bash
   # Python ilə:
   python -m http.server 8080

   # və ya Node.js ilə:
   npx serve .
   ```
3. Brauzerinizdə `http://localhost:8080` ünvanına daxil olun.

---

## 🎮 İdarəetmə Düymələri

| Düymə / Hərəkət | Təyinatı |
|---|---|
| **Sol Klik + Sürükləmə** | Xəritəni sağa-sola, irəli-geri hərəkət etdirmək |
| **Q / E** (və ya ekran düymələri) | Kameranı sola / sağa fırlatmaq |
| **Siçan Təkəri (Scroll)** | Yaxınlaşdırmaq / Uzaqlaşdırmaq |
| **W / A / S / D** və ya Oxlar | Səlis kamera naviqasiyası |
| **Sol Klik (Obyektə)** | Həmin nöqtənin koordinat və biom detallarını açmaq |
| **Təsadüfi Seed** | Xəritəni yeni parametrlərlə yenidən yaratmaq |

---

## 🛠 Texnologiyalar

- **Three.js (r128)** — 3D qrafika və render mühərriki
- **HTML5 Canvas 2D** — Yüksək dəqiqlikli dinamik tekstura və radar generasiyası
- **Simplex / Perlin Noise** — Prosedural relyef və rəng paylanması
- **CSS3 Modern UI** — Şüşə effekti (glassmorphism) və RTS interfeysi
