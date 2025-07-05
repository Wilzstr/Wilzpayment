#wilzpayment
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Pembayaran Seram - DANA & GoPay</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Creepster&display=swap');

    body {
      margin: 0;
      padding: 0;
      background: url('https://files.catbox.moe/gx5mhw.jpg') no-repeat center center fixed;
      background-size: cover;
      font-family: 'Creepster', cursive;
      color: #ff0000;
      text-shadow: 2px 2px 8px black;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
    }

    h1 {
      font-size: 4em;
      margin-bottom: 0.2em;
      animation: flicker 2s infinite alternate;
    }

    @keyframes flicker {
      0% { opacity: 1; }
      50% { opacity: 0.6; }
      100% { opacity: 1; }
    }

    .payment-box {
      background-color: rgba(0, 0, 0, 0.75);
      border: 3px solid red;
      border-radius: 10px;
      padding: 2em;
      margin-top: 1em;
      box-shadow: 0 0 25px red;
      text-align: center;
      max-width: 90%;
    }

    .payment-method {
      margin: 1.5em 0;
    }

    .payment-method h2 {
      margin-bottom: 0.2em;
    }

    .payment-method p {
      font-size: 1.5em;
      margin-bottom: 0.5em;
    }

    button {
      padding: 0.6em 1.2em;
      font-size: 1em;
      background-color: red;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      box-shadow: 0 0 10px red;
    }

    button:hover {
      background-color: darkred;
    }

    .warning {
      color: yellow;
      background-color: rgba(255, 0, 0, 0.8);
      padding: 1em;
      border-radius: 8px;
      margin-top: 2em;
      font-size: 1.2em;
      max-width: 85%;
      box-shadow: 0 0 15px black;
    }

    .footer {
      margin-top: 3em;
      font-size: 0.9em;
      color: #ccc;
      text-shadow: none;
    }
  </style>
</head>
<body>
  <h1>BAYAR ATAU...</h1>

  <div class="payment-box">
    <div class="payment-method">
      <h2>DANA</h2>
      <p>0897 5919 495</p>
      <button onclick="copyToClipboard('08975919495')">Salin Nomor DANA</button>
    </div>

    <div class="payment-method">
      <h2>GoPay</h2>
      <p>0897 5919 495</p>
      <button onclick="copyToClipboard('08975919495')">Salin Nomor GoPay</button>
    </div>
  </div>

  <div class="warning">
    ⚠️ SERTAKAN BUKTI TF KE <strong>WILZ RESULT</strong><br>
    JIKA TIDAK, DIANGGAP <u>TIDAK MASUK</u>!!
  </div>

  <div class="footer">
    <p>🩸 Jangan abaikan panggilan ini...</p>
  </div>

  <script>
    function copyToClipboard(text) {
      navigator.clipboard.writeText(text).then(() => {
        alert('Nomor berhasil disalin: ' + text);
      });
    }
  </script>
</body>
</html>
