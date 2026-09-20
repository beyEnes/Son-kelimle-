# YDS/YÖKDİL Kelime Öğrenme

YDS / YÖKDİL sınavlarına hazırlananlar için tek dosyalık (`index.html`), tamamen tarayıcıda çalışan, Anki tarzı aralıklı tekrar (spaced repetition) ile çalışan bir **kelime kartı** uygulaması.

## Özellikler

- **1650 İngilizce kelime**: Her biri İngilizce kelime, Türkçe anlam ve içinde geçtiği örnek İngilizce cümle ile birlikte. Çoğu kelime için ayrıca 2-3 eş anlamlı kelime ve bir emoji bulunur.
- **Kart ekranı**: Flip animasyonlu kartlar. Kartların ~%30'unda ön yüzde kelimenin geçtiği cümle boşluk doldurma (cloze) formatında gösterilir, geri kalanında sadece kelime gösterilir. Arkada Türkçe anlam, örnek cümle (kelime kalın), varsa emoji ve eş anlamlılar yer alır.
- **Anki tarzı öğrenme algoritması**: 5 durum (Yeni → Bilmiyorum kutusu → Zorlandım kutusu → Pekiştirme → Bildiklerim). "Biliyorum" cevabı art arda 3 kez verilmeden kelime "Bildiklerim"e geçmez. Bildiklerim'e geçen kelimeler artan aralıklarla (1 → 3 → 14 gün, sonra ~2.5x katlanarak, azami 180 gün, ±%10 rastgele sapmayla) tekrar karşınıza gelir. 8 kez yanlış bilinen kelimeler "sorunlu kelime" (leech) olarak işaretlenip öne çıkarılır. Her tur, kelime durumlarına göre ağırlıklı rastgele seçimle oluşturulur.
- **İstatistik ekranı**: Genel doğruluk, toplam tekrar, gün serisi, öğrenme seviyesi dağılımı, son 7 günün aktivite grafiği, en çok yanlış bilinen kelimeler ve istatistikleri sıfırlama.
- **Kelime ekle ekranı**: `kelime - anlam | örnek cümle` formatında kendi kelimelerinizi ekleyebilirsiniz.
- **Koyu / açık tema**, sistem temasına uyumlu, kullanıcı override edebilir.
- **Kalıcılık**: Anlık yükleme için `localStorage`, gerçek kalıcılık için (Claude Artifact ortamında) kullanıcıya özel uzak veritabanı dokümanı. Bozuk/eksik yerel veriyle karşılaşıldığında güvenli şekilde varsayılana döner.

## Kullanım

`index.html` dosyasını doğrudan bir tarayıcıda açmanız yeterli. GitHub Pages ile yayınlamak için:

1. Repo ayarlarından **Settings → Pages** kısmına gidin.
2. Kaynak olarak `main` dalını ve `/ (root)` klasörünü seçin.
3. Yayınlanan adresten uygulamaya erişebilirsiniz.
