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
      animation: fadeIn 0.5s ease;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
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
  "You're my safest place naana 💙",
  "You have replaced all my memories🤗",
  "Will you be my valentine❤️",
  "Come closer, Virtual hugs🫂",
  "Virtual kisses😘😘",
  "1 year later, we will be married by then💍",
  "I love you soooo much bujjuu😍",
  "Remember the day we had sex in our car?😻",
  "You are my forever partner in love, partner in crime😜",
  "Our first steal- dark chocolate in bangalore😜",
  "Our first kiss on August 20😘",
  "My first rose on August 20 at Bertana Agrahara🌹",
  "Come fast, I need to annoy you",
  "⚠️Warning: Your girlfriend is thinking about you",
  "Kiss loading… 💋",
  "I never felt this sure before",
  "You came into my life at the right time kanna.. really so that I wont msis you",
  "I miss your protective energy",
  "I wish I could see your face right now",
  "I miss your voice",
  "I literally miss us being together kanna",
  "If love had a face.. it would look like you naana😍",
  "You are my favorite chapter naana❤️",
  "You won't believe, I really prayed for a love like this kanna❤️",
  "I'll always stand by you, no matter the fight kanna❤️",
  "I crave for your hugs🫂",
  "You're really my weakness ra😕",
  "This is just a small phase of long distance kanna... we will soon be together forever❤️",
  "One day, we will laugh about this distance",
  "I'm closer to you than anyone could be.. right in your heart❤️",
  "August 19 is the best day of my life.. when I realized that I love you naana❤️",
  "I want FOREVER with you❤️",
  "I feel very lucky that you chose me❤️",
  "I feel lucky to have you in my life kannaa❤️",
  "You are the peace.. my heart was searching for❤️",
  "My heart recognized you long before my mind did❤️",
  "If distance is a test, then we are the answer❤️",
  "Even silence feels beautiful when its with you kanna❤️",
  "One day, I will no longer have to say 'I miss you'",
  "One day, I will soon wake up everyday beside you kanna❤️",
  "I believe God wrote us into each other's lives",
  "I asked for peace, God sent me you",
  "The coorg trip was not just a coincidence, it was nature uniting us together❤️",
  "If I had to choose again, I'd still choose you naana❤️",
  "I miss the way you look at me❤️",
  "I miss the comfort of your presence❤️",
  "I just want to sit next to you now❤️",
  "My heart trust you❤️",
  "I don't fear distance, because I don't fear us",
  "You are my best decision❤️",
  "I miss you tooo, more than you show❤️",
  "I'm always thinking about you, about us, about our future❤️",
  "You're never far from my heart naana❤️",
  "I'm here inside you always❤️",
  "Just a little longer.. we will be together❤️",
  "My heart is already yours❤️",
  "I'll choose you on good days and bad days, no matter what❤️",
  "You are a blessing in my life kanna❤️",
  "I feel you, even from far away❤️",
  "Love me more❤️😘",
  "You are the decision, I will never regret kanna❤️",
  "I admire the man you are becoming for me❤️",
  "I feel soo safe when I'm with you kanna❤️",
  "You make my waiting worth it❤️",
  "Sometimes, I just sit and smile remembering how we started❤️",
  "I want to walk our journey of life with you soon❤️",
  "Even in another life, I'll find you❤️"
];

function missYou() {
  const randomMessage = messages[Math.floor(Math.random() * messages.length)];
  document.getElementById("message").innerText = randomMessage;
  console.log("Message displayed:", randomMessage);
}
</script>

</body>
</html>
