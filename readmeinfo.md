# README Markdown Rehberi

Bu belge, bir GitHub / GitLab **README.md** dosyasında kullanabileceğiniz tüm temel ve kullanışlı Markdown sözdizimlerini (syntax) ve ne işe yaradıklarını gösterir.

---

## 1. Başlıklar (Headers)
Satır başına `#` koyarak başlık boyutu belirlenir. Toplam 6 seviye vardır.

# Başlık 1 (`# Başlık 1`)
## Başlık 2 (`## Başlık 2`)
### Başlık 3 (`### Başlık 3`)
#### Başlık 4 (`#### Başlık 4`)
##### Başlık 5 (`#### Başlık 5`)
###### Başlık 6 (`#### Başlık 6`)

---

## 2. Metin Biçimlendirme
Metinleri vurgulamak ve biçimlendirmek için kullanılır.

* **Kalın Metin:** `**Kalın**` veya `__Kalın__`
* *İtalik Metin:* `*İtalik*` veya `_İtalik_`
* ***Hem Kalın Hem İtalik:*** `***Metin***`
* ~~Üstü Çizili Metin:~~ `~~Üstü Çizili~~`

---

## 3. Kod Blokları ve Vurgulama

### Tek Satırlık Kod
Satır içinde bir komut, değişken veya kısa kod parçasını vurgulamak için ters tırnak (`` ` ``) kullanılır.
> Örnek: Projeyi çalıştırmak için `npm start` komutunu kullanın.

### Çok Satırlık Kod Blokları
Üç adet ters tırnak (```` ``` ````) kullanılarak yazılır. Açılış tırnaklarının yanına dil adı yazılırsa **kod renklendirmesi (syntax highlighting)** aktif olur.

#### Bash / Terminal Komutları (```` ```bash ````)
```bash
# Depoyu klonlayın
git clone [https://github.com/kullanici/proje.git](https://github.com/kullanici/proje.git)

# Bağımlılıkları yükleyin
cd proje
npm install