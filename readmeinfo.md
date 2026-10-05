# 📘 Markdown Biçimlendirme Rehberi

Bu rehber, GitHub ve diğer destekleyen platformlarda **Markdown** dilini etkin bir şekilde kullanabilmeniz için hazırlanmış kapsamlı bir kılavuzdur.

> [!NOTE]
> Markdown, metinlerinizi biçimlendirip görsel olarak düzenlemenizi sağlar. Kod blokları içinde yazılan komutlar otomatik olarak çalıştırılmaz, yalnızca kod biçiminde görüntülenir.

---

## 📑 İçindekiler
- [Başlıklar](#-başlıklar)
- [Metin Biçimlendirme](#-metin-biçimlendirme)
- [Yatay Çizgi](#-yatay-çizgi)
- [Bağlantılar ve Görseller](#-bağlantılar)
- [Tablolar](#-tablolar)
- [Uyarı Kutuları (Alerts)](#-uyarı-kutuları-alerts)
- [Kod Blokları](#-kod-blokları)

---

## 🏷️ Başlıklar

Başlık oluşturmak için satırın başına `#` işareti konur. `#` sayısı arttıkça başlık seviyesi küçülür (1-6 arası).

# 1. Seviye Başlık
## 2. Seviye Başlık
### 3. Seviye Başlık
#### 4. Seviye Başlık
##### 5. Seviye Başlık
###### 6. Seviye Başlık


---

## ✍️ Metin Biçimlendirme

Metin içerisindeki önemli vurguları öne çıkarmak için aşağıdaki sözdizimleri kullanılır:

| Biçim | Markdown Sözdizimi | Önizleme |
| :--- | :--- | :--- |
| **Kalın** | `**Kalın**` veya `__Kalın__` | **Kalın** |
| *İtalik* | `*İtalik*` veya `_İtalik_` | *İtalik* |
| ~~Üstü Çizgili~~ | `~~Üstü Çizgili~~` | ~~Üstü Çizgili~~ |
| ***Kalın & İtalik*** | `***Metin***` | ***Kalın & İtalik*** |

---

## ➖ Yatay Çizgi

Sayfada bölümler arası geçiş yapmak ve görsel bir ayrım oluşturmak için üç adet tire `---` kullanılır (`<hr>` etiketine karşılık gelir).

```markdown
---
```

---

## 🔗 Bağlantılar

Web sitelerine yönlendirme yapmak için aşağıdaki yapı kullanılır:

```markdown
[Bağlantı Metni](URL)
```

**Örnek:**
- Kodu: `[GitHub](https://github.com)`
- Görünümü: [GitHub](https://github.com)

---

## 📊 Tablolar

Verileri sütunlar halinde düzenli göstermek için kullanılır. Sütun hizalamaları ikinci satırdaki `:` işaretinin konumuna göre belirlenir.

### Sözdizimi
```markdown
| Sol Sütun | Orta Sütun | Sağ Sütun |
| :--- | :---: | ---: |
| Sola Hizalı | Ortalanmış | Sağa Hizalı |
| Veri A | Veri B | Veri C |
```

### Önizleme

| Sol Sütun | Orta Sütun | Sağ Sütun |
| :--- | :---: | ---: |
| Sola Hizalı | Ortalanmış | Sağa Hizalı |
| Veri A | Veri B | Veri C |

---

## 💡 Uyarı Kutuları (Alerts)

GitHub Markdown üzerinde renklendirilmiş özel bildirim kutuları oluşturmak için `>` karakteri ile birlikte özel etiketler kullanılır.

> [!NOTE]
> **Bilgilendirme:** Genel bilgiler ve notlar için kullanılır.

> [!TIP]
> **İpucu:** Kullanışlı tavsiyeler ve pratik çözümler için önerilir.

> [!IMPORTANT]
> **Önemli:** Kullanıcının kaçırmaması gereken detaylar için tercih edilir.

> [!WARNING]
> **Uyarı:** Dikkat edilmesi gereken olası aksaklıkları belirtir.

> [!CAUTION]
> **Tehlike:** Riskli veya yıkıcı sonuçlar doğurabilecek işlemler için kullanılır.

---

## 💻 Kod Blokları

Kod parçacıklarını vurgulamak için 3 adet ters tırnak (```) kullanılır. Üstteki tırnağın yanına kod dili yazılarak sözdizimi renklendirmesi (syntax highlighting) sağlanır.

### Sık Kullanılan Dil Etiketleri
- `bash` (Terminal komutları)
- `javascript` / `typescript`
- `csharp` / `c` / `cpp`
- `python`
- `html` / `css`
- `json` / `yaml` / `xml`
- `sql`

### Sözdizimi
```markdown
```kod_tipi
Kod
```
```

### Örnekler

**C# Örneği:**
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

**Python Örneği:**
```python
print("Merhaba Dünya!")
```

**JavaScript Örneği:**
```javascript
const mesaj = "Merhaba Dünya!";
console.log(mesaj);
```

**JSON Örneği:**
```json
{
  "name": "CoreApi",
  "version": "1.0.0"
}
```