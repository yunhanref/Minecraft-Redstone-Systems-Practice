# Create a beautiful, highly modern and animated README.md file for the user's Minecraft Redstone project.
# We will use inline animated SVG directly inside the Markdown to achieve the requested "animations and effects" that work natively on GitHub.

svg_banner = """<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 880 260" width="100%">
  <defs>
    <style>
      @keyframes pulse {
        0%, 100% { stroke: #550a0a; filter: drop-shadow(0px 0px 0px #000); }
        50% { stroke: #ff2200; filter: drop-shadow(0px 0px 8px #ff2200); }
      }
      @keyframes torch-glow {
        0%, 100% { fill: #440505; filter: drop-shadow(0px 0px 0px #000); }
        50% { fill: #ff4411; filter: drop-shadow(0px 0px 12px #ff4411); }
      }
      @keyframes signal {
        0% { stroke-dashoffset: 40; }
        100% { stroke-dashoffset: 0; }
      }
      .grid-line { stroke: #1f242c; stroke-width: 1; }
      .wire { stroke-width: 6; stroke-linecap: round; stroke-linejoin: round; fill: none; stroke-dasharray: 8 4; animation: pulse 2.5s infinite, signal 5s linear infinite; }
      .wire-static { stroke: #2a0505; stroke-width: 6; stroke-linecap: round; fill: none; }
      .torch-head { animation: torch-glow 2.5s infinite; }
      .text-title { font-family: 'Segoe UI', system-ui, -apple-system, sans-serif; font-weight: 800; fill: #f0f6fc; font-size: 24px; letter-spacing: 2px; }
      .text-subtitle { font-family: 'Segoe UI', system-ui, sans-serif; font-weight: 400; fill: #8b949e; font-size: 14px; }
      .gate-box { fill: #161b22; stroke: #30363d; stroke-width: 2; rx: 8px; }
    </style>
  </defs>

  <rect width="100%" height="100%" fill="#0d1117" rx="12"/>

  <g>
    <line x1="40" y1="0" x2="40" y2="260" class="grid-line" />
    <line x1="80" y1="0" x2="80" y2="260" class="grid-line" />
    <line x1="120" y1="0" x2="120" y2="260" class="grid-line" />
    <line x1="160" y1="0" x2="160" y2="260" class="grid-line" />
    <line x1="200" y1="0" x2="200" y2="260" class="grid-line" />
    <line x1="240" y1="0" x2="240" y2="260" class="grid-line" />
    <line x1="280" y1="0" x2="280" y2="260" class="grid-line" />
    <line x1="320" y1="0" x2="320" y2="260" class="grid-line" />
    <line x1="360" y1="0" x2="360" y2="260" class="grid-line" />
    <line x1="400" y1="0" x2="400" y2="260" class="grid-line" />
    <line x1="440" y1="0" x2="440" y2="260" class="grid-line" />
    <line x1="480" y1="0" x2="480" y2="260" class="grid-line" />
    <line x1="520" y1="0" x2="520" y2="260" class="grid-line" />
    <line x1="560" y1="0" x2="560" y2="260" class="grid-line" />
    <line x1="600" y1="0" x2="600" y2="260" class="grid-line" />
    <line x1="640" y1="0" x2="640" y2="260" class="grid-line" />
    <line x1="680" y1="0" x2="680" y2="260" class="grid-line" />
    <line x1="720" y1="0" x2="720" y2="260" class="grid-line" />
    <line x1="760" y1="0" x2="760" y2="260" class="grid-line" />
    <line x1="800" y1="0" x2="800" y2="260" class="grid-line" />
    <line x1="840" y1="0" x2="840" y2="260" class="grid-line" />

    <line x1="0" y1="40" x2="880" y2="40" class="grid-line" />
    <line x1="0" y1="80" x2="880" y2="80" class="grid-line" />
    <line x1="0" y1="120" x2="880" y2="120" class="grid-line" />
    <line x1="0" y1="160" x2="880" y2="160" class="grid-line" />
    <line x1="0" y1="200" x2="880" y2="200" class="grid-line" />
    <line x1="0" y1="240" x2="880" y2="240" class="grid-line" />
  </g>

  <path d="M 60,130 L 220,130 L 220,90 L 340,90 M 220,130 L 220,170 L 340,170" class="wire" />
  
  <rect x="340" y="60" width="100" height="60" class="gate-box" />
  <text x="375" y="95" fill="#f0f6fc" font-family="monospace" font-size="14" font-weight="bold">NOT</text>

  <rect x="340" y="140" width="100" height="60" class="gate-box" />
  <text x="362" y="175" fill="#f0f6fc" font-family="monospace" font-size="12" font-weight="bold">REPEATER</text>

  <path d="M 440,90 L 520,90 L 520,130 L 600,130" class="wire" />
  <path d="M 440,170 L 520,170 L 520,130" class="wire" />

  <g transform="translate(590, 105)">
    <rect x="7" y="25" width="6" height="20" fill="#855a30" rx="1" />
    <rect x="5" y="10" width="10" height="15" class="torch-head" rx="2" />
  </g>

  <rect x="50" y="30" width="460" height="70" fill="#161b22" opacity="0.90" rx="6" stroke="#30363d" stroke-width="1"/>
  <text x="70" y="62" class="text-title">REDSTONE COMPUTERS</text>
  <text x="70" y="85" class="text-subtitle">Sayısal Mantık ve Bilgisayar Mimarisi Pratikleri</text>
</svg>"""

readme_content = f"""# 🕹️ Minecraft Redstone Systems & Practice

<div align="center">
  {svg_banner}
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Minecraft-1.20+-red?style=for-the-badge&logo=minecraft&logoColor=white" />
  <img src="https://img.shields.io/badge/Logic-Gates-ff2200?style=for-the-badge&logo=cpu&logoColor=white" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" />
</p>

---

## 📖 Proje Hakkında

Bu depo, **Minecraft Redstone** devreleri aracılığıyla fiziksel bilgisayar mimarisini (Computer Architecture), sayısal mantık tasarımını (Digital Logic Design) ve temel donanım bileşenlerini pratik olarak anlamak için tasarlanmış bir Minecraft dünyasını barındırmaktadır. 

Redstone, Turing-bütünsel (Turing-complete) bir yapıya sahip olduğu için, modern işlemcilerin (CPU), belleklerin (RAM) ve mantık kapılarının (Logic Gates) çalışma mantığını 3 boyutlu bir ortamda somutlaştırarak öğrenmek için mükemmel bir laboratuvardır.

---

## ⚡ Donanım Bileşenleri & Mantık Kapıları Tablosu

Dünya içerisinde inşa edilen ve pratik yapılan temel mantık kapıları ve Redstone karşılıkları:

| Mantık Kapısı (Gate) | Boolean İfadesi | Minecraft Redstone Karşılığı | Görsel / Şematik Mantık |
| :---: | :---: | :---: | :--- |
| **NOT (Değil)** | $Y = \\bar{{A}}$ | Redstone Meşalesi (Torch) bloğun arkasına yerleştirilir. | Sinyali tersine çevirir. |
| **AND (Ve)** | $Y = A \\cdot B$ | İki adet sönük meşalenin birleştirilip tekrar ters çevrilmesi. | Sadece iki giriş de aktifken ($1$) çıkış verir. |
| **OR (Veya)** | $Y = A + B$ | İki ayrı kablonun tek bir Redstone hattında birleştirilmesi. | Girişlerden en az biri aktifse ($1$) çıkış verir. |
| **XOR (Özel Veya)** | $Y = A \\oplus B$ | Kapalı devre mantığı ile tasarlanmış özel Redstone köprüsü. | Girişler birbirinden farklı olduğunda ($1$ ve $0$) çıkış verir. |

---

## 🗺️ Gelişim Yol Haritası (Roadmap)

Aşağıdaki liste, temel elektrik devrelerinden tam fonksiyonel bir işlemciye (CPU) giden yoldaki gelişim aşamalarını göstermektedir:

- [x] **Faz 1: Temel Kapılar (Logic Gates)**
  - [x] NOT, AND, OR, XOR kapılarının inşası.
  - [x] Sinyal gecikmesi (Tick/Delay) ve Repeater mantığının çözülmesi.
- [ ] **Faz 2: Aritmetik İşlemler (Arithmetic Circuits)**
  - [ ] **Half Adder** (Yarım Toplayıcı) tasarımı.
  - [ ] **Full Adder** (1-Bit Tam Toplayıcı) tasarımı.
  - [ ] **4-Bit Ripple Carry Adder** (Çoklu bit toplama ünitesi).
- [ ] **Faz 3: Bellek Elemanları (Sequential Logic)**
  - [ ] **SR Latch** (Basit veri saklama hücresi).
  - [ ] **D Flip-Flop** (Saat vuruşuna -*Clock Signal*- duyarlı bellek hücresi).
  - [ ] **Register** (Çoklu bit veri depolama birimi).
- [ ] **Faz 4: İşlem Birimleri (ALU & Control)**
  - [ ] **Multiplexer (MUX)** ve Demultiplexer yapıları.
  - [ ] **ALU (Aritmetik Mantık Birimi)** - Toplama ve çıkarma yapabilen ünite.

---

## ⚙️ Dünyayı Klonlama ve Kurulum

Bu dünyayı kendi bilgisayarındaki Minecraft oyununa eklemek için aşağıdaki adımları uygulayabilirsin:

### 1. Depoyu Klonla
Terminale aşağıdaki komutu yazarak dünyayı doğrudan Minecraft kayıt dosyalarının (`saves`) içerisine `redstone` adıyla klonlayabilirsin:
