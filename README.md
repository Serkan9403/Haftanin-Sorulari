# Ziraat 2025 ÜYS – Haftanın Soruları (Quiz App)

A data‑driven, single‑page quiz you can deploy on **GitHub Pages**.

## Özellikler
- Her sayfada **1 soru**
- Seçenek tıklandığında **doğru yeşil**, **yanlış kırmızı** görünür
- Test bitince **kaç doğru/yanlış** gösterilir
- **Yanlış soruları inceleme** modu
- Sorular **/data/questions.json** dosyasından yüklenir

## Kullanım (GitHub Pages)
1. Bu repo’yu oluşturun ve aşağıdaki dosyaları köke ekleyin.
2. `Settings → Pages → Source: Deploy from a branch` ve `Branch: main / root` olarak ayarlayın.
3. 30–90sn içinde sayfanız yayına alınır: `https://<kullanıcı-adı>.github.io/<repo-adı>/`

## Soru Eklemek
- `data/questions.json` dosyasını düzenleyin ve aşağıdaki şemaya uyun:

```json
[
  {
    "question": "Soru metni… (Roma rakamları dahil serbest metin)",
    "choices": ["A şıkkı", "B şıkkı", "C şıkkı", "D şıkkı", "E şıkkı"],
    "answer": 0
  }
]
```

- `answer` alanı **0=A, 1=B, 2=C, 3=D, 4=E** demektir.
- Şık sayısı 2-5 arası olabilir.

## Kısayollar
- `1..5` → Şıkları işaretler
- `←/→` → Önceki/Sonraki

---

> Not: Varsayılan olarak 10 örnek soru eklenmiştir. Kendi 78+ sorunuzun tamamını `data/questions.json` içine kopyalayabilirsiniz.
