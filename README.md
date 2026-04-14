# ini web sederhana yang saya buat

<html>
<head>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; margin-top: 50px; }
        #sapaan { font-size: 24px; color: #2c3e50; font-weight: bold; }
    </style>
</head>
<body>

    <div id="sapaan"></div>
    <p>Terima kasih telah berkunjung.</p>

    <script>
        const jam = new Date().getHours();
        let teks;

        if (jam < 12) {
            teks = "Selamat Pagi! 🌅";
        } else if (jam < 18) {
            teks = "Selamat Siang! ☀️";
        } else {
            teks = "Selamat Malam! 🌙";
        }

        document.getElementById("sapaan").innerText = teks + " Selamat datang di web saya.";
    </script>
</body>
</html>
