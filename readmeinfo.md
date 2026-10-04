# 📘 README.md — Markdown Kullanım Rehberi

Bu dosya, GitHub ve benzeri platformlarda kullanılan **Markdown** biçimlendirme dilini kapsamlı örneklerle açıklar. README dosyaları; projeyi tanıtmak, kurulum adımlarını anlatmak, komutları göstermek ve dosya yapısını belgelemek için kullanılır.

> [!NOTE]
> Markdown, metnin görünümünü düzenler. Kod bloklarının içine yazılan komutlar kendiliğinden çalışmaz; yalnızca gösterilir.

---

## 📑 İçindekiler

- [1. Markdown Nedir?](#1-markdown-nedir)
- [2. Başlıklar](#2-başlıklar)
- [3. Kalın, İtalik ve Üstü Çizili Yazılar](#3-kalın-italik-ve-üstü-çizili-yazılar)
- [4. Satır İçi Kod ve Kod Blokları](#4-satır-içi-kod-ve-kod-blokları)
- [5. Kod Bloğunda Dil Belirtme](#5-kod-bloğunda-dil-belirtme)
- [6. Listeler](#6-listeler)
- [7. Alıntılar ve Uyarı Kutuları](#7-alıntılar-ve-uyarı-kutuları)
- [8. Yatay Ayırıcılar](#8-yatay-ayırıcılar)
- [9. Tablolar](#9-tablolar)
- [10. Bağlantılar](#10-bağlantılar)
- [11. Görsel Ekleme](#11-görsel-ekleme)
- [12. Satır Sonları ve Paragraflar](#12-satır-sonları-ve-paragraflar)
- [13. Kaçış Karakteri](#13-kaçış-karakteri)
- [14. HTML Kullanımı](#14-html-kullanımı)
- [15. İçindekiler ve Bölüm Bağlantıları](#15-içindekiler-ve-bölüm-bağlantıları)
- [16. Rozetler](#16-rozetler)
- [17. Dosya ve Klasör Ağacı](#17-dosya-ve-klasör-ağacı)
- [18. Terminal Komutları](#18-terminal-komutları)
- [19. Açılır Bölümler](#19-açılır-bölümler)
- [20. Dipnotlar](#20-dipnotlar)
- [21. Emoji Kullanımı](#21-emoji-kullanımı)
- [22. Matematik ve Özel İçerikler](#22-matematik-ve-özel-içerikler)
- [23. Sık Kullanılan İşaretlerin Özeti](#23-sık-kullanılan-işaretlerin-özeti)
- [24. Örnek Bir Proje README Dosyası](#24-örnek-bir-proje-readme-dosyası)
- [25. İyi README Yazma Önerileri](#25-iyi-readme-yazma-önerileri)

---

## 1. Markdown Nedir?

**Markdown**, düz metin dosyalarını başlık, liste, tablo, bağlantı, görsel ve kod bloğu gibi öğelerle biçimlendirmek için kullanılan hafif bir işaretleme dilidir.

- README dosyalarının uzantısı çoğunlukla `.md` olur.
- `README.md`, GitHub depolarında proje hakkında ilk bilgi verilen dosyalardan biridir.
- Markdown kaynak dosyası düz metindir; GitHub gibi platformlar bu metni biçimlendirilmiş şekilde gösterir.
- Markdown özellikleri platforma göre küçük farklılıklar gösterebilir. GitHub, **GitHub Flavored Markdown (GFM)** adı verilen ek özellikleri de destekler.

Örnek dosya:

```text
Projem/
├── README.md
├── src/
└── tests/
```

---

## 2. Başlıklar

Başlık oluşturmak için satırın başına `#` işareti yazılır. `#` sayısı arttıkça başlığın seviyesi küçülür.

### Markdown kodu

```markdown
# Ana Başlık
## İkinci Seviye
### Üçüncü Seviye
#### Dördüncü Seviye
##### Beşinci Seviye
###### Altıncı Seviye
```

### Açıklama

- `#`: Genellikle proje adı için kullanılır.
- `##`: Kurulum, özellikler veya lisans gibi ana bölümleri gösterir.
- `###`: Bir ana bölümün alt konusunu belirtir.
- `####` ve sonrası: Daha ayrıntılı alt başlıklar oluşturur.
- `#` ile başlık metni arasında boşluk bırakmak iyi bir alışkanlıktır.

Örnek:

```markdown
# Core / Web API

## Proje Hakkında

### Kullanılan Teknolojiler

## Kurulum

### Gereksinimler

### Çalıştırma
```

**İpucu:** Başlık seviyelerini mantıklı sırada kullan. Çoğu README için tek bir `#` başlığı ve onun altında `##` bölümleri yeterlidir.

---

## 3. Kalın, İtalik ve Üstü Çizili Yazılar

Metindeki önemli kelimeleri vurgulamak için kullanılır.

| Markdown yazımı | Anlamı |
|---|---|
| `**önemli**` | **Kalın yazı** |
| `*not*` | *İtalik yazı* |
| `__önemli__` | __Kalın yazı__ |
| `_not_` | _İtalik yazı_ |
| `~~eski bilgi~~` | ~~Üstü çizili yazı~~ |
| `***vurgulu***` | ***Kalın ve italik yazı*** |

Örnek:

```markdown
Projeyi çalıştırmadan önce **.NET SDK** kurulu olmalıdır.

*Not: Komutları proje klasöründe çalıştırın.*

Bu özellik ~~eski sürümde~~ artık kullanılmıyor.
```

### Ne zaman kullanılır?

- Teknoloji adlarını veya önemli kavramları vurgulamak için kalın yazı kullan.
- Kısa notlar için italik yazı kullan.
- Artık geçerli olmayan bilgileri göstermek için üstü çizili yazı kullanılabilir; dokümantasyonda eski bilgiyi tamamen kaldırmak çoğu zaman daha temizdir.

---

## 4. Satır İçi Kod ve Kod Blokları

Kod veya komut göstermek için iki yaygın yöntem vardır. Kullanılan işaretin adı **backtick** karakteridir: `` ` ``.

### 4.1. Satır içi kod: Tek backtick

Kısa komutları, dosya adlarını, değişkenleri veya kod içindeki isimleri cümle içinde göstermek için kullanılır.

Markdown:

```markdown
Projeyi `dotnet run` komutuyla başlatın.

Ana dosya `Program.cs` dosyasıdır.

Değişkenin adı `ogrenciNo` olarak belirlenmiştir.
```

Görünümü:

Projeyi `dotnet run` komutuyla başlatın.

Ana dosya `Program.cs` dosyasıdır.

Değişkenin adı `ogrenciNo` olarak belirlenmiştir.

### 4.2. Çok satırlı kod bloğu: Üç backtick

Birden fazla satır içeren kodu ayrı bir blokta göstermek için üç backtick kullanılır. Açılış ve kapanış işaretleri ayrı satırlarda olmalıdır.

Markdown:

````markdown
```
Bu bir kod bloğudur.
Birden fazla satır yazılabilir.
```
````

Kod bloğunun içine yazılan içerik, genellikle normal Markdown biçimlendirmesi olarak yorumlanmaz. Bu nedenle kodun içindeki `#`, `*` veya `<` gibi karakterler kodun parçası olarak gösterilir.

### 4.3. Kod bloğunu kapatmayı unutma

Üç backtick ile açılan blok, başka bir üç backtick satırıyla kapatılmalıdır. Kapatılmazsa sonraki README bölümleri de kod bloğunun içindeymiş gibi görünebilir.

---

## 5. Kod Bloğunda Dil Belirtme

Açılışta kullanılan üç backtick'in hemen ardından dilin adı yazılabilir. Bu, desteklenen görüntüleyicilerde **sözdizimi renklendirmesi** sağlar.

### Bash / terminal

````markdown
```bash
dotnet restore
dotnet build
dotnet run
```
````

### C#

````markdown
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Merhaba Dünya!");
    }
}
```
````

### C

````markdown
```c
#include <stdio.h>

int main(void)
{
    printf("Merhaba Dünya!\n");
    return 0;
}
```
````

### Python

````markdown
```python
print("Merhaba Dünya!")
```
````

### JavaScript

````markdown
```javascript
const mesaj = "Merhaba Dünya!";
console.log(mesaj);
```
````

### JSON

````markdown
```json
{
  "name": "CoreApi",
  "version": "1.0.0"
}
```
````

### HTML

````markdown
```html
<h1>Merhaba Dünya!</h1>
<p>Bu bir paragraftır.</p>
```
````

### CSS

````markdown
```css
body {
    font-family: Arial, sans-serif;
}
```
````

### SQL

````markdown
```sql
SELECT Id, Name
FROM Users;
```
````

### Düz metin veya klasör ağacı

````markdown
```text
Projem/
├── src/
└── README.md
```
````

Sık kullanılan etiketler:

| Etiket | Kullanım alanı |
|---|---|
| `bash` | Bash ve birçok terminal örneği |
| `powershell` | Windows PowerShell |
| `csharp` | C# |
| `c` | C |
| `cpp` | C++ |
| `python` | Python |
| `javascript` | JavaScript |
| `typescript` | TypeScript |
| `html` | HTML |
| `css` | CSS |
| `json` | JSON |
| `sql` | SQL |
| `yaml` | YAML |
| `xml` | XML |
| `text` | Düz metin ve dosya ağacı |

Dil etiketi zorunlu değildir. Ancak doğru etiketi kullanmak kodun okunmasını kolaylaştırır. Etiket, kodu çalıştırmaz; yalnızca nasıl görüntüleneceğini belirtir.

---

## 6. Listeler

Listeler; özellikleri, gereksinimleri, kurulum adımlarını ve görevleri sıralamak için kullanılır.

### 6.1. Sırasız liste: `-`, `*`, `+`

Bu üç işaret de sırasız liste oluşturabilir.

```markdown
- C#
- ASP.NET Core
- Entity Framework Core
- SQL Server
```

Alternatif yazımlar:

```markdown
* C#
* ASP.NET Core
```

```markdown
+ C#
+ ASP.NET Core
```

Bir dosyada tutarlı olması için genellikle `-` tercih edilir.

### 6.2. Numaralı liste

```markdown
1. Depoyu klonlayın.
2. Proje klasörüne girin.
3. Bağımlılıkları yükleyin.
4. Projeyi çalıştırın.
```

Numaralı listeler özellikle sırası önemli olan işlemlerde kullanılır. Markdown görüntüleyicileri çoğu zaman numaraları otomatik olarak düzenler.

### 6.3. İç içe liste

Bir listenin alt maddesini oluşturmak için başına boşluk koyarak girinti yapılır.

```markdown
- Backend
  - Controllers
  - Services
  - Models
- Frontend
  - Components
  - Pages
```

Girinti düzeyi, hangi maddenin hangi ana maddeye bağlı olduğunu belirtir. Alt maddelerde tutarlı girinti kullan.

### 6.4. Görev listesi

GitHub, onay kutusu biçimindeki görev listelerini destekler.

```markdown
- [x] Proje oluşturuldu.
- [x] Veritabanı bağlantısı yapıldı.
- [ ] Kimlik doğrulama eklenecek.
- [ ] Testler yazılacak.
```

- `[x]`: Tamamlanan görev.
- `[ ]`: Tamamlanmamış görev.

GitHub üzerinde bu kutular bazı bağlamlarda etkileşimli olabilir. Diğer Markdown görüntüleyicilerinde yalnızca işaretli metin olarak görünebilir.

---

## 7. Alıntılar ve Uyarı Kutuları

### 7.1. Alıntı: `>`

Satırın başındaki `>` işareti alıntı görünümü oluşturur.

```markdown
> Bu bir alıntıdır.
```

Birden fazla paragraf da yazılabilir:

```markdown
> Bu proje ASP.NET Core kullanılarak geliştirilmiştir.
>
> Veriler bir veritabanında saklanabilir.
```

İç içe alıntı:

```markdown
> Ana not.
>
> > Bu, ana notun içindeki başka bir nottur.
```

### 7.2. GitHub uyarı kutuları

GitHub, belirli etiketlerle özel uyarı biçimlerini destekler:

```markdown
> [!NOTE]
> Bilgilendirme amaçlı bir not.

> [!TIP]
> Kullanışlı bir ipucu.

> [!IMPORTANT]
> Dikkat edilmesi gereken önemli bilgi.

> [!WARNING]
> Olası bir sorun hakkında uyarı.

> [!CAUTION]
> Riskli bir işlem öncesinde dikkatli olun.
```

Bu özel biçimler her Markdown görüntüleyicisinde desteklenmeyebilir. Desteklenmediklerinde normal alıntı gibi görünebilirler.

**Güvenlik örneği:**

```markdown
> [!WARNING]
> Gerçek parolaları, API anahtarlarını veya bağlantı dizelerindeki gizli bilgileri README dosyasına eklemeyin.
```

---

## 8. Yatay Ayırıcılar

`---`, `***` veya `___` tek başına bir satıra yazıldığında yatay çizgi oluşturabilir.

```markdown
## Proje Hakkında

Projenin açıklaması.

---

## Kurulum

Kurulum adımları.
```

Ayırıcı, uzun dokümanlarda bölümleri görsel olarak birbirinden ayırır. İşaretin öncesinde ve sonrasında boş satır bırakmak okunabilirliği artırır.

---

## 9. Tablolar

Tablolar verileri satır ve sütunlarda göstermek için kullanılır.

- `|` sütunları ayırır.
- Başlık satırının altındaki `---` dizisi başlıkla verileri ayırır.
- `:` karakteri sütun hizalamasını belirleyebilir.

### 9.1. Basit tablo

```markdown
| Teknoloji | Açıklama |
|---|---|
| C# | Programlama dili |
| ASP.NET Core | Web uygulamaları ve API geliştirme |
| SQL Server | İlişkisel veritabanı |
```

### 9.2. Sütun hizalama

```markdown
| Sol | Orta | Sağ |
|:---|:---:|---:|
| A | B | C |
| 10 | 20 | 30 |
```

- `:---`: Sola hizalama.
- `:---:`: Ortaya hizalama.
- `---:`: Sağa hizalama.

### 9.3. Tablo yazarken dikkat edilecekler

- Her satırda sütun ayırıcılarını tutarlı kullan.
- Hücreleri kısa ve anlaşılır tut.
- Uzun açıklamaları tablo yerine paragraf veya liste olarak yaz.
- Tablo içindeki `|` karakterini gerçek metin olarak göstermen gerekiyorsa `\\|` kullanımı bazı bağlamlarda işe yarayabilir; gerekirse hücreyi yeniden düzenleyerek tabloyu daha basit tut.

---

## 10. Bağlantılar

Bağlantı oluşturmanın genel biçimi şöyledir:

```markdown
[Görünen metin](https://example.com)
```

Köşeli parantez içindeki metin okuyucunun gördüğü bağlantı metnidir. Parantez içindeki adres bağlantının hedefidir.

### 10.1. İnternet bağlantısı

```markdown
[GitHub](https://github.com)

[.NET Dokümantasyonu](https://learn.microsoft.com/dotnet/)
```

### 10.2. Proje içindeki dosyaya bağlantı

```markdown
[Program.cs dosyası](src/Program.cs)

[Controllers klasörü](src/Controllers/)
```

Bu yollar, README dosyasının konumuna göre değerlendirilir. Dosyanın gerçekten bu yolda bulunması gerekir.

### 10.3. Aynı README içindeki bölüme bağlantı

```markdown
[Kurulum bölümüne git](#kurulum)

## Kurulum
```

GitHub, çoğu başlık için otomatik bağlantı kimliği oluşturur. Genellikle başlık küçük harfe çevrilir ve boşluklar tireye dönüşür. Özel karakterler veya aynı isimli başlıklar varsa oluşan bağlantıyı kontrol et.

### 10.4. E-posta bağlantısı

```markdown
[Destek ekibine e-posta gönder](mailto:destek@example.com)
```

Örnekteki adresi kendi gerçek destek adresinle değiştir.

---

## 11. Görsel Ekleme

Genel biçim:

```markdown
![Alternatif açıklama](gorsel-yolu)
```

Örnek:

```markdown
![Proje logosu](images/logo.png)
```

- `!`: Görsel ekleneceğini belirtir.
- `[Proje logosu]`: Görsel için alternatif açıklamadır. Görsel yüklenmediğinde yararlı olur ve erişilebilirliği destekler.
- `(images/logo.png)`: Görselin konumudur.

Örnek klasör yapısı:

```text
CoreApi/
├── README.md
└── images/
    ├── logo.png
    └── swagger.png
```

README içinde:

```markdown
# Core API

## Ekran Görüntüsü

![Swagger ekran görüntüsü](images/swagger.png)
```

Görselin görünmesi için dosyanın depoda bulunması ve yolun doğru olması gerekir. Büyük ekran görüntülerini ayrı bir `images/` veya `docs/images/` klasöründe tutmak düzen sağlar.

---

## 12. Satır Sonları ve Paragraflar

Markdown'da kaynak dosyadaki her Enter tuşu her zaman yeni bir görsel satır oluşturmaz.

### 12.1. Yeni paragraf

İki paragraf arasında boş satır bırak:

```markdown
Bu birinci paragraftır.

Bu ikinci paragraftır.
```

### 12.2. Aynı paragraf içinde satır sonu

GitHub Flavored Markdown'da satırın sonunda iki boşluk bırakmak satır sonu oluşturabilir:

```markdown
Birinci satır.  
İkinci satır.
```

Noktadan sonra iki boşluk bulunduğuna dikkat et.

### 12.3. HTML ile satır sonu

HTML desteği bulunan ortamlarda `<br>` kullanılabilir:

```markdown
Birinci satır.<br>
İkinci satır.
```

**Öneri:** Normal metinlerde paragraf ayırmak için boş satır kullan. `<br>` etiketini yalnızca gerçekten aynı paragraf içinde satır kırmak istediğinde tercih et.

---

## 13. Kaçış Karakteri

Ters eğik çizgi `\\`, bazı Markdown işaretlerinin biçimlendirme olarak yorumlanmasını önlemek için kullanılır. Bu işleme **escape (kaçış)** denir.

Örnek:

```markdown
\# Bu bir başlık değildir.

\*Bu metin italik değildir.\*

\- Bu bir liste maddesi değildir.
```

Bu örnekte işaretler biçimlendirme oluşturmak yerine düz metin olarak gösterilmeye çalışılır.

Kaçış karakteri, özellikle Markdown sözdizimini anlatan bir doküman yazarken işe yarar. Ancak her karakterin her durumda kaçırılması gerekmez; sonuç, kullanılan Markdown bağlamına göre değişebilir.

---

## 14. HTML Kullanımı

Markdown birçok temel biçimlendirmeyi destekler. Bazı platformlar Markdown içinde belirli HTML etiketlerinin kullanılmasına da izin verir.

### 14.1. Ortalanmış başlık

```html
<h1 align="center">Core / Web API</h1>

<p align="center">
  ASP.NET Core ile geliştirilmiş Web API projesi.
</p>
```

### 14.2. Genişliği belirtilmiş görsel

```html
<p align="center">
  <img
    src="images/logo.png"
    alt="Proje logosu"
    width="180"
  >
</p>
```

Bu örnekte:

- `<p>`: Paragraf alanı oluşturur.
- `align="center"`: İçeriği ortalamayı amaçlar.
- `<img>`: Görsel ekler.
- `src`: Görselin yolunu belirtir.
- `alt`: Alternatif açıklamayı belirtir.
- `width`: Görsel genişliğini ayarlar.

HTML desteği ve izin verilen etiketler platforma göre değişebilir. Taşınabilirlik için mümkün olduğunca standart Markdown kullanmak iyi bir tercihtir.

---

## 15. İçindekiler ve Bölüm Bağlantıları

Uzun README dosyalarında okuyucunun doğrudan istediği bölüme ulaşmasını sağlar.

```markdown
## İçindekiler

- [Proje Hakkında](#proje-hakkinda)
- [Kullanılan Teknolojiler](#kullanilan-teknolojiler)
- [Kurulum](#kurulum)
- [Çalıştırma](#calistirma)
- [Proje Yapısı](#proje-yapisi)
- [Lisans](#lisans)

## Proje Hakkında

...

## Kullanılan Teknolojiler

...

## Kurulum

...
```

Bağlantıların çalışması için hedef başlıkların gerçekten bulunması gerekir. Başlık adını değiştirirsen içindekiler bağlantısını da güncelle. Çok uzun olmayan README dosyalarında içindekiler bölümü zorunlu değildir.

---

## 16. Rozetler

**Rozetler (badges)**, projenin kullandığı teknolojileri, lisansını veya durumunu küçük görsellerle göstermek için kullanılır. GitHub README dosyalarında sıkça görülür.

Örnek:

```markdown
![.NET](https://img.shields.io/badge/.NET-8.0-purple)
![C%23](https://img.shields.io/badge/C%23-language-blue)
![License](https://img.shields.io/badge/License-MIT-green)
```

Rozet sağlayıcısı olarak [Shields.io](https://shields.io/) kullanılabilir.

> [!IMPORTANT]
> Rozetlerdeki sürüm, lisans ve durum bilgileri projeyle gerçekten uyumlu olmalıdır. Projede bulunmayan bir teknolojiyi veya kullanılmayan bir lisansı varmış gibi göstermeyin.

---

## 17. Dosya ve Klasör Ağacı

Proje klasörlerini ve dosyalarını göstermek için `text` etiketli bir kod bloğu kullanılabilir.

````markdown
## Proje Yapısı

```text
CoreApi/
├── Controllers/
│   └── WeatherForecastController.cs
├── Properties/
├── Program.cs
├── appsettings.json
├── CoreApi.csproj
└── README.md
```
````

Sembollerin anlamı:

- `├──`: Aynı seviyede bir öğe gösterir.
- `└──`: O seviyedeki son öğeyi gösterir.
- `│`: Üst klasörün görsel bağlantısının devam ettiğini gösterir.
- `/`: Klasör adının sonunda klasörü belirtmek için kullanılır.

Bu karakterler dosya sistemi komutları değildir; yalnızca yapıyı görsel olarak anlatırlar. Örnek ağacı kendi projenizdeki gerçek dosyalarla güncelleyin.

---

## 18. Terminal Komutları

Kurulum ve çalıştırma komutlarını README içinde kod bloğuyla göstermek, okuyucunun komutları kolayca kopyalamasını sağlar.

### 18.1. .NET CLI

````markdown
## Kurulum

Bağımlılıkları geri yükleyin:

```bash
dotnet restore
```

Projeyi derleyin:

```bash
dotnet build
```

Projeyi çalıştırın:

```bash
dotnet run
```
````

### 18.2. Git komutları

```bash
git clone https://github.com/kullanici/proje.git
cd proje
git status
```

### 18.3. Windows PowerShell örneği

````markdown
```powershell
Get-Location
Get-ChildItem
```
````

`bash` veya `powershell` etiketi yalnızca kodun türünü belirtir; komutların hangi terminalde çalıştırılacağına dikkat edilmelidir. İşletim sistemine, kurulu araçlara ve proje yapısına göre komutlar değişebilir.

---

## 19. Açılır Bölümler

GitHub gibi HTML desteği bulunan platformlarda `<details>` ve `<summary>` etiketleri, uzun açıklamaları başlangıçta kapalı tutmak için kullanılabilir.

```html
<details>
  <summary>Ek kurulum ayrıntılarını göster</summary>

  Bu bölüm açıldığında görünür.

  ```bash
  dotnet --info
  ```

</details>
```

- `<details>`: Açılıp kapanabilen alanı oluşturur.
- `<summary>`: Alan kapalıyken görünen başlığı belirtir.

Bu özellik her Markdown görüntüleyicisinde aynı şekilde çalışmayabilir. Açılır bölümün içindeki kod bloklarını kapatırken backtick sayısına dikkat et; içteki blok dıştaki Markdown bloğundan farklı bir bağlamda yazılmalıdır.

---

## 20. Dipnotlar

Dipnotlar, ana metni uzatmadan ek açıklama vermek için kullanılabilir. Dipnot desteği platforma göre değişebilir.

```markdown
Markdown, README yazımında yaygın olarak kullanılır.[^1]

[^1]: GitHub, Markdown için kendi ek özelliklerini de destekler.
```

`[^1]` metindeki dipnot referansıdır. Aynı numara veya isim, aşağıda açıklamanın yerini belirtir.

---

## 21. Emoji Kullanımı

Başlıklara veya kısa bölümlere emoji eklemek, README'yi görsel olarak daha kolay taranabilir hâle getirebilir.

```markdown
# 🚀 Core / Web API

## 📌 Proje Hakkında

## 🛠️ Kullanılan Teknolojiler

## ⚙️ Kurulum

## ▶️ Çalıştırma

## 📁 Proje Yapısı

## 📄 Lisans
```

Emoji kullanımı isteğe bağlıdır. Çok fazla emoji, özellikle kurumsal projelerde dokümanın okunmasını zorlaştırabilir. Tutarlı ve ölçülü kullanım tercih edilmelidir.

---

## 22. Matematik ve Özel İçerikler

Bazı Markdown görüntüleyicileri matematiksel ifadeleri LaTeX benzeri sözdizimiyle gösterebilir. Bu destek her platformda aynı değildir.

Örnek:

```markdown
Satır içi formül: $a^2 + b^2 = c^2$

Blok formül:

$$
a^2 + b^2 = c^2
$$
```

Markdown görüntüleyicisi matematiksel ifadeleri desteklemiyorsa dolar işaretleri ve formül metni normal yazı olarak görünebilir. README'nin temel amacı proje dokümantasyonu olduğu için formülleri yalnızca gerçekten gerekli olduğunda kullan.

---

## 23. Sık Kullanılan İşaretlerin Özeti

| İşaret / Sözdizimi | Görevi | Örnek |
|---|---|---|
| `#` | Başlık | `## Kurulum` |
| `**...**` | Kalın yazı | `**Önemli**` |
| `*...*` | İtalik yazı | `*Not*` |
| `~~...~~` | Üstü çizili yazı | `~~Eski bilgi~~` |
| `` `...` `` | Satır içi kod | `` `dotnet run` `` |
| ` ``` ` | Kod bloğu | ` ```bash ` |
| `-` | Sırasız liste | `- Özellik` |
| `1.` | Numaralı liste | `1. Kurulum` |
| `- [ ]` | Tamamlanmamış görev | `- [ ] Test yaz` |
| `- [x]` | Tamamlanmış görev | `- [x] Test yazıldı` |
| `>` | Alıntı | `> Bilgi` |
| `---` | Yatay ayırıcı | `---` |
| `\|` | Tablo sütun ayırıcı | `\| Ad \| Açıklama \|` |
| `[metin](URL)` | Bağlantı | `[GitHub](https://github.com)` |
| `![alt](yol)` | Görsel | `![Logo](images/logo.png)` |
| `\\` | Kaçış karakteri | `\#` |
| `<br>` | Satır sonu | `Birinci<br>İkinci` |
| `<details>` | Açılır bölüm | Ek açıklamaları gizleme |
| `[^1]` | Dipnot referansı | `Açıklama[^1]` |

### Hangi işareti ne zaman kullanmalısın?

- Başlık için `#`.
- Bir kelimeyi vurgulamak için `**kalın**`.
- Komut veya dosya adı için tek backtick.
- Çok satırlı kod için üç backtick.
- Kurulum adımlarını sıralamak için `1.`.
- Özellikleri sıralamak için `-`.
- Uyarı veya alıntı için `>`.
- Teknolojileri karşılaştırmak için tablo.
- Harici kaynak veya proje dosyasına gitmek için bağlantı.
- Ekran görüntüsü veya logo göstermek için görsel sözdizimi.

---

## 24. Örnek Bir Proje README Dosyası

Aşağıdaki örnek, temel Markdown özelliklerinin gerçek bir proje dokümanında nasıl bir araya getirilebileceğini gösterir. Kendi projenizdeki adları, yolları, sürümleri ve komutları kullanın.

````markdown
# 🚀 Core / Web API

**Core / Web API**, ASP.NET Core kullanılarak geliştirilen bir Web API projesidir.

> [!NOTE]
> Bu dosya projenin amacı, kurulumu, çalıştırılması ve klasör yapısı hakkında bilgi verir.

---

## 📑 İçindekiler

- [Proje Hakkında](#proje-hakkinda)
- [Kullanılan Teknolojiler](#kullanilan-teknolojiler)
- [Gereksinimler](#gereksinimler)
- [Kurulum](#kurulum)
- [Çalıştırma](#calistirma)
- [Proje Yapısı](#proje-yapisi)
- [Lisans](#lisans)

## 📌 Proje Hakkında

Bu proje, HTTP isteklerini işleyen ve istemcilere veri sağlayan bir Web API uygulamasıdır.

**Temel amaçlar:**

- API uç noktaları oluşturmak.
- İstekleri ve yanıtları yönetmek.
- Uygulama kodunu düzenli tutmak.

## 🛠️ Kullanılan Teknolojiler

| Teknoloji | Açıklama |
|---|---|
| C# | Programlama dili |
| ASP.NET Core | Web API geliştirme çatısı |
| .NET CLI | Derleme ve çalıştırma araçları |
| Visual Studio Code | Kod editörü |

## 📋 Gereksinimler

- Projenin hedeflediği sürümle uyumlu .NET SDK
- Visual Studio Code veya başka bir kod editörü
- Terminal veya komut satırı

> [!IMPORTANT]
> Kurulu .NET SDK sürümünün proje hedefiyle uyumlu olduğunu kontrol edin.

## ⚙️ Kurulum

1. Depoyu klonlayın:

   ```bash
   git clone https://github.com/kullanici/proje.git
   ```

2. Proje klasörüne girin:

   ```bash
   cd proje
   ```

3. Bağımlılıkları geri yükleyin:

   ```bash
   dotnet restore
   ```

## ▶️ Çalıştırma

Projeyi derleyin:

```bash
dotnet build
```

Projeyi başlatın:

```bash
dotnet run
```

Uygulamanın adresi ve portu, proje yapılandırmasına göre değişebilir.

## 📁 Proje Yapısı

```text
CoreApi/
├── Controllers/
├── Properties/
├── Program.cs
├── appsettings.json
├── CoreApi.csproj
└── README.md
```

| Dosya / Klasör | Açıklama |
|---|---|
| `Controllers/` | API isteklerini karşılayan controller sınıfları |
| `Properties/` | Başlatma ayarları |
| `Program.cs` | Uygulamanın başlangıç noktası |
| `appsettings.json` | Uygulama yapılandırması |
| `CoreApi.csproj` | Proje ve bağımlılık tanımları |
| `README.md` | Proje dokümantasyonu |

## 🔗 Faydalı Bağlantılar

- [.NET Dokümantasyonu](https://learn.microsoft.com/dotnet/)
- [ASP.NET Core Dokümantasyonu](https://learn.microsoft.com/aspnet/core/)
- [GitHub](https://github.com/)

## 📌 Geliştirme Durumu

- [x] Temel proje yapısı oluşturuldu.
- [ ] API uç noktaları geliştirilecek.
- [ ] Testler eklenecek.
- [ ] Dokümantasyon güncellenecek.

## 📄 Lisans

Bu bölümde projenin gerçek lisans türünü ve gerekiyorsa lisans dosyasına bağlantıyı belirtin.

---

**Geliştirici:** Geliştirici adınızı buraya yazın.
````

> [!WARNING]
> Örnekteki `kullanici/proje` adresi, dosya ağacı ve geliştirme durumu yer tutucu örneklerdir. Gerçek projenizdeki bilgilerle değiştirin. Kullanmadığınız teknolojileri, mevcut olmayan dosyaları veya sahip olmadığınız lisansları yazmayın.

---

## 25. İyi README Yazma Önerileri

1. **Kısa ve açık bir proje açıklamasıyla başla.** Okuyucu ilk birkaç satırda projenin ne yaptığını anlayabilmeli.
2. **Kurulum ve çalıştırma adımlarını ayrı bölümlere koy.** Birbirinden farklı işleri tek paragrafta karıştırma.
3. **Komutları kod bloklarında göster.** Terminal komutları için `bash`, PowerShell komutları için `powershell` kullan.
4. **Gerçek dosya yapısını göster.** Örnek ağacı projeye göre güncelle.
5. **Bağlantıları kontrol et.** Dosya yollarının ve bölüm bağlantılarının gerçekten çalıştığından emin ol.
6. **Gereksiz ayrıntılardan kaçın.** README ayrıntılı olabilir ama aynı bilgiyi tekrar tekrar yazmamalıdır.
7. **Gizli bilgileri ekleme.** Parolaları, erişim anahtarlarını, kişisel token'ları veya gizli bağlantı dizelerini paylaşma.
8. **Sürümleri doğru belirt.** Yalnızca gerçekten kullandığın .NET, Node.js, Python veya diğer sürümleri yaz.
9. **Ekran görüntülerini açıklamayla ekle.** Görselin ne gösterdiğini `alt` metninde belirt.
10. **Dosyayı düzenli güncelle.** Projenin kurulum şekli veya klasörleri değiştiğinde README'yi de güncelle.

### Sonuç

Markdown'da en çok kullanacağın yapılar başlıklar (`#`), vurgu (`**...**`), listeler (`-` ve `1.`), kod (`\`...\`` ve üç backtick), alıntılar (`>`), tablolar (`|`), bağlantılar (`[metin](URL)`) ve görsellerdir (`![alt](yol)`). Bunları doğru kullandığında GitHub'da okunabilir, düzenli ve kullanışlı bir proje dokümantasyonu hazırlayabilirsin.
