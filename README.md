# mc-multiplier
Coin A, Coin B’nin market cap’ine (veya FDV’sine) ulaşırsa kaç kat ve yeni fiyat ne olur? Tek dosyalık HTML/JS hesaplayıcı (MC/FDV, senaryolar, CSV).
# Market Cap Çarpan Hesaplayıcı (Coin A → Coin B)

**Ne yapar?**  
Coin **A**’nın, Coin **B**’nin **piyasa değerine (market cap)** veya **FDV’sine** ulaşması halinde **kaç kat** olacağını ve **yeni fiyatını** hesaplar.  
Ayrıca kendi belirlediğiniz **senaryo market cap** değerleri için çarpan ve hedef fiyat tablosu üretir (**CSV indir** destekli).

**Canlı demo:** `https://mhmtysrkoca.github.io/mc-multiplier/`

---

## Özellikler
- **Girdi türü seçimi:**  
  - **A (mevcut):** Market cap **veya** Fiyat + Dolaşımdaki Arz (opsiyonel: Maks arz → FDV).  
  - **B (hedef):** Market cap **veya** Fiyat + Arz (FDV seçeneği var).
- **Çıktılar:**  
  - **Çarpan (B/A), % değişim, A için hedef fiyat** (arz sabit varsayımı).  
  - **Senaryolar:** 100M, 1B, 10B, 50B gibi değerleri gir; tablo ve **CSV** oluştur.
- **Grafik:** A ve B market cap karşılaştırma grafiği.
- **Tek dosya:** Sadece `index.html` – GitHub Pages ile anında host edilir.

---

## Kullanım
1. **Mevcut (A)** için market cap **ya da** fiyat+arz gir.  
2. **Hedef (B)** için market cap **ya da** fiyat+arz gir (FDV istiyorsan “FDV kullan” seç).  
3. **Hesapla**’ya bas → çarpan, % değişim ve hedef fiyatı gör.  
4. Alt kısımdaki **Senaryolar** alanına (ör. `100000000, 1000000000, 10000000000`) değerleri yaz → tablo ve **CSV indir**.

> **Formül:** Çarpan = Hedef MC / Mevcut MC  
> **Yeni Fiyat (A)** ≈ Mevcut Fiyat × Çarpan (arz sabit varsayımı)  
> Fiyat bilinmiyorsa: Yeni Fiyat ≈ Hedef MC / Mevcut Arz  
> **FDV** için MC yerine **Fiyat × Maks Arz** kullanılır.

---

## Notlar
- Bu araç veri çekmez; girilen rakamlarla çalışır.  
- Para birimi yalnızca **gösterim formatıdır** (USD/EUR/TRY seçimi dönüşüm yapmaz).  
- **Yasal uyarı:** Bu bir yatırım tavsiyesi değildir; eğitim amaçlıdır.

---

## Lisans
MIT (isterseniz `LICENSE` dosyası ekleyin).
