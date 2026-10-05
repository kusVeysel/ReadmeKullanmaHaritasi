# 📘 README.md — Markdown Kullanım Rehberi

Bu dosya, GitHub ve benzeri platformlarda kullanılan **Markdown** biçimlendirme dilini kapsamlı örneklerle açıklar.

> [!NOTE]
> Markdown, metnin görünümünü düzenler. Kod bloklarının içine yazılan komutlar kendiliğinden çalışmaz; yalnızca gösterilir.


## hr - yatay çizgi

`---`: `<hr>` ile aynı, yatada çizgi çeker

---

## Başlıklar
Başlık oluşturmak için satırın başına `#` işareti yazılır. İşaret sayısı arttıkça başlık seviyesi küçülür(1-6).Her başlıktan sonra otomarik `---` hr atar sistem

# 1.Seviye
## 2.Seviye
### 3.Seviye
#### 4.Seviye
##### 5.Seviye
###### 6.Seviye
---

## Kalın, İtalik ve Üstü Çizili Yazılar

Metindeki önemli kelimeleri vurgulamak için kullanılır.
- `** **`: Kalın yapar.
- `__ __` Kalın yapar.
- `* *`: İtalik yapar.
- `_ _`: İtalik yapar.
- `~~ ~~`: Üstü çizgili yapar
- `*** ***`: Hem kalın hem italik yapar

Örnekler:
- `**KALIN**`: **KALIN**     
- `__KALIN__`: __KALIN__ 
- `*İtalik*`: *İtalik*
- `_İtalik_`: _İtalik_
- `~~Üstü Çizgili~~`: ~~Üstü Çizgili~~
- `***Hem Kalın hem İtalik***`: ***Hem Kalın hem İtalik***

---

## Tablolar
Verileri düzenli sütunlarda göstermek ve hizalamak için kullanılır.

Temel Yapı: 
`|Başlık1|Başlık2|` <br>
`|---|---|` <br>
`|Yazı1|Yazı2|` <br>
`|Yazı1|Yazı2|` <br>
`|Yazı1|Yazı2|` <br>

- `:`
`|:---|:---:|---:|`: Sırayla yazıyı sola ortaya ve sağa dayar 

Örnek:
`|Başlık1|Başlık2|Başlık3|` <br>
`|:---|:---:|---:|` <br>
`|A|B|C|` <br>
`|D|E|F|` <br>

|Başlık1|Başlık2|Başlık3|
|:---|:---:|---:|
|A|B|C|
|D|E|F|

---

## Uyarı Kutuları

`[!NOTE]`: ℹ️ Bilgilendirme notu
`[!TIP]`: 💡 Kullanışlı bir ipucu
`[!IMPORTANT]`: ❗ Önemli bilgi
`[!WARNING]` ⚠️ Olası bir sorun uyarısı
`[!CAUTION]`: 🛑 Riskli işlem uyarısı
`>`: ile beraber kullanılır. 

Örnekler:
> [!NOTE]
> Bilgilendirme notu

> [!TIP]
> Kullanışlı bir ipucu

> [!IMPORTANT]
> Önemli bir bilgi

> [!WARNING]
> Olası bir sorun uyarısı

> [!CAUTİON]
> Riskli işlem uyarısı

---

## Bağlantılar
Web adresleri yönlendirmek için kullanılır.

`[Metin](URL)`

Örnek:
`[GitHub](https://githup.com)`: [GitHub](https://githup.com)

## Kod Blokları

`3 tane(``) ile beraber yazılır`,3 üstte 3 alttan olacak şekilde üstteki 3 tırnaktan sonra kod tipi yazılır

- bash(terminal için)
- markdown(markdown için)
- csharp(csharp için)
- c(c için)
- python(python için)
- html(html için)
- css(css için)
- javascript(javascript için)
- json(json için)
- sql(sql için)
- text(text için)
- xml(xml için)
- yaml(yaml için)
- typescript(typescript için)
- ...

Temel Yapı:
```markdown
```tip
Yazı
```
```

Örnekler:
```bash
cd ..
```

```text
Metin
```

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

```python
print("Merhaba Dünya!")
```

```javascript
const mesaj = "Merhaba Dünya!";
console.log(mesaj);
```

```json
{
  "name": "CoreApi",
  "version": "1.0.0"
}
```