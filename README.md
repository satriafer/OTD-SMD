<!DOCTYPE html>
<html>
<head>
    <title>OTD MONITORING</title>
</head>
<body>
    <h1>SFE305</h1>
    <div id="hasil">Memuat...</div>

    <script>
        const url = 'https://script.google.com/macros/s/AKfycbw-pINJCc6F6RByg4Y1rJrT_bD4LT1ck1vkhYqSgEe0ZCPhhBEfOoRqt8pj4Ybnz-RO/exec'; // Masukkan URL GAS Anda di sini
        fetch(url)
            .then(response => response.json())
            .then(data => {
                document.getElementById('hasil').innerText = data.pesan;
            })
            .catch(err => console.error('Gagal:', err));
    </script>
</body>
</html>
