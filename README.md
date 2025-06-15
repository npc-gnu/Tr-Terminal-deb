- Not: Bu depo debian/ubuntu tabanlı sistemler içindir. Arch tabanlı sistemler için [buraya tıklayın](https://github.com/npc-gnu/Tr-Terminal) .

# Tr-Terminal

## Tr-Terminal Nedir?

**Tr-Terminal**, GNU/Linux terminalini *neredeyse tamamen* Türkçe kullanabilmenizi sağlayan bash betiklerinden oluşan bir projedir.

## Özellikler ve Notlar

- Bash betikleriyle yazıldığı için yalnızca `bash` kabuğunda çalışır. `fish`, `zsh` gibi alternatif kabuklarla uyumlu değildir.  
- *"Tamamen" Türkçe demek tam doğru olmaz; tüm komutlar Türkçeye çevrilmedi. Ancak düzenli olarak yeni Türkçe komutlar eklenmeye devam edecek.*
- Paket yönetimi ile ilgili komutlar yalnızca Arch tabanlı sistemlerde (örneğin: Manjaro, EndeavourOS) çalışır (`pacman` kullanır).

## Komutlar

| Türkçe Komut           | Karşılığı                     | Açıklama |
|------------------------|-------------------------------|----------|
| `durum`                | `neofetch`                    | Sistemin temel bilgilerini ASCII sanatıyla gösterir. `neofetch` yüklü olmalıdır.          |
| `hızlıdurum`           | `fastfetch`                   | `neofetch`'in daha hızlı çalışan alternatifi. `fastfetch` yüklü olmalıdır.                |
| `kaldır`               | `sudo pacman -Rs <paket>`     | Paketi ve artık kullanılmayan bağımlılıklarını kaldırır.                                  |
| `kaldır-c`             | `sudo pacman -Rns <paket>`    | Paketi, bağımlılıklarını ve yapılandırma dosyalarını kaldırır.                            |
| `kapat`                | `shutdown`                    | Sistemi kapatır. (Şimdilik `kapat now` gibi İngilizce parametrelerle kullanılmalı.)       |
| `kopyala`              | `cp`                          | Dosya veya dizinleri kopyalar.                                                            |
| `kullanıcıdeğiştir`    | `su`                          | Belirttiğiniz kullanıcıya geçiş yapar.                                                    |
| `sil`                  | `rm -rf`                      | Dosya veya dizinleri siler. (Dikkatli kullanın!)                                          |
| `süreçler`             | `htop`                        | Sistem süreçlerini izleyebilir, işlemleri sonlandırabilirsiniz.                           |
| `taşı`                 | `mv`                          | Dosya veya dizinleri taşır.                                                               |
| `yönetici`             | `sudo`                        | Komutu yönetici (root) yetkileriyle çalıştırır.                                           |
| `yükle`                | `apt install <paket>`         | Paket yüklemenizi sağlar.                                                                 |
| `kaldır`               | `apt remove <paket>`          | Paket silmenizi sağlar.                                                                   |
| `depo`                 | `apt update`                  | Depoları güncellemenizi sağlar.                                                           |
| `güncelleme`           | `apt upgrade`                 | Tüm paketlerinizi günceller.                                                              |
| `tamgüncelleme`        | `apt update && apt upgrade`   | Tüm depoları ve paketleri günceller.                                                      |

## Kurulum
### 1. Bağımlılıkları indirin:

```bash
sudo apt install git fastfetch neofetch
```

### 2. Depoyu indirin:

```bash
git clone https://github.com/npc-gnu/Tr-Terminal-deb
cd Tr-Terminal-deb
```

### 3. `indir` betiğini çalıştırın:

```bash
chmod +x indir && ./indir
```

## Lisans

Bu proje [GNU Affero General Public License v3](https://www.gnu.org/licenses/agpl-3.0.html) (AGPLv3) lisansı veya daha sonraki AGPL sürümleri ile lisanslanmıştır.
