# SnapFit V5

GitHub Pages için hazır tek dosyalı PWA.

Öne çıkanlar:
- Zorunlu profil kurulumu
- Hedefe göre kalori, protein, karbonhidrat, yağ ve su hedefleri
- Öğün bazlı gram/adet/ml besin girişi
- Geniş yerel besin ve egzersiz veri tabanı
- Haftalık/aylık manuel program oluşturma
- Ev/salon ve kas grubu kategorileri
- Egzersiz detayları, set/tekrar/dinlenme/ekipman
- 100/100 günlük tamamlama barı, otomatik gün tamamlama ve seri sistemi\n- Seri, puan, rozet ve günlük skor
- Profil ve ilerleme ekranları
- JSON yedekleme/geri yükleme
- Yalnızca Türkçe arayüz

## Bu revizyonda değişenler (v6)
- **Rozetler artık açılır pencerede:** İlerleme sekmesinde 100 rozetlik ızgara varsayılan olarak kapalı; "🏆 Tüm rozetleri göster" butonuna basınca aşağı doğru açılıyor.
- **Makro toleransı gevşetildi (%10, tutarlı):** Kalori üst sınırı artık hedefin tam %10 fazlası (örn. hedef 2000 ise üst sınır 2200) — önceden hedefe göre değişen, bazen %7 gibi daha sıkı bir sınır kullanılıyordu. Yağ/karbonhidrat için de aynı %10 sınır geçerli. %100–110 arasında (tolerans içinde) artık sert kırmızı uyarı yerine sarı bir "dikkatli ol" notu çıkıyor ve seri bozulmuyor; sadece %110'u geçince sert uyarı çıkıyor ve gün otomatik tamamlanmıyor.
- **İlerleme'deki "7 günlük değişim" kaldırıldı:** Günlük kilo kaydı azsa hep "—" gösteriyordu. Yerine, doğrudan profildeki başlangıç ve güncel kilodan hesaplanan **"Verilen kilo"** geldi; her zaman doğru değer gösterir.

## Önceki revizyon
- **Program eklemede "Kaydet"e gerek yok:** Program sayfasında, ana ekrandaki "Düzenle"de ve Egzersiz kütüphanesinde bir harekete "＋ Ekle" dediğinde artık anında programa yazılıyor. Yeni program oluştururken önce gün seçiliyor, sonra eklediğin her hareket o güne otomatik kaydediliyor. Alttaki buton artık sadece "✅ Bitti" (kapat) işlevi görüyor.
- **100 parçalı rozet/seri sistemi:** Seri (en iyi seri), tamamlanan gün sayısı, toplam puan, tek günlük adım, toplam adım, kilo değişimi, tam puanlı (100/100) gün sayısı ve su hedefi tamamlama gününe göre toplam 100 rozet üretiliyor. Kazanılmayan rozetler soluk/şeffaf kupa, kazanılanlar parlayan altın kupa olarak gösteriliyor; İlerleme sekmesinde "Kazanılan X / 100" özeti var.
- **Makro aşımı uyarısı ve seri koruması:** Günlük kalori üst sınırı, yağ veya karbonhidrat hedefin %10'undan fazla aşılırsa Bugün ve Beslenme sekmelerinde kırmızı bir uyarı çıkıyor ("...fazla, besin değerlerine daha dikkat etmelisiniz"). Bu durumda puan yeterli olsa bile gün otomatik tamamlanmıyor, yani seri o gün için ilerlemiyor.
- **Günlük seri eşiği 80 puana indirildi:** Gün artık 100 değil, 80/100 puana ulaşınca (ve makro aşımı yoksa) otomatik tamamlanıyor. 100 puanlık "mükemmel gün" hâlâ ayrı rozetlerle (💯) ödüllendiriliyor.
- **İlerleme'deki "7 günlük değişim" düzeltildi:** Daha önce profil kilosu her güncellemede geçmiş veriyi eziyordu, bu yüzden değişim çoğu zaman 0 görünüyordu. Artık gerçek geçmiş kilo kayıtları kullanılıyor; yeterli veri yoksa "—" gösteriliyor.
