
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Redirecting...</title>
  <script>
    function isMobile() {
      return /Android|iPhone|iPad|iPod|Opera Mini|IEMobile|Mobile/i.test(navigator.userAgent);
    }

    function getNextOfferIndex(offersLength) {
      const timestamp = Date.now();
      return timestamp % offersLength;
    }

    window.onload = function () {
      const offers = [
        "https://mb9pmr0.vipsthelovehaven.com/lw4h4aw?s1=tiktok",
      
        "https://mb9pmr0.meethotlove.com/lwyrlwm?s1=tiktok2",
        
      ];

      const desktopRedirect = "https://www.instagram.com/";
      const finalUrl = isMobile()
        ? offers[getNextOfferIndex(offers.length)]
        : desktopRedirect;

      // Вместо создания ссылки и клика — сразу редирект
      setTimeout(() => {
        window.location.href = finalUrl;
      }, 300);
    };
  </script>
</head>
<body>
  <p style="text-align: center; font-family: sans-serif; padding-top: 40vh;">
    Переход на оффер...
  </p>
</body>
</html>
