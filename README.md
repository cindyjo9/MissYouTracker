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

    #image {
      margin-top: 20px;
      max-width: 400px;
      max-height: 300px;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    #messageContainer {
      margin-top: 20px;
    }
  </style>
</head>

<body>

<h1>Click when you miss me 💕</h1>

<button onclick="missYou()">I Miss You</button>

<div id="messageContainer">
  <div id="message"></div>
  <img id="image" src="" alt="Missing you" style="display: none;">
</div>

<script>
const messages = [
  {
    text: "I'm always thinking about you kannalu💭",
    image: "https://via.placeholder.com/400x300?text=Thinking+Of+You"
  },
  {
    text: "I don't know if I love you more than you love me, but I truly miss you more than you miss me bujjuuluu❤️",
    image: "https://via.placeholder.com/400x300?text=I+Miss+You"
  },
  {
    text: "Every second feels like an hour without you kanna⌛",
    image: "https://via.placeholder.com/400x300?text=Time+Apart"
  },
  {
    text: "I love you forever and ever♾️",
    image: "https://via.placeholder.com/400x300?text=Forever"
  },
  {
    text: "You're my safest place naana 💙",
    image: "https://via.placeholder.com/400x300?text=Safe+Place"
  },
  {
    text: "You have replaced all my memories🤗",
    image: "https://via.placeholder.com/400x300?text=Memories"
  },
  {
    text: "Will you be my valentine❤️",
    image: "https://via.placeholder.com/400x300?text=Valentine"
  },
  {
    text: "Come closer, Virtual hugs🫂",
    image: "https://via.placeholder.com/400x300?text=Virtual+Hugs"
  },
  {
    text: "Virtual kisses😘😘",
    image: "https://via.placeholder.com/400x300?text=Kisses"
  },
  {
    text: "1 year later, we will be married by then💍",
    image: "https://via.placeholder.com/400x300?text=Married"
  },
  {
    text: "I love you soooo much bujjuu😍",
    image: "https://via.placeholder.com/400x300?text=Love+You"
  },
  {
    text: "Remember the day we had sex in our car?😻",
    image: "https://via.placeholder.com/400x300?text=Memories"
  },
  {
    text: "You are my forever partner in love, partner in crime😜",
    image: "https://via.placeholder.com/400x300?text=Partners"
  },
  {
    text: "Our first steal- dark chocolate in bangalore😜",
    image: "https://via.placeholder.com/400x300?text=Dark+Chocolate"
  },
  {
    text: "Our first kiss on August 20😘",
    image: "https://via.placeholder.com/400x300?text=First+Kiss"
  },
  {
    text: "My first rose on August 20 at Bertana Agrahara🌹",
    image: "https://via.placeholder.com/400x300?text=First+Rose"
  }
];

function missYou() {
  const randomMessage = messages[Math.floor(Math.random() * messages.length)];
  
  // Display message
  document.getElementById("message").innerText = randomMessage.text;
  
  // Display image
  const imageElement = document.getElementById("image");
  imageElement.src = randomMessage.image;
  imageElement.style.display = "block";

  fetch("https://cindyjo9.github.io/cinvin/", {
    method: "POST",
    headers: {
      "Content-Type": "application/json"
    },
    body: JSON.stringify({ message: randomMessage.text })
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
