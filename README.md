
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#ffe4ef">
<title>For My Kyuutu ♡</title>

<style>
:root{--pink:#ef83b0;--deep:#a72f68;--ink:#713950;--pale:#fff3f8;--white:#fffafd;--line:#f5c5da}
*{box-sizing:border-box}
html{scroll-behavior:smooth;scroll-padding-top:75px}
body{margin:0;color:var(--ink);font-family:Georgia,"Times New Roman",serif;background:radial-gradient(ellipse at 5% 5%,#fff 0,transparent 40%),radial-gradient(ellipse at 95% 25%,#ffd0e4 0,transparent 40%),linear-gradient(145deg,#fff7fb,#ffe4ef,#fff8fb);overflow-x:hidden}
body.locked{overflow:hidden}
button,input{font:inherit}
button,a{-webkit-tap-highlight-color:transparent}
a{color:inherit;text-decoration:none}
button{cursor:pointer}
nav{position:sticky;top:0;z-index:20;display:flex;align-items:center;justify-content:space-between;gap:8px;padding:13px 4%;background:#fff5faed;backdrop-filter:blur(14px);border-bottom:1px solid #fff}
.brand{font-weight:bold;color:var(--deep);white-space:nowrap}
.navlinks{display:flex;gap:12px;overflow-x:auto;font:11px Arial,sans-serif}
.navlinks a{white-space:nowrap}
.navlinks a:hover{color:#e15a98}
section{padding:65px 5%;position:relative}
.hero{min-height:89vh;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;padding-top:50px}
.eyebrow{color:var(--deep);text-transform:uppercase;letter-spacing:3px;font:10px Arial,sans-serif}
h1{font-size:clamp(3.5rem,14vw,7rem);line-height:.96;color:var(--deep);font-weight:normal;margin:20px 0}
h1 em{color:#e26b9f}
h2{font-size:clamp(2rem,7vw,3.1rem);color:var(--deep);font-weight:normal;margin:12px 0 18px}
h3{color:var(--deep)}
p{line-height:1.8}
.subtitle{max-width:520px}
.head{text-align:center;max-width:680px;margin:0 auto 30px}
.head p{max-width:560px;margin-left:auto;margin-right:auto}
.btn{display:inline-block;border:0;border-radius:40px;padding:14px 22px;color:white;background:linear-gradient(135deg,#f1a0c2,#d64e8d);box-shadow:0 8px 25px #b8327025;transition:transform .2s}
.btn:hover{transform:translateY(-3px)}
.btn.light{background:white;color:var(--deep);border:1px solid var(--line)}
.hero-heart{font-size:4rem;animation:pulse 1.8s infinite}
@keyframes pulse{50%{transform:scale(1.13)}}
@keyframes floatUp{0%{transform:translateY(0) rotate(0);opacity:0}15%{opacity:.8}100%{transform:translateY(-110vh) rotate(40deg);opacity:0}}
.heart-float{position:fixed;bottom:-35px;z-index:1;pointer-events:none;color:#e56ca0;animation:floatUp linear forwards}
.card{background:#ffffffc9;border:1px solid white;border-radius:24px;padding:23px;box-shadow:0 12px 36px #a83e7117;backdrop-filter:blur(10px)}
.center{text-align:center}
.small{font:12px Arial,sans-serif;opacity:.8}
.pill{display:inline-block;border:1px solid #f5c5da;border-radius:40px;padding:7px 12px;margin:4px;background:#fff9fc;font-size:.85rem}
.countdown{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:8px;max-width:550px;margin:24px auto}
.timebox{padding:14px 2px;border-radius:15px;border:1px solid var(--line);background:#fff9fc}
.timebox strong{display:block;color:var(--deep);font-size:clamp(1.4rem,6vw,2.4rem)}
.timebox small{font:9px Arial,sans-serif;letter-spacing:1px}
.gallery{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:13px}
.photo{min-width:0;background:white;padding:8px 8px 13px;border-radius:7px;box-shadow:0 8px 24px #8e3d621b;transform:rotate(-1deg)}
.photo:nth-child(even){transform:rotate(1.2deg)}
.photo img{width:100%;aspect-ratio:3/4;object-fit:cover;display:block;background:#ffe1ed;border-radius:4px;cursor:pointer}
.photo p{text-align:center;font-size:.86rem;margin:9px 2px 0}
.note{text-align:center;font:12px Arial,sans-serif;opacity:.8}
.storyline{max-width:600px;margin:auto}
.storyitem{position:relative;margin:16px 0;padding:18px 20px 18px 27px;border-left:3px solid #e78ab3;background:#ffffffa6;border-radius:0 16px 16px 0}
.storyitem:before{content:"♡";position:absolute;left:-13px;top:17px;background:#fff0f7;color:var(--deep);border-radius:50%;padding:2px 5px}
.reasons{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px}
.reason{min-height:130px;border:1px solid white;border-radius:19px;padding:16px 10px;background:#ffffffc9;color:var(--ink)}
.reason .emoji{display:block;font-size:1.8rem;margin-bottom:8px}
.answer{display:none;font-size:.9rem;line-height:1.6}
.reason.revealed .prompt{display:none}
.reason.revealed .answer{display:block;animation:appear .3s}
.envelope{width:min(280px,90%);height:170px;background:#f3a0c3;border:0;border-radius:12px;margin:20px auto;position:relative;box-shadow:0 12px 30px #a83e7120;overflow:hidden}
.envelope:before{content:"";position:absolute;inset:0;background:#ec8ab6;clip-path:polygon(0 0,50% 58%,100% 0)}
.seal{position:relative;z-index:1;font-size:3rem}
.letter{display:none;text-align:left;white-space:pre-line;line-height:1.9;padding:clamp(20px,5vw,38px);background:#fffdfb;border-radius:16px;border:1px solid #f4d4e2}
.letter.show{display:block;animation:appear .6s}
@keyframes appear{from{opacity:0;transform:translateY(12px)}to{opacity:1;transform:translateY(0)}}
.music{max-width:540px;margin:auto;text-align:center}
.bigemoji{font-size:4rem;display:block;margin:15px auto}
.cake{font-size:5rem;border:0;background:none;transition:.3s}
.cake:hover{transform:scale(1.1)}
.candles{font-size:2rem;letter-spacing:7px}
.jar{font-size:4rem;border:0;background:none}
.jar-message{font-size:1.1rem;color:var(--deep);min-height:55px}
.envelopes{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
.mini-envelope{background:#fff0f7;border:1px solid #f5bfd7;border-radius:15px;padding:18px 5px;font-size:2rem}
.mini-envelope small{display:block;font:11px Arial,sans-serif;margin-top:8px}
.quiz-option{display:block;width:100%;margin:9px 0;padding:12px;border-radius:14px;background:#fff5fa;border:1px solid var(--line);color:var(--ink)}
.quiz-option:hover{background:#ffe4ef}
.quiz-result{min-height:35px;color:var(--deep)}
.future-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.future-card{padding:17px;border-radius:17px;background:#fff8fc;border:1px solid white}
.appreciation{display:flex;flex-wrap:wrap;justify-content:center;gap:8px}
.hidden-heart{display:inline-block;margin:8px;padding:8px;border:0;border-radius:50%;background:#fff0f7;font-size:1.5rem}
.hidden-heart.found{background:#f3b1cf;transform:scale(1.12)}
.secret-message{display:none}
.secret-message.show{display:block;animation:appear .6s}
footer{text-align:center;padding:40px 15px 55px;background:#ffffff75}
footer .footer-heart{font-size:2rem;color:var(--deep)}
#toast{position:fixed;bottom:20px;left:50%;transform:translateX(-50%);background:#96325f;color:white;padding:12px 18px;border-radius:30px;z-index:1050;display:none;text-align:center;width:max-content;max-width:90%}
#lightbox{display:none;position:fixed;inset:0;z-index:1040;background:#371422e8;align-items:center;justify-content:center;padding:18px}
#lightbox.open{display:flex}
#lightbox img{max-width:100%;max-height:82vh;object-fit:contain;border-radius:12px}
#lightbox button{position:absolute;top:18px;right:18px;border:0;border-radius:50%;width:42px;height:42px;font-size:1.4rem;background:white;color:var(--deep)}

/* Floating hearts and stars across the entire page */
#love-sky{position:fixed;inset:0;overflow:hidden;pointer-events:none;z-index:1001;contain:strict}
.love-particle{position:absolute;bottom:-45px;left:var(--left);color:var(--color);font-size:var(--size);opacity:0;animation:love-float var(--speed) linear var(--delay) infinite;text-shadow:0 0 12px #ffb5d7;will-change:transform,opacity}
.love-particle.star{color:#e7a83e;text-shadow:0 0 10px #ffe8a3}
@keyframes love-float{
  0%{transform:translate3d(0,0,0) rotate(0deg) scale(.7);opacity:0}
  12%{opacity:.8}
  50%{transform:translate3d(25px,-55vh,0) rotate(100deg) scale(1);opacity:.75}
  90%{opacity:.5}
  100%{transform:translate3d(-20px,-115vh,0) rotate(240deg) scale(.8);opacity:0}
}

/* Song player inside the locked screen, above the countdown */
.lock-music{margin:18px auto;padding:15px;background:#fff5fa;border:1px solid #f5c5da;border-radius:20px}
.lock-music audio{display:block;width:100%;margin:12px 0}
.song-timer{display:flex;justify-content:space-between;gap:10px;font:12px Arial,sans-serif}
.song-progress{width:100%;height:5px;border-radius:10px;background:#f5c5da;overflow:hidden;margin-top:10px}
.song-progress-fill{height:100%;width:0%;background:linear-gradient(90deg,#f1a0c2,#d64e8d);transition:width .15s linear}

#birthdayLock{position:fixed;inset:0;z-index:1000;overflow-y:auto;display:flex;align-items:center;justify-content:center;padding:15px;background:linear-gradient(145deg,#ffe0ed,#fff5fa,#f9d9ee)}
.lock-card{width:min(520px,100%);padding:24px 18px;border-radius:28px;background:#ffffffed;box-shadow:0 10px 45px #c64a8633;text-align:center}
.lock-card h1{font-size:clamp(2.7rem,10vw,4rem)}
@media(min-width:700px){
  section{padding:85px 9%}
  .gallery{grid-template-columns:repeat(3,minmax(0,1fr));gap:20px}
  .reasons{grid-template-columns:repeat(3,minmax(0,1fr))}
}
@media(max-width:370px){
  .navlinks{gap:8px;font-size:10px}
  .brand{font-size:.9rem}
  section{padding:55px 4%}
  .card{padding:17px}
  #birthdayLock{padding:8px}
  .lock-card{padding:18px 12px}
  .lock-music{padding:11px}
}
@media(prefers-reduced-motion:reduce){
  *,*:before,*:after{animation:none!important;scroll-behavior:auto!important}
  .love-particle{display:none}
}
</style>
</head>

<body class="locked">

<!-- Decorative hearts and stars stay above the page without blocking taps -->
<div id="love-sky" aria-hidden="true"></div>

<!-- BIRTHDAY LOCK: SONG IS PLAYABLE BEFORE UNLOCK -->
<div id="birthdayLock">
  <div class="lock-card">
    <div style="font-size:3.5rem">🎀💗🦋</div>
    <p class="eyebrow">A little surprise is waiting</p>
    <h1>For My<br><em>Kyuutu</em> ♡</h1>
    <p>Dear Anuska, this little world was made just for you, with memories, music and tiny surprises. 🌷</p>

    <div class="lock-music">
      <p class="eyebrow">A song picked just for you 🎶</p>
      <h3>Tera Naam Doon ♡</h3>
      <p class="small">A little birthday soundtrack for my favourite girl. 💗</p>
      <audio id="topSong" controls loop preload="metadata">
        <source src="Tera%20Naam%20Doon%20Entertainment%20320%20Kbps.mp3" type="audio/mpeg">
        Your browser does not support this audio file.
      </audio>
      <div class="song-timer">
        <span id="songElapsed">0:00</span>
        <span id="songDuration">0:00</span>
      </div>
      <div class="song-progress" aria-label="Song progress">
        <div class="song-progress-fill" id="songProgressFill"></div>
      </div>
      <p class="small">Tap play to listen 🎧</p>
    </div>

    <div class="countdown">
      <div class="timebox"><strong id="lockDays">--</strong><small>DAYS</small></div>
      <div class="timebox"><strong id="lockHours">--</strong><small>HOURS</small></div>
      <div class="timebox"><strong id="lockMinutes">--</strong><small>MINUTES</small></div>
      <div class="timebox"><strong id="lockSeconds">--</strong><small>SECONDS</small></div>
    </div>
    <p id="lockMessage">Your birthday surprise unlocks at midnight. 💌</p>
    <p class="small">5 October 2026 · 12:00 AM IST ♡</p>
  </div>
</div>

<nav>
  <a class="brand" href="#home">♡ Kyuutu's World</a>
  <div class="navlinks">
    <a href="#birthday">Birthday</a>
    <a href="#memories">Photos</a>
    <a href="#letter">Letter</a>
    <a href="#music">Song</a>
    <a href="#final">Surprise</a>
  </div>
</nav>

<main>
<section class="hero" id="home">
  <p class="eyebrow">A little world made with love</p>
  <h1>For my<br><em>Kyuutu</em> ♡</h1>
  <p class="subtitle">To my favourite girl, Anuska. This little world is made just for you, with sweet memories, tiny surprises and a whole lot of love.</p>
  <div class="hero-heart">💗</div>
  <p>Made with love by Biraja Prasad Jena</p>
  <a class="btn" href="#birthday">Enter your little world ↓</a>
  <p class="small">20 little corners, one special girl 🌷</p>
</section>

<section id="birthday">
  <div class="head"><p class="eyebrow">Save the date</p><h2>It's your day, Kyuutu 🎂</h2><p>October 5 is special because the world welcomed you.</p></div>
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

<section id="greeting">
  <div class="head"><p class="eyebrow">A message for you</p><h2>Happy Birthday, Anuska! 🌷</h2></div>
  <div class="card center">
    <span class="bigemoji">🎂🌸🎀</span>
    <p>Today is a celebration of you — your dreams, your laughter, your kindness and every little thing that makes you who you are.</p>
    <p>May this new chapter bring peaceful days, beautiful opportunities, genuine smiles and people who treat your heart with care.</p>
    <a class="btn" href="#memories">Let's look at our memories ♡</a>
  </div>
</section>

<section id="memories">
  <div class="head"><p class="eyebrow">Little moments, big feelings</p><h2>Our memory corner 📸</h2><p>Tap any picture to see it bigger. Twelve little spaces for memories to treasure.</p></div>
  <div class="gallery">
    <div class="photo"><img src="IMG-20260329-WA0053(1).jpg" alt="Memory 1" loading="lazy"><p>A favourite moment ♡</p></div>
    <div class="photo"><img src="IMG-20260404-WA0112.jpg" alt="Memory 2" loading="lazy"><p>A little memory 🌷</p></div>
    <div class="photo"><img src="IMG-20260501-WA0167.jpg" alt="Memory 3" loading="lazy"><p>You make moments special ✨</p></div>
    <div class="photo"><img src="IMG-20260527-WA0055.jpg" alt="Memory 4" loading="lazy"><p>One for the memory book 💗</p></div>
    <div class="photo"><img src="IMG-20260617-WA0067.jpg" alt="Memory 5" loading="lazy"><p>Sweet little memories 🌸</p></div>
    <div class="photo"><img src="IMG-20260617-WA0105.jpg" alt="Memory 6" loading="lazy"><p>Another moment to keep ♡</p></div>
    <div class="photo"><img src="IMG-20260729-WA0018.jpg" alt="Memory 7" loading="lazy"><p>Little things, big feelings 💕</p></div>
    <div class="photo"><img src="IMG-20260811-WA0055.jpg" alt="Memory 8" loading="lazy"><p>A lovely little moment ✨</p></div>
    <div class="photo"><img src="IMG-20260829-WA0026.jpg" alt="Memory 9" loading="lazy"><p>One more for us 🌷</p></div>
    <div class="photo"><img src="IMG-20260909-WA0045.jpg" alt="Memory 10" loading="lazy"><p>Something to smile about 😊</p></div>
    <div class="photo"><img src="IMG-20260917-WA0025.jpg" alt="Memory 11" loading="lazy"><p>Memories worth keeping 💗</p></div>
    <div class="photo"><img src="IMG-20260921-WA0050.jpg" alt="Memory 12" loading="lazy"><p>More memories to come ♡</p></div>
  </div>
  <p class="note">A little gallery made just for you.</p>
</section>

<section id="scrapbook">
  <div class="head"><p class="eyebrow">A page from our scrapbook</p><h2>Little things to remember 📔</h2></div>
  <div class="card center">
    <span class="bigemoji">📷💌🌷</span>
    <p>Some memories are loud and exciting. Others are tiny moments, simple words or a conversation that makes you smile later.</p>
    <p>This page is a reminder that lovely memories don't have to be perfect or extraordinary. Sometimes, the smallest things become the ones we cherish.</p>
    <span class="pill">Little moments</span><span class="pill">Real smiles</span><span class="pill">Sweet memories</span><span class="pill">More to come</span>
  </div>
</section>

<section id="story">
  <div class="head"><p class="eyebrow">Every story has little chapters</p><h2>Our story, one step at a time 🌙</h2><p>Edit these captions whenever you want to add your own special dates.</p></div>
  <div class="storyline">
    <div class="storyitem"><strong>Chapter 1 — The beginning 🌸</strong><p>Every meaningful story starts somewhere. This is a little space for the beginning of ours.</p></div>
    <div class="storyitem"><strong>Chapter 2 — Getting to know you 💬</strong><p>Little conversations, discovering the things that make each other smile, and learning more along the way.</p></div>
    <div class="storyitem"><strong>Chapter 3 — Little memories 📸</strong><p>Moments that become special because we remember how they made us feel.</p></div>
    <div class="storyitem"><strong>Chapter 4 — Today, and what's ahead 💗</strong><p>Celebrating you today and leaving room for many more lovely chapters in the future.</p></div>
  </div>
</section>

<section id="adore">
  <div class="head"><p class="eyebrow">The little things</p><h2>Things I adore about you 🌷</h2></div>
  <div class="card center">
    <span class="bigemoji">🎀🌸🦋</span>
    <p>Your unique personality, the little things that make you laugh, the way you have your own dreams and ideas, and the person you continue to become.</p>
    <p>You don't have to be perfect to be appreciated. You deserve to be valued for who you are, on ordinary days as much as special ones.</p>
  </div>
</section>

<section id="reasons">
  <div class="head"><p class="eyebrow">Tap to discover</p><h2>Reasons you're special 💕</h2><p>Open each card for a little reminder.</p></div>
  <div class="reasons">
    <button class="reason"><span class="emoji">🌸</span><span class="prompt">Reason one…</span><span class="answer">I appreciate the unique person you are.</span></button>
    <button class="reason"><span class="emoji">😊</span><span class="prompt">Reason two…</span><span class="answer">Your smile can make an ordinary moment feel special.</span></button>
    <button class="reason"><span class="emoji">🫶</span><span class="prompt">Reason three…</span><span class="answer">I value the trust we build by being honest with each other.</span></button>
    <button class="reason"><span class="emoji">✨</span><span class="prompt">Reason four…</span><span class="answer">You have your own magic. You don't need to be anyone else.</span></button>
    <button class="reason"><span class="emoji">🌷</span><span class="prompt">Reason five…</span><span class="answer">I love learning the little things that make you happy.</span></button>
    <button class="reason"><span class="emoji">💗</span><span class="prompt">One last reason…</span><span class="answer">Being yourself is already something special, Kyuutu.</span></button>
  </div>
</section>

<section id="letter">
  <div class="head"><p class="eyebrow">Just between us</p><h2>A letter from me 💌</h2><p>Tap the envelope to open your letter.</p></div>
  <div class="center">
    <button class="envelope" id="envelope" aria-label="Open the birthday letter"><span class="seal">💌</span></button>
    <p class="small" id="letterHint">Tap to open your letter</p>
  </div>
  <article class="letter" id="letterContent"><h3>To my Kyuutu, Anuska ♡</h3>
Happy Birthday, my girl! 🎂💗

I may not always find the perfect words, but today I want you to know how special you are to me.

Thank you for being yourself, for your little ways, your smile, and the moments that become beautiful simply because you're part of them. Even a small conversation can make an ordinary day feel different.

For this new year of your life, I wish you peace, happiness, courage for your dreams, good health, and countless reasons to smile. I hope you always remember that you matter and deserve kindness, respect and beautiful things.

I don't expect every day to be perfect. I hope we continue to understand each other, speak honestly, respect each other, and make lovely memories along the way.

This website is a little birthday gift, made with thought and affection, to celebrate the wonderful person you are.

Keep smiling, keep dreaming, and keep being your adorable self.

Happy Birthday once again, my Kyuutu. 🌷

With lots of love,
Your Biraja ♡</article>
</section>

<section id="music">
  <div class="head"><p class="eyebrow">A song for my girl</p><h2>Our little soundtrack 🎶</h2></div>
  <div class="card music">
    <span class="bigemoji">🎧💗🎵</span>
    <h3>Tera Naam Doon ♡</h3>
    <p>The song player is available on the birthday countdown screen. ♡</p>
    <a class="btn light" href="#birthdayLock">Go to the song ↑</a>
    <p class="small">Tap play whenever you're ready to listen.</p>
  </div>
</section>

<section id="cake">
  <div class="head"><p class="eyebrow">Time for cake</p><h2>A little virtual birthday cake 🎂</h2><p>Tap the cake to celebrate!</p></div>
  <div class="card center">
    <button class="cake" id="cakeButton" aria-label="Celebrate with cake">🎂</button>
    <div class="candles" id="candles">🕯️ 🕯️ 🕯️</div>
    <p id="cakeMessage">Three little candles, a world of wishes.</p>
    <button class="btn" id="cakeCelebrate">Celebrate! 🎉</button>
  </div>
</section>

<section id="wish">
  <div class="head"><p class="eyebrow">Make a wish</p><h2>A wish for your new chapter 🌟</h2></div>
  <div class="card center">
    <span class="bigemoji">🌙✨🌸</span>
    <p>Take a little moment for yourself. Think of a dream you're excited about, a place you'd like to see, a skill you'd like to learn or something that would bring you joy.</p>
    <button class="btn" id="wishButton">I've made my wish ♡</button>
    <p id="wishMessage" class="quiz-result">Your wish is yours to keep. 💗</p>
  </div>
</section>

<section id="jar">
  <div class="head"><p class="eyebrow">A jar of kind words</p><h2>Pick a little compliment 🌷</h2><p>Tap the jar whenever you need a smile.</p></div>
  <div class="card center">
    <button class="jar" id="jarButton" aria-label="Pick a compliment">🫙</button>
    <p class="jar-message" id="jarMessage">Your little compliment is waiting…</p>
    <button class="btn light" id="anotherCompliment">Another one ♡</button>
  </div>
</section>

<section id="envelopes">
  <div class="head"><p class="eyebrow">Choose your surprise</p><h2>Three little envelopes 💌</h2><p>Tap each envelope to reveal a message.</p></div>
  <div class="envelopes">
    <button class="mini-envelope" data-message="You deserve gentle days, sincere people and reasons to smile. 🌸">💌<small>Envelope 1</small></button>
    <button class="mini-envelope" data-message="Never stop believing in your dreams. Every small step matters. ✨">💌<small>Envelope 2</small></button>
    <button class="mini-envelope" data-message="A little reminder from Biraja: you're appreciated just as you are. 💗">💌<small>Envelope 3</small></button>
  </div>
  <div class="card center" style="margin-top:18px"><p id="envelopeMessage">Choose an envelope to open your note.</p></div>
</section>

<section id="quiz">
  <div class="head"><p class="eyebrow">A tiny game</p><h2>A little birthday quiz 🎀</h2><p>No wrong answers — just a little fun!</p></div>
  <div class="card">
    <h3>What makes a birthday feel special?</h3>
    <button class="quiz-option" data-answer="A">A. Thoughtful moments and kindness 💗</button>
    <button class="quiz-option" data-answer="B">B. Only expensive presents 🎁</button>
    <button class="quiz-option" data-answer="C">C. A perfect photo 🌸</button>
    <p id="quizResult" class="quiz-result">Pick your answer!</p>
  </div>
</section>

<section id="future">
  <div class="head"><p class="eyebrow">There is more ahead</p><h2>Future memories waiting to happen 🌈</h2></div>
  <div class="future-grid">
    <div class="future-card"><span>🌅</span><h3>New beginnings</h3><p>More days to learn and grow.</p></div>
    <div class="future-card"><span>📸</span><h3>More memories</h3><p>More little moments to remember.</p></div>
    <div class="future-card"><span>🌍</span><h3>New adventures</h3><p>New places, ideas and experiences.</p></div>
    <div class="future-card"><span>💗</span><h3>More kindness</h3><p>Honest words and thoughtful gestures.</p></div>
  </div>
</section>

<section id="appreciation">
  <div class="head"><p class="eyebrow">A wall of warm wishes</p><h2>Little reminders for you 🌸</h2></div>
  <div class="card center">
    <div class="appreciation">
      <span class="pill">You matter ♡</span><span class="pill">Keep dreaming ✨</span>
      <span class="pill">You are appreciated 🌷</span><span class="pill">Take your time 🌙</span>
      <span class="pill">Celebrate your growth 🌱</span><span class="pill">Be kind to yourself 💗</span>
      <span class="pill">Your ideas matter 🎀</span><span class="pill">You deserve respect 🫶</span>
    </div>
    <p>Save this little reminder for days when you need it: you don't have to do everything perfectly to be worthy of love and kindness.</p>
  </div>
</section>

<section id="hunt">
  <div class="head"><p class="eyebrow">Can you find them?</p><h2>Hidden heart treasure hunt 🔎</h2><p>Tap the hearts below. Find all five to unlock a tiny message!</p></div>
  <div class="card center">
    <div id="heartHunt">
      <button class="hidden-heart" aria-label="Find heart 1">♡</button>
      <button class="hidden-heart" aria-label="Find heart 2">♡</button>
      <button class="hidden-heart" aria-label="Find heart 3">♡</button>
      <button class="hidden-heart" aria-label="Find heart 4">♡</button>
      <button class="hidden-heart" aria-label="Find heart 5">♡</button>
    </div>
    <p id="huntCount">Hearts found: 0 / 5</p>
    <p id="huntMessage">Your treasure hunt begins! 💗</p>
  </div>
</section>

<section id="secret">
  <div class="head"><p class="eyebrow">One last little note</p><h2>A secret just for you 🤫</h2></div>
  <div class="card center">
    <button class="btn" id="secretButton">Reveal the secret 💗</button>
    <div class="secret-message" id="secretMessage">
      <span class="bigemoji">💝</span><h3>Dear Kyuutu,</h3>
      <p>This little website may be made of code, pictures and words, but the thought behind it is simple: I wanted to make something personal to celebrate you.</p>
      <p>Thank you for being the person you are. May this year bring you moments that make your heart feel light and your dreams feel closer.</p>
      <p>With love, Biraja ♡</p>
    </div>
  </div>
</section>

<section id="final">
  <div class="head"><p class="eyebrow">The final surprise</p><h2>Happy Birthday, my Kyuutu! 🎂</h2><p>One last button. One more birthday wish. All for you.</p></div>
  <div class="card center">
    <button class="cake" id="finalGift" aria-label="Reveal final birthday surprise">🎁</button>
    <p id="finalHint">Tap your gift to finish the celebration!</p>
    <div class="secret-message" id="finalMessage">
      <span class="bigemoji">🎉💗🌸🎂</span>
      <h2>Happy Birthday, Anuska!</h2>
      <p>May your days be filled with laughter, your heart with peace, and your life with opportunities to become everything you dream of.</p>
      <p>Keep smiling, keep growing, and never forget how special you are.</p>
      <h3>With lots of love, your Biraja ♡</h3>
      <button class="btn" id="sendLove">Send one last burst of love 💗</button>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="footer-heart">♡</div>
  <p>Made especially for Anuska, my Kyuutu.</p>
  <p class="small">A little pink world by Biraja Prasad Jena · 2026</p>
  <a class="small" href="#home">Back to the beginning ↑</a>
</footer>

<div id="lightbox" aria-label="Expanded photo">
  <button id="closeLightbox" aria-label="Close photo">×</button>
  <img id="lightboxImage" src="" alt="Expanded memory">
</div>
<div id="toast" role="status"></div>

<script>
/* Birthday countdown and automatic unlock: 5 October 2026 at midnight IST */
const birthday = new Date("2026-10-05T00:00:00+05:30");
const birthdayEnd = new Date("2026-10-06T00:00:00+05:30");

function updateBirthdayLock(){
  const remaining = birthday.getTime() - Date.now();
  const lock = document.getElementById("birthdayLock");

  if(remaining <= 0){
    lock.style.display = "none";
    document.body.classList.remove("locked");
    return;
  }

  lock.style.display = "flex";
  document.body.classList.add("locked");
  document.getElementById("lockDays").textContent = String(Math.floor(remaining/86400000)).padStart(2,"0");
  document.getElementById("lockHours").textContent = String(Math.floor(remaining/3600000)%24).padStart(2,"0");
  document.getElementById("lockMinutes").textContent = String(Math.floor(remaining/60000)%60).padStart(2,"0");
  document.getElementById("lockSeconds").textContent = String(Math.floor(remaining/1000)%60).padStart(2,"0");
}

function updateCountdown(){
  const now = Date.now();
  const diff = birthday.getTime() - now;
  const label = document.getElementById("countLabel");
  const msg = document.getElementById("birthdayMessage");
  const boxes = document.getElementById("countBoxes");

  if(now >= birthday.getTime() && now < birthdayEnd.getTime()){
    label.textContent = "It's your birthday, Kyuutu! 🎂";
    msg.textContent = "Today is all about you. Happy Birthday! 💗";
    boxes.style.display = "grid";
    ["days","hours","minutes","seconds"].forEach((id,i)=>{
      document.getElementById(id).textContent = ["🎂","💗","🎉","♡"][i];
    });
    return;
  }

  if(diff <= 0){
    boxes.style.display = "none";
    label.textContent = "Your birthday has arrived and passed for this year 💕";
    msg.textContent = "The birthday wishes stay here for you!";
    return;
  }

  boxes.style.display = "grid";
  document.getElementById("days").textContent = Math.floor(diff/86400000);
  document.getElementById("hours").textContent = Math.floor(diff/3600000)%24;
  document.getElementById("minutes").textContent = Math.floor(diff/60000)%60;
  document.getElementById("seconds").textContent = Math.floor(diff/1000)%60;
}

updateBirthdayLock();
updateCountdown();
setInterval(()=>{updateBirthdayLock();updateCountdown();},1000);

/* Song elapsed timer, duration and progress bar */
const topSong = document.getElementById("topSong");

function formatSongTime(seconds){
  if(!Number.isFinite(seconds) || seconds < 0) return "0:00";
  return Math.floor(seconds/60)+":"+String(Math.floor(seconds%60)).padStart(2,"0");
}

function updateSongTimer(){
  document.getElementById("songElapsed").textContent = formatSongTime(topSong.currentTime);
  document.getElementById("songDuration").textContent = formatSongTime(topSong.duration);

  const duration = topSong.duration;
  const progress = Number.isFinite(duration) && duration > 0
    ? (topSong.currentTime/duration)*100 : 0;

  document.getElementById("songProgressFill").style.width = Math.min(100,progress)+"%";
}

topSong.addEventListener("loadedmetadata",updateSongTimer);
topSong.addEventListener("durationchange",updateSongTimer);
topSong.addEventListener("timeupdate",updateSongTimer);

/* Floating hearts */
const heartSymbols = ["♡","♥","💗","💕","✧"];
function createHeart(){
  const el = document.createElement("span");
  el.className = "heart-float";
  el.textContent = heartSymbols[Math.floor(Math.random()*heartSymbols.length)];
  el.style.left = Math.random()*100+"vw";
  el.style.fontSize = (12+Math.random()*19)+"px";
  el.style.animationDuration = (7+Math.random()*6)+"s";
  document.body.appendChild(el);
  setTimeout(()=>el.remove(),14000);
}
setInterval(createHeart,1200);

/* Floating hearts and stars throughout the website */
(function createLoveSky(){
  const sky = document.getElementById("love-sky");
  const symbols = ["♡","♥","💗","💕","✧","⋆","✦","✨","☆"];
  const colors = ["#ed75a8","#d95b91","#f4a6c7","#e7a83e","#c99be8"];

  for(let i=0;i<32;i++){
    const particle = document.createElement("span");
    const isStar = Math.random() < 0.45;
    particle.className = "love-particle"+(isStar?" star":"");
    particle.textContent = isStar
      ? ["✧","⋆","✦","✨","☆"][Math.floor(Math.random()*5)]
      : ["♡","♥","💗","💕"][Math.floor(Math.random()*4)];

    particle.style.setProperty("--left",Math.random()*100+"%");
    particle.style.setProperty("--size",(12+Math.random()*18)+"px");
    particle.style.setProperty("--speed",(9+Math.random()*12)+"s");
    particle.style.setProperty("--delay",(-Math.random()*20)+"s");
    particle.style.setProperty("--color",colors[Math.floor(Math.random()*colors.length)]);
    sky.appendChild(particle);
  }
})();

/* Toast notifications */
let toastTimer;
function toast(message){
  const el = document.getElementById("toast");
  el.textContent = message;
  el.style.display = "block";
  clearTimeout(toastTimer);
  toastTimer = setTimeout(()=>el.style.display="none",2400);
}

/* Gallery lightbox */
document.querySelectorAll(".photo img").forEach(img=>{
  img.addEventListener("click",()=>{
    document.getElementById("lightboxImage").src = img.src;
    document.getElementById("lightbox").classList.add("open");
  });
});

function closeLightbox(){
  document.getElementById("lightbox").classList.remove("open");
  document.getElementById("lightboxImage").src = "";
}

document.getElementById("closeLightbox").addEventListener("click",closeLightbox);
document.getElementById("lightbox").addEventListener("click",e=>{
  if(e.target.id === "lightbox") closeLightbox();
});

/* Birthday letter */
document.getElementById("envelope").addEventListener("click",()=>{
  const letter = document.getElementById("letterContent");
  const opened = letter.classList.toggle("show");
  document.querySelector("#envelope .seal").textContent = opened ? "💖" : "💌";
  document.getElementById("letterHint").textContent =
    opened ? "A little letter, written with love ♡" : "Tap to open your letter";
});

/* Reasons cards */
document.querySelectorAll(".reason").forEach(card=>{
  card.addEventListener("click",()=>card.classList.toggle("revealed"));
});

/* Confetti */
function confetti(){
  const symbols = ["💗","💕","✨","🌸","🎉","♡"];
  for(let i=0;i<38;i++){
    const item = document.createElement("span");
    item.textContent = symbols[Math.floor(Math.random()*symbols.length)];
    item.style.cssText = "position:fixed;z-index:1035;top:-30px;pointer-events:none;transition:transform 2.5s ease,opacity 2.5s ease";
    item.style.left = (5+Math.random()*90)+"vw";
    item.style.fontSize = (14+Math.random()*18)+"px";
    document.body.appendChild(item);

    requestAnimationFrame(()=>{
      item.style.transform = `translate(${Math.random()*100-50}px,${innerHeight+80}px) rotate(${Math.random()*500}deg)`;
      item.style.opacity = "0";
    });
    setTimeout(()=>item.remove(),2800);
  }
}

/* Birthday cake */
let cakeTaps = 0;
document.getElementById("cakeButton").addEventListener("click",()=>{
  cakeTaps++;
  const messages = [
    "Make a little wish, Kyuutu! 🌟",
    "One more birthday wish for you! 💗",
    "May your wishes bring you joy! 🌸",
    "Sending you a whole lot of love! 🎂"
  ];
  document.getElementById("cakeMessage").textContent = messages[Math.min(cakeTaps-1,3)];
  if(cakeTaps>=3) confetti();
});

document.getElementById("cakeCelebrate").addEventListener("click",()=>{
  document.getElementById("candles").textContent = "✨ 💗 ✨";
  document.getElementById("cakeMessage").textContent = "Cake, wishes and happiness for my Kyuutu!";
  confetti();
});

/* Make a wish */
document.getElementById("wishButton").addEventListener("click",()=>{
  document.getElementById("wishMessage").textContent = "Wish made! Keep believing in the lovely things ahead. ♡";
  confetti();
});

/* Compliment jar */
const compliments = [
  "Your dreams deserve time and care. 🌷",
  "You bring your own special energy to the world. ✨",
  "You deserve kindness, respect and happiness. 💗",
  "Keep being curious and keep growing. 🌱",
  "Your smile is worth celebrating. 😊",
  "You don't need to be perfect to be wonderful. 🌸",
  "I hope today gives you a reason to laugh. 🎀",
  "You are allowed to take things one step at a time. 🫶",
  "Your ideas and feelings matter. 💌",
  "Keep a little room for magic and new beginnings. 🌙"
];

function newCompliment(){
  document.getElementById("jarMessage").textContent =
    compliments[Math.floor(Math.random()*compliments.length)];
}
document.getElementById("jarButton").addEventListener("click",newCompliment);
document.getElementById("anotherCompliment").addEventListener("click",newCompliment);

/* Surprise envelopes */
document.querySelectorAll(".mini-envelope").forEach(btn=>{
  btn.addEventListener("click",()=>{
    document.getElementById("envelopeMessage").textContent = btn.dataset.message;
    btn.innerHTML = '💝<small>Opened ♡</small>';
  });
});

/* Mini quiz */
document.querySelectorAll(".quiz-option").forEach(btn=>{
  btn.addEventListener("click",()=>{
    document.getElementById("quizResult").textContent =
      btn.dataset.answer === "A"
        ? "Correct in this little birthday game! Thoughtful moments can mean so much. 💗"
        : "That's one way to celebrate, too! But kindness and thoughtful moments are lovely gifts. 🌸";
  });
});

/* Hidden heart treasure hunt */
let heartsFound = 0;
document.querySelectorAll(".hidden-heart").forEach(btn=>{
  btn.addEventListener("click",()=>{
    if(btn.classList.contains("found")) return;
    btn.classList.add("found");
    btn.textContent = "💗";
    heartsFound++;
    document.getElementById("huntCount").textContent = `Hearts found: ${heartsFound} / 5`;

    if(heartsFound===5){
      document.getElementById("huntMessage").textContent =
        "You found every heart! Your secret reward: you're appreciated just as you are. 💝";
      confetti();
    }else{
      document.getElementById("huntMessage").textContent = "You found one! Keep going. ♡";
    }
  });
});

/* Secret note */
document.getElementById("secretButton").addEventListener("click",()=>{
  document.getElementById("secretMessage").classList.toggle("show");
});

/* Final birthday gift */
document.getElementById("finalGift").addEventListener("click",()=>{
  document.getElementById("finalMessage").classList.add("show");
  document.getElementById("finalHint").textContent = "Surprise! This little celebration is all for you 💗";
  document.getElementById("finalGift").textContent = "💝";
  confetti();
});

document.getElementById("sendLove").addEventListener("click",()=>{
  toast("A little love sent from Biraja to Kyuutu. ♡");
  confetti();
});
</script>
</body>
</html>
