
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#ffe4ef">
<title>For My Kyuutu ♡</title>

<style>
:root {
  --pink:#ed78a9;
  --deep:#ad326b;
  --text:#713b53;
  --pale:#fff4f8;
}
* { box-sizing:border-box; }
html { scroll-behavior:smooth; scroll-padding-top:75px; }
body {
  margin:0;
  font-family:Georgia,"Times New Roman",serif;
  color:var(--text);
  background:
    radial-gradient(ellipse at top left,#fff 0,transparent 45%),
    radial-gradient(ellipse at right,#ffc8df 0,transparent 42%),
    linear-gradient(145deg,#fff7fb,#ffe2ee,#fff5f9);
  overflow-x:hidden;
}
button,a { -webkit-tap-highlight-color:transparent; }
button { font:inherit; }
a { color:inherit;text-decoration:none; }
nav {
  position:sticky;top:0;z-index:10;
  padding:13px 4%;
  display:flex;align-items:center;justify-content:space-between;gap:8px;
  background:#fff4f8ed;backdrop-filter:blur(14px);
  border-bottom:1px solid #ffffff;
}
.brand { color:var(--deep);font-weight:bold;font-size:1.05rem; }
.links { display:flex;gap:12px;font:11px Arial,sans-serif; }
.links a:hover { color:#e35e99; }
section { padding:65px 5%; }
.hero {
  min-height:88vh;display:flex;flex-direction:column;
  justify-content:center;align-items:center;text-align:center;
  padding-top:55px;position:relative;
}
.eyebrow {
  font:11px Arial,sans-serif;text-transform:uppercase;
  letter-spacing:3px;color:var(--deep);
}
h1 {
  font-size:clamp(3.5rem,14vw,7rem);line-height:.96;
  color:var(--deep);font-weight:normal;margin:20px 0;
}
h1 em { color:#e56da1; }
h2 {
  font-size:clamp(2rem,8vw,3.3rem);color:var(--deep);
  font-weight:normal;margin:12px 0 18px;
}
h3 { color:var(--deep); }
p { line-height:1.8; }
.subtitle { max-width:500px; }
.btn {
  border:0;border-radius:40px;padding:14px 23px;
  display:inline-block;background:linear-gradient(135deg,#f29bc0,#d64f8d);
  color:white;box-shadow:0 8px 25px #c64e8329;cursor:pointer;
  transition:transform .2s;
}
.btn:hover { transform:translateY(-3px); }
.hero-heart { font-size:4rem;animation:pulse 1.8s infinite; }
@keyframes pulse { 50% { transform:scale(1.13); } }
@keyframes floatUp {
  from { transform:translateY(0) rotate(0);opacity:0; }
  15% { opacity:.8; }
  to { transform:translateY(-110vh) rotate(45deg);opacity:0; }
}
.heart-float {
  position:fixed;bottom:-35px;z-index:1;pointer-events:none;
  color:#e36b9e;animation:floatUp linear forwards;
}
.head { text-align:center;max-width:650px;margin:0 auto 32px; }
.head p { max-width:520px;margin:0 auto; }
.card {
  background:#ffffffc9;border:1px solid white;border-radius:25px;
  padding:23px;box-shadow:0 12px 36px #a83e7117;
  backdrop-filter:blur(10px);
}
.center { text-align:center; }
.countdown {
  display:grid;grid-template-columns:repeat(4,minmax(0,1fr));
  gap:8px;max-width:560px;margin:25px auto;
}
.timebox {
  background:#fff9fc;border:1px solid #f6c9dd;
  border-radius:16px;padding:15px 3px;
}
.timebox strong {
  display:block;font-size:clamp(1.4rem,6vw,2.5rem);color:var(--deep);
}
.timebox small { font:9px Arial,sans-serif;letter-spacing:1px; }
.gallery {
  display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:13px;
}
.photo {
  min-width:0;padding:8px 8px 14px;background:white;
  border-radius:7px;box-shadow:0 8px 22px #8e3d621c;
  transform:rotate(-1deg);
}
.photo:nth-child(even) { transform:rotate(1deg); }
.photo img {
  width:100%;aspect-ratio:3/4;object-fit:cover;
  display:block;background:#ffe3ef;border-radius:4px;
}
.photo p { font-size:.88rem;text-align:center;margin:9px 2px 0; }
.note { font:12px Arial,sans-serif;text-align:center;opacity:.8; }
.letter-area { max-width:650px;margin:auto;text-align:center; }
.envelope {
  width:min(280px,90%);height:175px;border:0;border-radius:12px;
  background:#f3a2c4;cursor:pointer;margin:25px auto;
  box-shadow:0 12px 30px #a83e7120;position:relative;overflow:hidden;
}
.envelope:before {
  content:"";position:absolute;inset:0;background:#ee8bb7;
  clip-path:polygon(0 0,50% 58%,100% 0);
}
.seal { position:relative;z-index:1;font-size:3rem; }
.letter {
  display:none;background:#fffdfb;border:1px solid #f5d7e4;
  padding:clamp(20px,5vw,38px);border-radius:16px;
  text-align:left;white-space:pre-line;line-height:1.9;
}
.letter.show { display:block;animation:appear .6s ease; }
@keyframes appear {
  from { opacity:0;transform:translateY(12px); }
  to { opacity:1;transform:translateY(0); }
}
.reasons { display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px; }
.reason {
  min-height:140px;border:1px solid white;border-radius:20px;
  padding:16px 10px;background:#ffffffc7;color:var(--text);
  cursor:pointer;box-shadow:0 8px 22px #a94c7310;
}
.reason .emoji { display:block;font-size:1.8rem;margin-bottom:10px; }
.answer { display:none;font-size:.9rem;line-height:1.6; }
.reason.revealed .prompt { display:none; }
.reason.revealed .answer { display:block;animation:appear .3s; }
.music { max-width:540px;margin:auto;text-align:center; }
audio { width:100%;margin:12px 0; }
.small { font:12px Arial,sans-serif;opacity:.8; }
.gift {
  font-size:5rem;border:0;background:transparent;cursor:pointer;
  transition:transform .25s;
}
.gift:hover { transform:scale(1.1) rotate(-7deg); }
.secret-message { display:none; }
.secret-message.show { display:block;animation:appear .6s; }
footer { padding:38px 15px 50px;text-align:center;background:#ffffff68; }
footer .footer-heart { color:var(--deep);font-size:2rem; }
@media(min-width:700px) {
  section { padding:85px 9%; }
  .gallery { grid-template-columns:repeat(3,minmax(0,1fr));gap:20px; }
  .reasons { grid-template-columns:repeat(3,minmax(0,1fr)); }
}
@media(max-width:370px) {
  .links { gap:8px;font-size:10px; }
  .brand { font-size:.9rem; }
  section { padding:55px 4%; }
  .card { padding:17px; }
}
@media(prefers-reduced-motion:reduce) {
  *,*:before,*:after { animation:none!important;scroll-behavior:auto!important; }
}
</style>
</head>

<body>
<nav>
  <a class="brand" href="#home">♡ My Kyuutu</a>
  <div class="links">
    <a href="#birthday">Birthday</a>
    <a href="#memories">Photos</a>
    <a href="#letter">Letter</a>
    <a href="#surprise">Surprise</a>
  </div>
</nav>

<main>
<section class="hero" id="home">
  <p class="eyebrow">A little world made with love</p>
  <h1>For my<br><em>Kyuutu</em> ♡</h1>
  <p class="subtitle">
    To my favourite girl, Anuska. A little corner of the internet
    made just for you, filled with memories, smiles and love.
  </p>
  <div class="hero-heart">💗</div>
  <p>Made with love by Biraja Prasad Jena</p>
  <a class="btn" href="#birthday">Open your little surprise ↓</a>
  <p class="small">Scroll down, birthday girl 🌷</p>
</section>

<section id="birthday">
  <div class="head">
    <p class="eyebrow">Your special day</p>
    <h2>It's almost your day, Kyuutu 🎂</h2>
    <p>October 5 is special because the world welcomed you.</p>
  </div>
  <div class="card center">
    <p id="countLabel">Counting down to your birthday…</p>
    <div class="countdown" id="countBoxes">
      <div class="timebox"><strong id="days">--</strong><small>DAYS</small></div>
      <div class="timebox"><strong id="hours">--</strong><small>HOURS</small></div>
      <div class="timebox"><strong id="minutes">--</strong><small>MINUTES</small></div>
      <div class="timebox"><strong id="seconds">--</strong><small>SECONDS</small></div>
    </div>
    <p id="birthdayMessage">Wishing you all the happiness in the world. 💕</p>
  </div>
</section>

<section id="memories">
  <div class="head">
    <p class="eyebrow">Little moments, big feelings</p>
    <h2>Our memory corner 📸</h2>
    <p>Every picture tells a little story. Here's a collection of moments to treasure.</p>
  </div>

  <div class="gallery">
    <div class="photo">
      <img src="IMG-20260329-WA0053(1).jpg" alt="Memory one" loading="lazy">
      <p>A favourite moment ♡</p>
    </div>
    <div class="photo">
      <img src="IMG-20260404-WA0112.jpg" alt="Memory two" loading="lazy">
      <p>A little memory 🌷</p>
    </div>
    <div class="photo">
      <img src="IMG-20260501-WA0167.jpg" alt="Memory three" loading="lazy">
      <p>You make moments special ✨</p>
    </div>
    <div class="photo">
      <img src="IMG-20260527-WA0055.jpg" alt="Memory four" loading="lazy">
      <p>One for the memory book 💗</p>
    </div>
    <div class="photo">
      <img src="IMG-20260617-WA0067.jpg" alt="Memory five" loading="lazy">
      <p>Sweet little memories 🌸</p>
    </div>
    <div class="photo">
      <img src="IMG-20260617-WA0105.jpg" alt="Memory six" loading="lazy">
      <p>Another moment to keep ♡</p>
    </div>
    <div class="photo">
      <img src="IMG-20260729-WA0018.jpg" alt="Memory seven" loading="lazy">
      <p>Little things, big feelings 💕</p>
    </div>
    <div class="photo">
      <img src="IMG-20260811-WA0055.jpg" alt="Memory eight" loading="lazy">
      <p>A lovely little moment ✨</p>
    </div>
    <div class="photo">
      <img src="IMG-20260829-WA0026.jpg" alt="Memory nine" loading="lazy">
      <p>One more for us 🌷</p>
    </div>
    <div class="photo">
      <img src="IMG-20260909-WA0045.jpg" alt="Memory ten" loading="lazy">
      <p>Something to smile about 😊</p>
    </div>
    <div class="photo">
      <img src="IMG-20260917-WA0025.jpg" alt="Memory eleven" loading="lazy">
      <p>Memories worth keeping 💗</p>
    </div>
    <div class="photo">
      <img src="IMG-20260921-WA0050.jpg" alt="Memory twelve" loading="lazy">
      <p>More memories to come ♡</p>
    </div>
  </div>
  <p class="note">Twelve little spaces in our memory corner, made with love.</p>
</section>

<section id="letter">
  <div class="head">
    <p class="eyebrow">Just for you</p>
    <h2>A letter from me 💌</h2>
    <p>Tap the envelope to open something written from the heart.</p>
  </div>
  <div class="letter-area">
    <button class="envelope" id="envelope" aria-label="Open letter">
      <span class="seal">💌</span>
    </button>
    <p class="small" id="letterHint">Tap to open your letter</p>
    <article class="letter" id="letterContent">
      <h3>To my Kyuutu, Anuska ♡</h3>
Happy Birthday, my girl! 🎂💗

I may not always find the perfect words, but today I want you to know how special you are to me.

Thank you for being yourself, for your little ways, your smile, and all the moments that become beautiful simply because you're part of them. Sometimes even a small conversation with you can make an ordinary day feel different.

For your new year of life, I wish you happiness, peace, good health, courage for your dreams, and countless reasons to smile. I hope you always remember that you matter and deserve kindness, respect and beautiful things.

I don't expect every day to be perfect. I hope we continue to understand each other, speak honestly, respect each other and make lovely memories along the way.

This website is a small birthday gift, made with thought and affection, to celebrate the wonderful person you are.

Keep smiling, keep dreaming, and keep being your adorable self.

Happy Birthday once again, my Kyuutu. 🌷

With lots of love,
Your Biraja ♡
    </article>
  </div>
</section>

<section id="reasons">
  <div class="head">
    <p class="eyebrow">A few little reminders</p>
    <h2>Reasons you're special 💕</h2>
    <p>Tap every card to reveal a little reminder.</p>
  </div>
  <div class="reasons">
    <button class="reason">
      <span class="emoji">🌸</span><span class="prompt">Reason one…</span>
      <span class="answer">I appreciate the unique person you are.</span>
    </button>
    <button class="reason">
      <span class="emoji">😊</span><span class="prompt">Reason two…</span>
      <span class="answer">Your smile can make an ordinary moment feel special.</span>
    </button>
    <button class="reason">
      <span class="emoji">🫶</span><span class="prompt">Reason three…</span>
      <span class="answer">I value the trust and comfort we build by being honest.</span>
    </button>
    <button class="reason">
      <span class="emoji">✨</span><span class="prompt">Reason four…</span>
      <span class="answer">You have your own magic. You never need to be anyone else.</span>
    </button>
    <button class="reason">
      <span class="emoji">🌷</span><span class="prompt">Reason five…</span>
      <span class="answer">I love learning the little things that make you happy.</span>
    </button>
    <button class="reason">
      <span class="emoji">💗</span><span class="prompt">One last reason…</span>
      <span class="answer">Being you is already special, Kyuutu. Never forget that.</span>
    </button>
  </div>
</section>

<section id="music">
  <div class="head">
    <p class="eyebrow">A song for you</p>
    <h2>Press play, my girl 🎶</h2>
    <p>A little soundtrack for this little world.</p>
  </div>
  <div class="card music">
    <div style="font-size:3rem">🎧💗🎵</div>
    <h3>Tera Naam Doon ♡</h3>
    <audio controls loop preload="metadata">
      <source src="Tera%20Naam%20Doon%20Entertainment%20320%20Kbps.mp3" type="audio/mpeg">
      Your browser does not support audio.
    </audio>
    <p class="small">Tap play to listen to your song.</p>
  </div>
</section>

<section id="surprise">
  <div class="head">
    <p class="eyebrow">One final surprise</p>
    <h2>Something for you 🎁</h2>
    <p>Ready to open your little gift, Kyuutu?</p>
  </div>
  <div class="card center">
    <button class="gift" id="gift" aria-label="Open surprise">🎁</button>
    <p id="giftHint">Tap the gift to reveal your surprise</p>
    <div class="secret-message" id="secretMessage">
      <div style="font-size:3rem">🎉💗🎂</div>
      <h2>Happy Birthday, Anuska!</h2>
      <p>
        Today we celebrate you, your dreams, your laughter, and
        everything that makes you wonderfully yourself.
      </p>
      <p>I hope your year is filled with new beginnings, lovely memories, and reasons to smile.</p>
      <h3>You're one of a kind, Kyuutu. ♡</h3>
      <button class="btn" id="loveButton">Send a little love 💗</button>
      <p id="loveResponse" class="small"></p>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="footer-heart">♡</div>
  <p>Made especially for Anuska, my Kyuutu.</p>
  <p class="small">With love, Biraja Prasad Jena · 2026</p>
  <a class="small" href="#home">Back to the beginning ↑</a>
</footer>

<script>
/* Birthday countdown: October 5, 2026 */
const birthday = new Date(2026, 9, 5, 0, 0, 0);

function updateCountdown() {
  const now = new Date();
  const diff = birthday.getTime() - now.getTime();
  const label = document.getElementById("countLabel");
  const message = document.getElementById("birthdayMessage");
  const boxes = document.getElementById("countBoxes");

  if (now.toDateString() === birthday.toDateString()) {
    label.textContent = "It's your birthday, Kyuutu! 🎂";
    message.textContent = "Today is all about you. Happy Birthday! 💗";
    document.getElementById("days").textContent = "🎂";
    document.getElementById("hours").textContent = "💗";
    document.getElementById("minutes").textContent = "🎉";
    document.getElementById("seconds").textContent = "♡";
    return;
  }

  if (diff <= 0) {
    boxes.style.display = "none";
    label.textContent = "Your birthday celebration is here to stay 💕";
    message.textContent = "Sending you birthday wishes and love, Kyuutu!";
    return;
  }

  document.getElementById("days").textContent =
    Math.floor(diff / 86400000);
  document.getElementById("hours").textContent =
    Math.floor(diff / 3600000) % 24;
  document.getElementById("minutes").textContent =
    Math.floor(diff / 60000) % 60;
  document.getElementById("seconds").textContent =
    Math.floor(diff / 1000) % 60;
}
updateCountdown();
setInterval(updateCountdown, 1000);

/* Floating hearts */
const heartSymbols = ["♡","♥","💗","💕","✧"];
function createHeart() {
  const heart = document.createElement("span");
  heart.className = "heart-float";
  heart.textContent = heartSymbols[Math.floor(Math.random()*heartSymbols.length)];
  heart.style.left = Math.random()*100 + "vw";
  heart.style.fontSize = (12 + Math.random()*20) + "px";
  heart.style.animationDuration = (7 + Math.random()*6) + "s";
  document.body.appendChild(heart);
  setTimeout(() => heart.remove(), 14000);
}
setInterval(createHeart, 900);

/* Interactive letter */
const envelope = document.getElementById("envelope");
const letter = document.getElementById("letterContent");
envelope.addEventListener("click", () => {
  const opened = letter.classList.toggle("show");
  envelope.querySelector(".seal").textContent = opened ? "💖" : "💌";
  document.getElementById("letterHint").textContent =
    opened ? "A little letter, written with love ♡" : "Tap to open your letter";
});

/* Reveal the reasons */
document.querySelectorAll(".reason").forEach(card => {
  card.addEventListener("click", () => card.classList.toggle("revealed"));
});

/* Birthday gift and confetti */
let giftOpened = false;

function confetti() {
  const symbols = ["💗","💕","✨","🌸","🎉","♡"];
  for (let i = 0; i < 35; i++) {
    const item = document.createElement("span");
    item.textContent = symbols[Math.floor(Math.random()*symbols.length)];
    item.style.cssText =
      "position:fixed;z-index:30;top:-30px;pointer-events:none;transition:transform 2.5s ease,opacity 2.5s ease;";
    item.style.left = (5 + Math.random()*90) + "vw";
    item.style.fontSize = (14 + Math.random()*18) + "px";
    document.body.appendChild(item);

    requestAnimationFrame(() => {
      item.style.transform =
        `translate(${Math.random()*100-50}px,${innerHeight+80}px) rotate(${Math.random()*500}deg)`;
      item.style.opacity = "0";
    });
    setTimeout(() => item.remove(), 2800);
  }
}

document.getElementById("gift").addEventListener("click", () => {
  if (giftOpened) return;
  giftOpened = true;
  document.getElementById("secretMessage").classList.add("show");
  document.getElementById("giftHint").textContent = "Surprise! This is all for you 💗";
  document.getElementById("gift").textContent = "💝";
  confetti();
});

document.getElementById("loveButton").addEventListener("click", () => {
  document.getElementById("loveResponse").textContent =
    "A little love sent from Biraja to Kyuutu. ♡";
  confetti();
});
</script>
</body>
</html>
