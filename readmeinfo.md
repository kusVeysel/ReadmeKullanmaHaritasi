# 📘 README.md — Markdown Kullanım Rehberi

Bu dosya, GitHub ve benzeri platformlarda kullanılan **Markdown** biçimlendirme dilini kapsamlı örneklerle açıklar.

> [!NOTE]
> Markdown, metnin görünümünü düzenler. Kod bloklarının içine yazılan komutlar kendiliğinden çalışmaz; yalnızca gösterilir.

---

## 📑 İçindekiler

- [1. Markdown Nedir?](#1-markdown-nedir)
- [2. Başlıklar](#2-başlıklar)
- [3. Kalın, İtalik ve Üstü Çizili Yazılar](#3-kalın-italik-ve-üstü-çizili-yazılar)
- [4. Listeler](#4-listeler)
- [5. Uyarı Kutuları](#5-uyarı-kutuları)
- [6. Tablolar](#6-tablolar)
- [7. Bağlantılar ve Görseller](#7-bağlantılar-ve-görseller)
- [8. Kod Blokları](#8-kod-blokları)

---

## 1. Markdown Nedir?

**Markdown**, düz metin dosyalarını başlık, liste, tablo, bağlantı, görsel ve kod bloğu gibi öğelerle biçimlendirmek için kullanılan hafif bir işaretleme dilidir.

- README dosyalarının uzantısı çoğunlukla `.md` olur.
- GitHub depolarında proje hakkında ilk bilgi verilen dosyalardan biridir.
- GitHub, **GitHub Flavored Markdown (GFM)** adı verilen ek özellikleri destekler.

---

## 2. Başlıklar

Başlık oluşturmak için satırın başına `#` işareti yazılır. İşaret sayısı arttıkça başlık seviyesi küçülür.

| Markdown Yazımı | Çıktı |
| :--- | :--- |
| `# Birinci Seviye` | <h1>Birinci Seviye</h1> |
| `## İkinci Seviye` | <h2>İkinci Seviye</h2> |
| `### Üçüncü Seviye` | <h3>Üçüncü Seviye</h3> |
| `#### Dördüncü Seviye` | <h4>Dördüncü Seviye</h4> |
| `##### Beşinci Seviye` | <h5>Beşinci Seviye</h5> |
| `###### Altıncı Seviye` | <h6>Altıncı Seviye</h6> |

---

## 3. Kalın, İtalik ve Üstü Çizili Yazılar

Metindeki önemli kelimeleri vurgulamak için kullanılır.

| Markdown Yazımı | Çıktı |
| :--- | :--- |
| `**önemli**` | **önemli** |
| `*not*` | *not* |
| `__önemli__` | __önemli__ |
| `_not_` | _not_ |
| `~~eski bilgi~~` | ~~eski bilgi~~ |
| `***vurgulu***` | ***vurgulu*** |

---

## 4. Listeler

Sıralı, sırasız, iç içe ve görev listeleri oluşturmak için kullanılır.

| Markdown Yazımı | Çıktı |
| :--- | :--- |
| `- C#`<br>`- SQL Server` | • C#<br>• SQL Server |
| `1. Depoyu klonlayın.`<br>`2. Projeyi çalıştırın.` | 1. Depoyu klonlayın.<br>2. Projeyi çalıştırın. |
| `- Backend`<br>`  - Models` | • Backend<br>&nbsp;&nbsp;&nbsp;&nbsp;• Models |
| `- [x] Tamamlandı`<br>`- [ ] Bekliyor` | ☑ Tamamlandı<br>☐ Bekliyor |

---

## 5. Uyarı Kutuları

GitHub üzerinde özel renkli bilgilendirme kutuları oluşturmak için kullanılır.

| Markdown Yazımı | Çıktı |
| :--- | :--- |
| `> [!NOTE]`<br>`> Bilgilendirme notu.` | ℹ️ **NOTE:** Bilgilendirme notu. |
| `> [!TIP]`<br>`> Kullanışlı bir ipucu.` | 💡 **TIP:** Kullanışlı bir ipucu. |
| `> [!IMPORTANT]`<br>`> Önemli bilgi.` | ❗ **IMPORTANT:** Önemli bilgi. |
| `> [!WARNING]`<br>`> Olası bir sorun uyarısı.` | ⚠️ **WARNING:** Olası bir sorun uyarısı. |
| `> [!CAUTION]`<br>`> Riskli işlem uyarısı.` | 🛑 **CAUTION:** Riskli işlem uyarısı. |

---

## 6. Tablolar

Verileri düzenli sütunlarda göstermek ve hizalamak için kullanılır.

| Markdown Yazımı | Çıktı |
| :--- | :--- |
| `\| Sol \| Orta \| Sağ \|`<br>`\|:---\|:---:\|---:\|`<br>`\| A \| B \| C \|` | <table><tr><th align="left">Sol</th><th align="center">Orta</th><th align="right">Sağ</th></tr><tr><td align="left">A</td><td align="center">B</td><td align="right">C</td></tr></table> |

---

## 7. Bağlantılar ve Görseller

Web adresleri yönlendirmek ve görsel eklemek için kullanılır.

| Markdown Yazımı | Çıktı |
| :--- | :--- |
| `[GitHub](https://github.com)` | [GitHub](https://github.com) |

---

## 8. Kod Blokları

Hazır terminal kodları.

```bash
```bash``` ile yapılır
```
