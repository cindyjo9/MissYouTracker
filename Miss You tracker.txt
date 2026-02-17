<html>
<head>
  <title>Miss You 💙</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      text-align: center;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #ffe6f0, #ffffff);
      padding-top: 60px;
    }

    h1 {
      color: #ff4d6d;
    }

    button {
      padding: 15px 35px;
      font-size: 18px;
      border: none;
      border-radius: 12px;
      background-color: #ff4d6d;
      color: white;
      cursor: pointer;
      transition: transform 0.2s ease, background 0.3s ease;
    }

    button:hover {
      background-color: #e60039;
      transform: scale(1.05);
    }

    #message {
      margin-top: 30px;
      font-size: 22px;
      color: #444;
      min-height: 30px;
    }
  </style>
</head>

<body>

<h1>Click when you miss me 💕</h1>

<button onclick="missYou()">I Miss You</button>

<div id="message"></div>

<script>
const messages = [
  "I'm always thinking about you kannalu💭",
  "I don't know if I love you more than you love me, but I truly miss you more than you miss me bujjuuluu❤️",
  "Every second feels like an hour without you kanna⌛",
  "I love you forever and ever♾️",
  "You’re my safest place naana 💙",
  "You have replaced all my memories🤗"
  "Will you be my valentine❤️"
  "Come closer, Virtual hugs🫂"
  "Virtual kisses😘😘"
  "1 year later, we will be married by then💍"
  "I love you soooo much bujjuu😍"
  "Remember the day we had sex in our car?😻"
  "You are my forever partner in love, partner in crime😜"
  "Our first steal- dark chocolate in bangalore😜"
  "Our first kiss on August 20😘"
  "My first rose on August 20 at Bertana Agrahara🌹"
];

function missYou() {
  const randomMessage = messages[Math.floor(Math.random() * messages.length)];
  document.getElementById("message").innerText = randomMessage;

  fetch("https://cindyjo9.github.io/cinvin/", {
    method: "POST",
    headers: {
      "Content-Type": "application/json"
    },
    body: JSON.stringify({ message: randomMessage })
  })
  .then(response => {
    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`);
    }
    return response.json();
  })
  .then(data => {
    console.log('Notification sent successfully:', data);
  })
  .catch(error => {
    console.error('Error sending notification:', error);
  });
}
</script>

</body>
</html>
