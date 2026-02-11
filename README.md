<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<title>Happy Valentine's Day</title>
<style>
  body {
    background: #ffe6f0;
    font-family: 'Arial', sans-serif;
    text-align: center;
    padding-top: 50px;
  }

  h1 {
    color: #ff3366;
    font-size: 3em;
    animation: bounce 1s infinite alternate;
  }

  @keyframes bounce {
    from { transform: translateY(0); }
    to { transform: translateY(-20px); }
  }

  button {
    background: #ff6699;
    color: white;
    border: none;
    padding: 10px 20px;
    margin: 10px;
    font-size: 1.2em;
    cursor: pointer;
    border-radius: 10px;
    transition: transform 0.2s;
  }

  button:hover {
    transform: scale(1.2);
  }

  .hidden-letter {
    display: none;
    margin-top: 20px;
    font-size: 1.2em;
    color: #cc3366;
    animation: fadein 1s forwards;
  }

  @keyframes fadein {
    from { opacity: 0; }
    to { opacity: 1; }
  }
</style>
</head>
<body>

<h1>Happy Valentine's Day! 💖</h1>
<button onclick="playMusic()">🎵 เปิดเพลง</button>
<button onclick="showLetter()">เปิดจดหมาย</button>

<div id="letter" class="hidden-letter">
  💌 กลับมาคุยได้ไหม 🥹 
</div>

<audio id="music" src="เพลง.mp3"></audio>

<script>
function playMusic() {
  const music = document.getElementById('music');
  music.play();
}

function showLetter() {
  document.getElementById('letter').style.display = 'block';
}
</script>

</body>
</html>
