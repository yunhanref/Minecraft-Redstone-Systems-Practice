# 🕹️ Minecraft Redstone Systems & Practice

---

## 📖 Proje Hakkında

Bu depo, **Minecraft Redstone** devreleri aracılığıyla fiziksel bilgisayar mimarisini (Computer Architecture), sayısal mantık tasarımını (Digital Logic Design) ve temel donanım bileşenlerini pratik olarak anlamak için tasarlanmış bir Minecraft dünyasını barındırmaktadır. 

Redstone, Turing-bütünsel (Turing-complete) bir yapıya sahip olduğu için, modern işlemcilerin (CPU), belleklerin (RAM) ve mantık kapılarının (Logic Gates) çalışma mantığını 3 boyutlu bir ortamda somutlaştırarak öğrenmek için mükemmel bir laboratuvardır.

---

## ⚡ Donanım Bileşenleri & Mantık Kapıları Tablosu

Dünya içerisinde inşa edilen ve pratik yapılan temel mantık kapıları ve Redstone karşılıkları:

| Mantık Kapısı (Gate) | Boolean İfadesi | Minecraft Redstone Karşılığı | Görsel / Şematik Mantık |
| :---: | :---: | :---: | :--- |
| **NOT (Değil)** | Y = A' | Redstone Meşalesi (Torch) bloğun arkasına yerleştirilir. | Sinyali tersine çevirir. |
| **AND (Ve)** | Y = A . B | İki adet sönük meşalenin birleştirilip tekrar ters çevrilmesi. | Sadece iki giriş de aktifken (1) çıkış verir. |
| **OR (Veya)** | Y = A + B | İki ayrı kablonun tek bir Redstone hattında birleştirilmesi. | Girişlerden en az biri aktifse (1) çıkış verir. |
| **XOR (Özel Veya)** | Y = A ⊕ B | Kapalı devre mantığı ile tasarlanmış özel Redstone köprüsü. | Girişler birbirinden farklı olduğunda (1 ve 0) çıkış verir. |

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

## ⚙️ Dosyalar ve Çalıştırma İşlemi

Kullanılan texture pack: ["https://modrinth.com/resourcepack/mattpack?version=1.21&loader=minecraft"](mattpack)
Save sürümü: 1.21.11

### 1. Depoyu Klonla
Terminale aşağıdaki komutu yazarak dünyayı doğrudan Minecraft kayıt dosyalarının (`saves`) içerisine `redstone` adıyla klonlayabilirsin:

```bash
# Windows kullananlar için komut satırında:
cd %appdata%\.minecraft\saves

# Depoyu klonla
git clone [https://github.com/yunhanref/Minecraft-Redstone-Systems-Practice.git](https://github.com/yunhanref/Minecraft-Redstone-Systems-Practice.git) redstone
