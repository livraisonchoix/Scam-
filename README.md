<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Simulation - Suivi Livraison</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #eef2f7;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .container {
      background: white;
      padding: 25px;
      border-radius: 8px;
      box-shadow: 0 0 8px rgba(0,0,0,0.1);
      text-align: center;
      width: 350px;
    }
    h2 {
      margin-bottom: 20px;
      color: #444;
    }
    input {
      width: 90%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #bbb;
      border-radius: 5px;
    }
    button {
      background: #28a745;
      color: white;
      border: none;
      padding: 10px 15px;
      cursor: pointer;
      border-radius: 5px;
      font-size: 15px;
    }
    button:hover {
      background: #218838;
    }
    .warning {
      margin-top: 20px;
      color: red;
      font-weight: bold;
      display: none;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Suivi de colis</h2>
    <form onsubmit="event.preventDefault(); showWarning();">
      <input type="text" placeholder="Numéro de suivi" required><br>
      <button type="submit">Vérifier</button>
    </form>
    <div id="warning" class="warning">
      ⚠️ Ceci est une simulation pédagogique !<br>
      Méfiez-vous des fausses pages de livraison qui demandent vos coordonnées bancaires.
    </div>
  </div>

  <script>
    function showWarning() {
      document.getElementById("warning").style.display = "block";
    }
  </script>
</body>
</html>
