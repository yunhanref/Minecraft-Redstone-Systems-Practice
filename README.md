# 🕹️ Minecraft Redstone Systems & Practice

---

## 📖 Proje Hakkında

Bu depo, **Minecraft Redstone** devreleri aracılığıyla fiziksel bilgisayar mimarisini (Computer Architecture), sayısal mantık tasarımını (Digital Logic Design) ve temel donanım bileşenlerini pratik olarak anlamak için tasarlanmış bir Minecraft dünyasını barındırmaktadır. 

Redstone, Turing-bütünsel (Turing-complete) bir yapıya sahip olduğu için, modern işlemcilerin (CPU), belleklerin (RAM) ve mantık kapılarının (Logic Gates) çalışma mantığını 3 boyutlu bir ortamda somutlaştırarak öğrenmek için mükemmel bir laboratuvardır.

---

## 🗺️ Gelişim Yol Haritası (Roadmap)

Aşağıdaki liste, temel elektrik devrelerinden tam fonksiyonel bir işlemciye (CPU) giden yoldaki gelişim aşamalarını göstermektedir:

- [x] **Faz 0: Kurulum ve Temel Bileşenler**
  - [x] World creation
  - [x] Basic components and their usage
- [ ] **Faz 1: Temel Kapılar (Logic Gates)**
  - [ ] NOT, AND, OR, XOR kapılarının inşası.
  - [ ] Sinyal gecikmesi (Tick/Delay) ve Repeater mantığının çözülmesi.
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
