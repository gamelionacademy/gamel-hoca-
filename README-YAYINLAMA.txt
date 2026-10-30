İngilizce360 – Web sitesi yayınlama notları
===========================================

Bu klasör, yayına hazır statik web sitesidir. Sunucu, veritabanı veya kod derlemesi gerekmez.

1) Yayınlama (önerilen: Netlify, ücretsiz)
   - app.netlify.com/drop adresine git, bu klasörün tamamını sürükle-bırak.
   - Site birkaç saniyede yayına girer (ör. xxxx.netlify.app).
   - Alternatifler: Cloudflare Pages, Vercel, GitHub Pages (hepsi ücretsiz).

2) Alan adı (gamelhoca.com)
   - Netlify > Domain management > Add a domain > gamelhoca.com
   - Netlify'ın verdiği DNS kayıtlarını, alan adını aldığın yerde (Wix / GoDaddy vb.) gir:
       www  -> CNAME -> <site-adın>.netlify.app
       @    -> A     -> 75.2.60.5   (Netlify'ın gösterdiği değeri kullan)
   - SSL (https) Netlify tarafından otomatik açılır.

3) Yayından önce tamamla
   - Footer'daki "Mesafeli Satış Sözleşmesi" ve "KVKK Aydınlatma Metni" bağlantıları şu an "#".
     Bu metinleri hazırlayıp sayfa olarak ekle ve bağlantıları güncelle.
   - Analytics: her sayfada "<!-- ANALYTICS -->" satırına Google Analytics 4 ve/veya Meta Pixel kodunu yapıştır.

4) Güncelleme
   - Değişiklik sonrası klasörü yeniden Netlify'a sürükle-bırak; aynı site güncellenir.

Dosyalar
   index.html        Akademi (ana sayfa)
   kurs.html         İngilizce360 Video Kursu
   kitap-seti.html   İngilizce360 Kitap Seti (E-Kitap)
   ucretsiz.html     Ücretsiz kaynaklar
   blog*.html        Blog
   404.html          Bulunamadı sayfası
   img/              Görseller (og.jpg = paylaşım önizlemesi)
   favicon.svg, robots.txt, sitemap.xml
