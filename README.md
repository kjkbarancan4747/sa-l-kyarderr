
<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SağlıkYarder | Sağlık Çalışanları Yardımlaşma ve Dayanışma Derneği</title>

<meta name="description" content="SağlıkYarder - Sağlık Çalışanları Yardımlaşma ve Dayanışma Derneği. Sağlıkta birlik, yaşamda dayanışma.">

<style>
:root {
  --lacivert: #12345a;
  --kirmizi: #c7192d;
  --altin: #b78a35;
  --metin: #18324e;
  --gri: #64748b;
  --acik: #f4f7fb;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  color: var(--metin);
  background: white;
}

/* ÜST BİLGİ */

.ust-bilgi {
  background: var(--lacivert);
  color: white;
  padding: 10px 5%;
  display: flex;
  justify-content: space-between;
  gap: 15px;
  flex-wrap: wrap;
  font-size: 12px;
}

/* ÜST MENÜ */

header {
  background: white;
  box-shadow: 0 5px 22px #102d4b12;
  position: sticky;
  top: 0;
  z-index: 100;
}

.menu-alani {
  max-width: 1250px;
  margin: auto;
  padding: 14px 24px;
  display: flex;
  align-items: center;
  gap: 18px;
}

.logo-alani {
  display: flex;
  align-items: center;
  gap: 12px;
  text-decoration: none;
  min-width: 245px;
}

.logo-alani img {
  width: 70px;
  height: 70px;
  object-fit: contain;
}

.logo-yazi strong {
  display: block;
  color: var(--lacivert);
  font-size: 19px;
}

.logo-yazi small {
  display: block;
  color: var(--gri);
  font-size: 10px;
  line-height: 1.5;
  max-width: 190px;
}

nav {
  display: flex;
  align-items: center;
  gap: 3px;
  margin-left: auto;
}

nav a {
  text-decoration: none;
  color: var(--lacivert);
  font-size: 12px;
  font-weight: bold;
  padding: 13px 10px;
  border-radius: 7px;
  transition: .3s;
}

nav a:hover,
nav a.aktif {
  background: #edf3fa;
  color: var(--kirmizi);
}

.katil-butonu {
  background: var(--kirmizi);
  color: white;
  text-decoration: none;
  padding: 13px 17px;
  border-radius: 7px;
  font-size: 12px;
  font-weight: bold;
  white-space: nowrap;
}

.mobil-menu {
  display: none;
  background: var(--lacivert);
  color: white;
  border: none;
  border-radius: 7px;
  padding: 11px 15px;
  font-size: 14px;
  cursor: pointer;
}

/* ANA GÖRSEL */

.ana-alan {
  background:
    linear-gradient(110deg, #102f54f5, #143d68e8);
  color: white;
  overflow: hidden;
}

.ana-icerik {
  max-width: 1200px;
  margin: auto;
  padding: 75px 24px;
  display: grid;
  grid-template-columns: 1.2fr .8fr;
  gap: 50px;
  align-items: center;
}

.ust-baslik {
  color: #f0c66e;
  font-weight: bold;
  font-size: 13px;
  letter-spacing: 2px;
}

.ana-icerik h1 {
  font-size: clamp(35px, 5vw, 58px);
  line-height: 1.1;
  margin: 20px 0;
}

.ana-icerik p {
  color: #e1eaf4;
  font-size: 17px;
  line-height: 1.8;
  max-width: 620px;
}

.butonlar {
  display: flex;
  gap: 12px;
  margin-top: 28px;
  flex-wrap: wrap;
}

.buton {
  display: inline-block;
  padding: 15px 20px;
  border-radius: 7px;
  text-decoration: none;
  font-size: 13px;
  font-weight: bold;
  transition: .3s;
}

.buton-kirmizi {
  background: var(--kirmizi);
  color: white;
}

.buton-beyaz {
  border: 1px solid #ffffff80;
  color: white;
}

.buton:hover {
  transform: translateY(-3px);
}

.ana-logo {
  background: white;
  border-radius: 20px;
  padding: 12px;
  max-width: 350px;
  width: 100%;
  justify-self: center;
  box-shadow: 0 20px 50px #071b3480;
}

.ana-logo img {
  width: 100%;
  display: block;
  border-radius: 12px;
}

/* GENEL BÖLÜMLER */

.bolum {
  max-width: 1200px;
  margin: auto;
  padding: 70px 24px;
}

.bolum-baslik {
  text-align: center;
  max-width: 700px;
  margin: 0 auto 38px;
}

.bolum-baslik span {
  color: var(--kirmizi);
  font-size: 12px;
  font-weight: bold;
  letter-spacing: 2px;
}

.bolum-baslik h2 {
  font-size: 33px;
  color: var(--lacivert);
  margin: 12px 0;
}

.bolum-baslik p {
  color: var(--gri);
  line-height: 1.7;
}

/* KARTLAR */

.kartlar {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.kart {
  border: 1px solid #e5ebf2;
  border-radius: 14px;
  padding: 27px;
  background: white;
  box-shadow: 0 10px 28px #17365309;
  transition: .3s;
}

.kart:hover {
  transform: translateY(-6px);
  box-shadow: 0 15px 35px #17365318;
}

.kart-ikon {
  width: 48px;
  height: 48px;
  border-radius: 12px;
  background: #eef3f9;
  color: var(--lacivert);
  display: grid;
  place-items: center;
  font-size: 25px;
}

.kart h3 {
  color: var(--lacivert);
  margin: 18px 0 10px;
  font-size: 19px;
}

.kart p {
  color: var(--gri);
  font-size: 14px;
  line-height: 1.7;
}

.kart a {
  display: inline-block;
  color: var(--kirmizi);
  text-decoration: none;
  font-weight: bold;
  font-size: 12px;
  margin-top: 18px;
}

/* PROJELER */

.acik-bolum {
  background: var(--acik);
}

/* DEĞERLER */

.degerler {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 15px;
}

.deger {
  background: white;
  padding: 25px 12px;
  border-radius: 12px;
  text-align: center;
}

.deger strong {
  display: block;
  font-size: 25px;
  color: var(--kirmizi);
  margin-bottom: 8px;
}

.deger span {
  color: var(--gri);
  font-size: 12px;
  font-weight: bold;
}

/* ALT BİLGİ */

footer {
  background: #102d4d;
  color: #d9e4ef;
  padding: 45px 24px;
}

.alt-icerik {
  max-width: 1200px;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 25px;
}

.alt-logo {
  display: flex;
  align-items: center;
  gap: 15px;
}

.alt-logo img {
  width: 65px;
  height: 65px;
  object-fit: contain;
  background: white;
  border-radius: 8px;
  padding: 3px;
}

.alt-logo strong {
  display: block;
}

.alt-logo small,
.telif {
  color: #aebfd0;
  font-size: 12px;
  line-height: 1.6;
}

/* MOBİL UYUMLULUK */

@media(max-width: 1050px) {

  .menu-alani {
    flex-wrap: wrap;
  }

  .mobil-menu {
    display: block;
    margin-left: auto;
  }

  nav {
    display: none;
    order: 3;
    width: 100%;
    margin: 0;
    flex-direction: column;
    align-items: stretch;
  }

  nav.acik {
    display: flex;
  }

  nav a {
    padding: 14px;
  }

  .katil-butonu {
    display: none;
  }

  .ana-icerik {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .ana-icerik p {
    margin: auto;
  }

  .butonlar {
    justify-content: center;
  }

  .ana-logo {
    max-width: 280px;
  }

  .kartlar {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media(max-width: 600px) {

  .ust-bilgi {
    justify-content: center;
    text-align: center;
  }

  .logo-alani {
    min-width: 0;
  }

  .logo-alani img {
    width: 55px;
    height: 55px;
  }

  .logo-yazi strong {
    font-size: 16px;
  }

  .logo-yazi small {
    font-size: 9px;
  }

  .kartlar {
    grid-template-columns: 1fr;
  }

  .degerler {
    grid-template-columns: repeat(2, 1fr);
  }

  .bolum {
    padding: 50px 18px;
  }

  .bolum-baslik h2 {
    font-size: 27px;
  }

  .alt-icerik {
    flex-direction: column;
    align-items: flex-start;
  }

}

</style>
</head>

<body>

<!-- ÜST BİLGİ -->

<div class="ust-bilgi">
  <span>Sağlık çalışanları için dayanışma ve ortak güç</span>
  <span>Birlikte daha güçlü, birlikte daha umutlu</span>
</div>

<!-- MENÜ -->

<header>
<div class="menu-alani">

  <a href="#anasayfa" class="logo-alani">
    <img src="assets/saglikyarder-logo.jpg" alt="SağlıkYarder Logosu">

    <span class="logo-yazi">
      <strong>SAĞLIKYARDER</strong>
      <small>Sağlık Çalışanları Yardımlaşma ve Dayanışma Derneği</small>
    </span>
  </a>

  <button class="mobil-menu" onclick="menuAc()">
    MENÜ ☰
  </button>

  <nav id="navigasyon">

    <a href="#anasayfa" class="aktif">ANASAYFA</a>
    <a href="#kurumsal">KURUMSAL</a>
    <a href="#subeler">ŞUBELERİMİZ</a>
    <a href="#multimedya">MULTİMEDYA</a>
    <a href="#projeler">PROJELER</a>
    <a href="#hizmetler">HİZMETLERİMİZ</a>

  </nav>

  <a href="#iletisim" class="katil-butonu">
    BİZE KATILIN
  </a>

</div>
</header>

<!-- ANA SAYFA -->

<main>

<section class="ana-alan" id="anasayfa">

  <div class="ana-icerik">

    <div>

      <div class="ust-baslik">
        SAĞLIKTA BİRLİK, YAŞAMDA DAYANIŞMA
      </div>

      <h1>
        Sağlık çalışanları için güçlü bir dayanışma.
      </h1>

      <p>
        Sağlık çalışanlarının birlikteliğini güçlendirmek,
        yardımlaşma kültürünü büyütmek ve ortak ihtiyaçlara
        birlikte çözümler üretmek için buradayız.
      </p>

      <div class="butonlar">

        <a href="#kurumsal" class="buton buton-kirmizi">
          DERNEĞİMİZİ TANIYIN
        </a>

        <a href="#projeler" class="buton buton-beyaz">
          PROJELERİMİZİ KEŞFEDİN
        </a>

      </div>

    </div>

    <div class="ana-logo">
      <img src="assets/saglikyarder-logo.jpg" alt="SağlıkYarder Dernek Logosu">
    </div>

  </div>

</section>

<!-- KURUMSAL -->

<section class="bolum" id="kurumsal">

  <div class="bolum-baslik">

    <span>SAĞLIKYARDER</span>

    <h2>Birlikte daha güçlüyüz</h2>

    <p>
      Dayanışmayı büyüten, sağlık çalışanlarının sesi olan
      ve toplumsal faydayı önceleyen bir dernek anlayışı.
    </p>

  </div>

  <div class="kartlar">

    <article class="kart">

      <div class="kart-ikon">✚</div>

      <h3>Kurumsal Yapımız</h3>

      <p>
        Derneğimizin kuruluş amacı, ilkeleri, yönetim yapısı
        ve çalışma anlayışı hakkında bilgi edinin.
      </p>

      <a href="#kurumsal">KURUMSAL BİLGİLER →</a>

    </article>

    <article class="kart" id="subeler">

      <div class="kart-ikon">⌖</div>

      <h3>Şubelerimiz</h3>

      <p>
        Şube ve temsilciliklerimiz aracılığıyla
        dayanışma ağımızı yakından tanıyın.
      </p>

      <a href="#subeler">ŞUBELERİ GÖRÜNTÜLE →</a>

    </article>

    <article class="kart" id="hizmetler">

      <div class="kart-ikon">♡</div>

      <h3>Hizmetlerimiz</h3>

      <p>
        Üyelerimize yönelik destek, bilgilendirme,
        eğitim ve sosyal dayanışma çalışmalarımız.
      </p>

      <a href="#hizmetler">HİZMETLERİMİZİ İNCELEYİN →</a>

    </article>

  </div>

</section>

<!-- PROJELER VE MULTİMEDYA -->

<section class="acik-bolum">

<div class="bolum">

  <div class="bolum-baslik">

    <span>ÇALIŞMALARIMIZ</span>

    <h2>Dayanışmayı projelerle büyütüyoruz</h2>

    <p>
      Ortak hedeflerimiz için geliştirdiğimiz çalışmalar
      ve faaliyetler.
    </p>

  </div>

  <div class="kartlar">

    <article class="kart" id="projeler">

      <div class="kart-ikon">✦</div>

      <h3>Projeler</h3>

      <p>
        Sağlık çalışanlarının yaşamına değer katmayı
        hedefleyen projelerimizi keşfedin.
      </p>

      <a href="#projeler">TÜM PROJELER →</a>

    </article>

    <article class="kart" id="multimedya">

      <div class="kart-ikon">▣</div>

      <h3>Multimedya</h3>

      <p>
        Etkinliklerimizden fotoğraflar, videolar ve
        dernek faaliyetlerinden görüntüler.
      </p>

      <a href="#multimedya">GALERİYE GİT →</a>

    </article>

    <article class="kart">

      <div class="kart-ikon">▤</div>

      <h3>Haberler ve Duyurular</h3>

      <p>
        Derneğimizden güncel haberleri, açıklamaları
        ve önemli duyuruları takip edin.
      </p>

      <a href="#iletisim">DUYURULARI GÖR →</a>

    </article>

  </div>

</div>

</section>

<!-- DEĞERLERİMİZ -->

<section class="bolum">

  <div class="bolum-baslik">

    <span>ORTAK DEĞERLERİMİZ</span>

    <h2>Dayanışmanın gücü, birlikteliğimizden gelir</h2>

  </div>

  <div class="degerler">

    <div class="deger">
      <strong>Birlik</strong>
      <span>Ortak hedefler</span>
    </div>

    <div class="deger">
      <strong>Destek</strong>
      <span>Karşılıklı yardımlaşma</span>
    </div>

    <div class="deger">
      <strong>Güven</strong>
      <span>Şeffaf ve güçlü iletişim</span>
    </div>

    <div class="deger">
      <strong>Gelecek</strong>
      <span>Sürdürülebilir dayanışma</span>
    </div>

  </div>

</section>

</main>

<!-- ALT BİLGİ -->

<footer id="iletisim">

  <div class="alt-icerik">

    <div class="alt-logo">

      <img src="assets/saglikyarder-logo.jpg" alt="SağlıkYarder Logosu">

      <div>
        <strong>SAĞLIKYARDER</strong>

        <small>
          Sağlık Çalışanları Yardımlaşma ve Dayanışma Derneği
        </small>
      </div>

    </div>

    <div class="telif">
      © 2026 SağlıkYarder · Tüm hakları saklıdır.
    </div>

  </div>

</footer>

<!-- MOBİL MENÜ KODU -->

<script>

function menuAc() {

  const menu = document.getElementById("navigasyon");

  menu.classList.toggle("acik");

}

// Menüye tıklanınca mobil menüyü kapat

document.querySelectorAll("#navigasyon a").forEach(function(link) {

  link.addEventListener("click", function() {

    document.getElementById("navigasyon").classList.remove("acik");

  });

});

</script>

</body>
</html>
