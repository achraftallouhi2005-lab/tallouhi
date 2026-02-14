<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine 💌</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: Arial, sans-serif;
    }

    .card {
      background: white;
      padding: 30px 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
    }

    h1 {
      color: #ff4d6d;
      margin-bottom: 25px;
    }

    .buttons {
      position: relative;
      height: 60px;
    }

    button {
      padding: 10px 25px;
      border: none;
      border-radius: 20px;
      font-size: 16px;
      cursor: pointer;
    }

    #yes {
      background-color: #ff4d6d;
      color: white;
      margin-right: 10px;
    }

    #no {
      position: absolute;
      background-color: #ccc;
      color: black;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Will you be my Valentine, Yassmine? 💖</h1>
    <div class="buttons">
      <button id="yes" onclick="yesClick()">Yes 💘</button>
      <button id="no" onmouseover="moveNo()">No 💔</button>
    </div>
  </div>

  <script>
    function moveNo() {
      const noBtn = document.getElementById("no");
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 100 - 50;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    }

    function yesClick() {
      document.body.innerHTML = `
        <div style="
          height:100vh;
          display:flex;
          flex-direction:column;
          justify-content:center;
          align-items:center;
          background:linear-gradient(135deg, #ff9a9e, #fad0c4);
          font-family: Arial, sans-serif;
        ">
          <h1 style="color:white; font-size:40px; margin-bottom:20px;">
            Yaay I knew it 😍
          </h1>

          <img 
            src="file:///C:/Users/achraf/Downloads/WhatsApp%20Image%202025-03-29%20%C3%A0%2007.19.47_2c458920.jpg"
            alt="valentine photo"
            style="
              width:260px;
              border-radius:20px;
              box-shadow:0 10px 25px rgba(0,0,0,0.3);
            "
          />
        </div>
      `;
    }
  </script>

</body>
</html>
