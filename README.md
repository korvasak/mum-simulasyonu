# mum-simulasyonu
This project offers a candle simulation for studying or reading a book. The burning time of the candle is chosen randomly and users can continue their work without knowing this time.
<!DOCTYPE html>
<html>
<head>
  <title>Mum Simülasyonu</title>
</head>
<body>
  <div id="mum"></div>

  <script>
    // Mumun bitme süresini rastgele belirleme
    var bitmeSuresi = Math.floor(Math.random() * (180 - 30 + 1)) + 30; // 30-180 dakika arası

    function mumuYak() {
      var mumElementi = document.getElementById("mum");
      var sure = bitmeSuresi;

      // Mum azalma animasyonu
      var azalmaHizi = 1000; // 1 saniyede 1 dakika azalma
      var azalmaTimer = setInterval(function() {
        sure--;
        mumElementi.innerText = "Kalan Süre: " + sure + " dakika";

        if (sure <= 0) {
          clearInterval(azalmaTimer);
          mumElementi.innerText = "Mum Bitti";
        }
      }, azalmaHizi);
    }

    mumuYak();
  </script>
</body>
</html>
