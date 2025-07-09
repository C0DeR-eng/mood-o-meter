# mood-o-meter
An emotionally confused yet loyal mood tracker that speaks fluent Gen Z. Built with Python and vibes.
# ✨ Mood-o-Meter 3000 🎭

Ever felt like your mood today deserves a whole Spotify playlist or a therapy session?  
Meet Mood-o-Meter 3000 — your emotionally confused but loyal Python bot that *gets* your vibe and responds like your favorite chaotic bestie.

---

## 💡 Features
- Asks how you're feeling — sad, tired, or delusional (y'know, the usual).
- Gives you a witty, relatable, and very Gen Z response.
- Handles unknown moods with sass (and maybe a hug).
- Pure Python. Pure serotonin.

---

## 🧪 Try It
Just run:
```bash
python mood_bot.py
[Uploading mood_bot.py…]()

# under25_username: e/shruusingh

print("🌈 Mood-o-Meter 3000 🌈")
print("What's your mood today?")
print("Options: sad / tired / delulu / angry / happy / blank")

# Get user input
mood = input("Enter your mood: ").strip().lower()
print("\nAnalyzing your vibe...\n")

# Respond based on mood
if mood == "sad":
    print("💔 It's okay to cry. Even the sky does sometimes.")
elif mood == "tired":
    print("😴 You're not lazy — just mentally exhausted. Go recharge!")
elif mood == "delulu":
    print("🦄 Delulu is the solulu! You're just manifesting a dream reality.")
elif mood == "angry":
    print("😡 Breathe in. Breathe out. You're stronger than the chaos.")
elif mood == "happy":
    print("😊 Look at you glowing! Spread that joy like confetti 🎉")
elif mood == "blank":
    print("🌀 No thoughts. Head empty. Just pure peaceful vibes.")
else:
    print("🤔 Hmm... that's a new one! Try: sad / tired / delulu / angry / happy / blank")

print("\n~ Program created with mood swings by e/shruusingh 💻")

#IN HTML FORMAT

<!-- under25_username: e/shruusingh -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Mood-o-Meter 3000</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #fceabb, #f8b500);
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      transition: background 0.5s ease;
    }

    .container {
      background: #fff;
      border-radius: 20px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      padding: 30px;
      width: 90%;
      max-width: 400px;
      text-align: center;
      animation: floatIn 1s ease-out;
    }

    @keyframes floatIn {
      0% {
        transform: translateY(30px);
        opacity: 0;
      }
      100% {
        transform: translateY(0);
        opacity: 1;
      }
    }

    h1 {
      font-size: 28px;
      color: #333;
      margin-bottom: 20px;
    }

    input {
      padding: 10px 15px;
      font-size: 16px;
      width: 80%;
      border-radius: 10px;
      border: 1px solid #ccc;
      margin-bottom: 15px;
    }

    button {
      padding: 10px 20px;
      background-color: #f8b500;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #d99800;
    }

    #message {
      margin-top: 20px;
      font-size: 18px;
      font-weight: 500;
      min-height: 60px;
      transition: all 0.3s ease;
    }

    .emoji {
      font-size: 40px;
      animation: pop 0.5s ease;
    }

    @keyframes pop {
      0% { transform: scale(0.5); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }

    footer {
      margin-top: 40px;
      font-size: 14px;
      color: #444;
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>🌈 Mood-o-Meter 3000</h1>
    <input type="text" id="moodInput" placeholder="Type your mood (e.g. sad)">
    <br>
    <button onclick="checkMood()">Check My Vibe</button>
    <div id="message"></div>
  </div>

  <footer>~ created with mood swings by e/shruusingh 💻</footer>

  <script>
    function checkMood() {
      const mood = document.getElementById("moodInput").value.toLowerCase();
      const message = document.getElementById("message");
      let output = "";
      let bg = "";

      switch (mood) {
        case "sad":
          output = "💔 It's okay to cry. Even the sky does sometimes.";
          bg = "linear-gradient(135deg, #a1c4fd, #c2e9fb)";
          break;
        case "tired":
          output = "😴 You're not lazy, you're just emotionally overloaded. Rest well.";
          bg = "linear-gradient(135deg, #fbc2eb, #a6c1ee)";
          break;
        case "delulu":
          output = "🦄 Delulu is the solulu! Stay dramatic, stay iconic.";
          bg = "linear-gradient(135deg, #fddb92, #d1fdff)";
          break;
        case "angry":
          output = "😡 Breathe in, breathe out. Don’t punch your laptop.";
          bg = "linear-gradient(135deg, #ff5858, #f09819)";
          break;
        case "happy":
          output = "😊 Yay! Spread that joy like WiFi!";
          bg = "linear-gradient(135deg, #a8edea, #fed6e3)";
          break;
        case "blank":
          output = "🌀 No thoughts. Head empty. Just vibes.";
          bg = "linear-gradient(135deg, #d3cce3, #e9e4f0)";
          break;
        default:
          output = "🤔 Unknown mood. Try sad, tired, delulu, angry, happy, or blank.";
          bg = "linear-gradient(135deg, #fceabb, #f8b500)";
      }

      message.innerHTML = `<div class="emoji">${output}</div>`;
      document.body.style.background = bg;
    }
  </script>

</body>
</html>
