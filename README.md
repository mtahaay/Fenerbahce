<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fenerbahçe Maç Tahmin Çizelgesi</title>
    <style>
        table {
            width: 100%;
            border-collapse: collapse;
            text-align: center;
        }
        th, td {
            border: 1px solid black;
            padding: 10px;
        }
        input {
            width: 50px;
            text-align: center;
        }
    </style>
    <script>
        function hesapla() {
            let kisiler = ["Taha", "Recep", "Yasin", "Hamim"];
            let toplamlar = [0, 0, 0, 0];

            for (let i = 1; i <= 11; i++) { // 11 maç var
                for (let j = 0; j < 4; j++) { // 4 kişi tahmin yapıyor
                    let input = document.getElementById("m" + i + "_k" + (j + 1));
                    let deger = parseInt(input.value) || 0; // Boşsa 0 kabul et
                    toplamlar[j] += deger;
                }
            }

            // Sonuçları güncelle
            for (let j = 0; j < 4; j++) {
                document.getElementById("toplam" + (j + 1)).innerText = toplamlar[j];
            }
        }
    </script>
</head>
<body>
    <h2>Fenerbahçe Maç Tahmin Çizelgesi</h2>
    <table>
        <tr>
            <th>Maç</th>
            <th>Taha</th>
            <th>Recep</th>
            <th>Yasin</th>
            <th>Hamim</th>
        </tr>
        <tr>
            <td>(ev) Fenerbahçe - Antalya</td>
            <td><input type="number" id="m1_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m1_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m1_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m1_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(ev) Fenerbahçe - Samsun</td>
            <td><input type="number" id="m2_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m2_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m2_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m2_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(d) Bodrum - Fenerbahçe</td>
            <td><input type="number" id="m3_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m3_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m3_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m3_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(ev) Fenerbahçe - Trabzon</td>
            <td><input type="number" id="m4_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m4_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m4_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m4_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(d) Sivas - Fenerbahçe</td>
            <td><input type="number" id="m5_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m5_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m5_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m5_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(ev) Fenerbahçe - Kayseri</td>
            <td><input type="number" id="m6_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m6_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m6_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m6_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(d) Antep - Fenerbahçe</td>
            <td><input type="number" id="m7_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m7_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m7_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m7_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(ev) Fenerbahçe - Beşiktaş</td>
            <td><input type="number" id="m8_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m8_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m8_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m8_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(d) Başakşehir - Fenerbahçe</td>
            <td><input type="number" id="m9_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m9_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m9_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m9_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(d) Hatay - Fenerbahçe</td>
            <td><input type="number" id="m10_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m10_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m10_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m10_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <td>(ev) Fenerbahçe - Konya</td>
            <td><input type="number" id="m11_k1" oninput="hesapla()"></td>
            <td><input type="number" id="m11_k2" oninput="hesapla()"></td>
            <td><input type="number" id="m11_k3" oninput="hesapla()"></td>
            <td><input type="number" id="m11_k4" oninput="hesapla()"></td>
        </tr>
        <tr>
            <th>Toplam</th>
            <th id="toplam1">0</th>
            <th id="toplam2">0</th>
            <th id="toplam3">0</th>
            <th id="toplam4">0</th>
        </tr>
    </table>
</body>
</html>
