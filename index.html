<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title id="dynamic-title">Rayhan Hacking Zone</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <script src="https://www.gstatic.com/firebasejs/8.10.0/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/8.10.0/firebase-database.js"></script>
    
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }
        body { background-color: #0b0c10; color: #ffffff; overflow: hidden; }

        #gate-keeper { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: #000; z-index: 70000; display: flex; justify-content: center; align-items: center; }
        .enter-btn { padding: 20px 50px; font-size: 20px; font-weight: bold; color: #fff; background: transparent; border: 2px solid #bc13fe; border-radius: 50px; cursor: pointer; box-shadow: 0 0 20px #bc13fe; transition: 0.3s; text-transform: uppercase; }

        #welcome-screen { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: #000; z-index: 60000; display: none; flex-direction: column; justify-content: center; align-items: center; }
        #welcome-video { width: 85%; max-width: 320px; border: 2px solid #bc13fe; border-radius: 15px; box-shadow: 0 0 20px #bc13fe; }

        #particles-js { position: fixed; width: 100%; height: 100%; top: 0; left: 0; z-index: -1; }
        header { background: rgba(0, 0, 0, 0.9); padding: 15px; border-bottom: 2px solid #bc13fe; text-align: center; position: sticky; top: 0; z-index: 100; }
        #site-logo { font-size: 24px; font-weight: bold; color: #bc13fe; }

        .marquee-box { background: rgba(188, 19, 254, 0.1); color: #ffffff; padding: 10px; font-weight: bold; border-bottom: 1px solid #bc13fe; }
        .hero-container { position: relative; width: 100%; height: 400px; background: #000; border-bottom: 3px solid #bc13fe; overflow: hidden; }
        #hero-img-div { width: 100%; height: 100%; background-repeat: no-repeat; background-position: center; background-size: contain; position: absolute; z-index: 1; filter: drop-shadow(0 0 15px #bc13fe); }
        
        .social-icons { display: flex; justify-content: center; gap: 30px; padding: 20px; }
        .social-icons a { color: #bc13fe; font-size: 35px; transition: 0.3s; }

        .container { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; padding: 40px 5%; padding-bottom: 100px; }
        .card { background: #111; border-radius: 15px; border: 1px solid #333; text-align: center; padding-bottom: 20px; overflow: hidden; transition: 0.3s; }
        .card:hover { border-color: #bc13fe; transform: translateY(-5px); }
        .card img { width: 100%; height: 200px; object-fit: cover; }
        .card h3 { margin: 15px 0 5px; color: #bc13fe; }
        .card p { font-size: 14px; padding: 0 15px; margin-bottom: 15px; color: #ccc; }

        .btn-group { display: flex; flex-direction: column; gap: 10px; align-items: center; }
        .btn { background: #bc13fe; color: white; padding: 10px 25px; border-radius: 50px; font-weight: bold; border:none; cursor:pointer; width: 80%; }
        .btn-video { background: #444; font-size: 12px; padding: 8px 15px; }

        #bottom-nav { position: fixed; bottom: 0; left: 0; width: 100%; height: 75px; background: #000; display: none; justify-content: space-around; align-items: center; border-top: 2.5px solid #bc13fe; z-index: 45000; }
        .nav-item { color: #bc13fe; text-align: center; cursor: pointer; font-weight: bold; font-size: 13px; }
        .nav-item span { font-size: 28px; display: block; }

        /* AI Section Styles */
        .animating { animation: wave-anim 0.8s infinite alternate; }
        @keyframes wave-anim { from { height: 20px; } to { height: 70px; } }
    </style>
</head>
<body onclick="applyClickEffect(event)">

    <div id="gate-keeper"><button class="enter-btn" onclick="startExperience()">Enter System</button></div>

    <div id="welcome-screen">
        <video id="welcome-video" playsinline><source src="https://files.catbox.moe/xn4w8l.mp4" type="video/mp4"></video>
        <div id="progress-container" style="width:250px; height:4px; background:#222; margin-top:20px; border:1px solid #bc13fe;">
            <div id="progress" style="width:0%; height:100%; background:#bc13fe; transition:3s linear;"></div>
        </div>
    </div>

    <div id="particles-js"></div>
    <header><div id="site-logo">Rayhan Hacking Zone</div></header>

    <div class="marquee-box"><marquee id="marquee-text">Loading message...</marquee></div>
    <div class="hero-container"><div id="hero-img-div"></div></div>

    <div class="social-icons">
        <a id="tele-link" href="#" target="_blank"><i class="fab fa-telegram"></i></a>
        <a id="insta-link" href="#" target="_blank"><i class="fab fa-instagram"></i></a>
        <a id="mail-link" href="#"><i class="fas fa-envelope"></i></a>
    </div>

    <div class="container" id="app-grid"></div>

    <div id="ai-container" style="position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: 10000; background: #0a0a0a; display: none;">
        <canvas id="matrix-canvas" style="position: absolute; top: 0; left: 0; z-index: -1;"></canvas>
        <div style="width: 100%; height: 100%; display: flex; flex-direction: column; background: rgba(10, 10, 10, 0.7); backdrop-filter: blur(5px);">
            <div style="padding: 20px; border-bottom: 1px solid rgba(171, 71, 188, 0.3); display: flex; justify-content: space-between; align-items: center;">
                <div><b id="ai-name-display" style="color: #e1bee7; font-size: 24px;">Rayhan AI</b><div style="font-size: 10px; color: #34a853; font-weight: bold;">● SYSTEM ONLINE</div></div>
                <div onclick="toggleLiveMode()" style="width: 50px; height: 50px; border-radius: 50%; background: rgba(171, 71, 188, 0.2); display: flex; align-items: center; justify-content: center; cursor: pointer; border: 1px solid #ab47bc;">
                    <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#e1bee7" stroke-width="2.5"><path d="M12 2v20M17 6v12M7 6v12M2 11v2M22 11v2"/></svg>
                </div>
            </div>
            <div id="groq-display" style="flex: 1; padding: 20px; overflow-y: auto; display: flex; flex-direction: column; gap: 15px;">
                <div id="ai-welcome-box" style="text-align: center; padding: 25px; background: rgba(106, 27, 154, 0.2); border-radius: 20px; border: 1px solid rgba(171, 71, 188, 0.4); color: #f3e5f5;"></div>
            </div>
            <div style="padding: 20px; display: flex; gap: 10px; background: rgba(0,0,0,0.5); margin-bottom: 80px;">
                <input type="text" id="groq-input" placeholder="Ask AI..." style="flex: 1; padding: 15px; border: 1px solid #ab47bc; border-radius: 30px; background: none; color: #fff; outline: none;">
                <button onclick="askTextAI()" style="background: #6a1b9a; border: none; width: 50px; height: 50px; border-radius: 50%; color: white; cursor: pointer;">🚀</button>
            </div>
        </div>
    </div>

    <div id="call-overlay" style="display:none; position:fixed; top:0; left:0; width:100%; height:100%; background: #000; z-index:20000; flex-direction:column; align-items:center; justify-content:center;">
        <div id="ai-call-name" style="font-size: 26px; color: #e1bee7; margin-bottom: 50px;">AI Calling...</div>
        <div id="wave-container" style="display:flex; gap:12px; height: 70px;">
            <div class="wave-bar" style="width:6px; height:30px; background:#ab47bc;"></div>
            <div class="wave-bar" style="width:6px; height:60px; background:#6a1b9a;"></div>
            <div class="wave-bar" style="width:6px; height:40px; background:#ab47bc;"></div>
            <div class="wave-bar" style="width:6px; height:60px; background:#6a1b9a;"></div>
            <div class="wave-bar" style="width:6px; height:30px; background:#ab47bc;"></div>
        </div>
        <p id="live-transcript" style="margin-top: 40px; color: #ce93d8;">Listening...</p>
        <button onclick="toggleLiveMode()" style="margin-top: 80px; background: #d32f2f; color: white; border: none; padding: 15px 50px; border-radius: 40px;">End Call</button>
    </div>

    <div id="bottom-nav">
        <div class="nav-item" onclick="showHome()"><span>🏠</span>HOME</div>
        <div class="nav-item" onclick="showAI()"><span>🤖</span>Rayhan AI</div>
    </div>

    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script>
        const firebaseConfig = { apiKey: "AIzaSyCyOLdS1MR7nnKUsBjDXpebSUZPJw25NxQ", databaseURL: "https://rayhanzone-964b1-default-rtdb.firebaseio.com", projectId: "rayhanzone-964b1", appId: "1:229256123112:web:529169099fef13d9ccef5d" };
        firebase.initializeApp(firebaseConfig);
        const db = firebase.database().ref('rayhan_data');

        function startExperience() {
            document.getElementById('gate-keeper').style.display = 'none';
            document.getElementById('welcome-screen').style.display = 'flex';
            document.getElementById('welcome-video').play();
            setTimeout(() => document.getElementById('progress').style.width = '100%', 50);
            setTimeout(() => {
                document.getElementById('welcome-screen').style.display = 'none';
                document.body.style.overflow = 'auto';
                document.getElementById('bottom-nav').style.display = 'flex';
            }, 3500);
        }

        db.on('value', (snapshot) => {
            const data = snapshot.val();
            if(!data) return;
            document.getElementById('site-logo').innerText = data.siteName || "Rayhan Zone";
            document.getElementById('dynamic-title').innerText = data.siteName || "Rayhan Zone";
            document.getElementById('marquee-text').innerText = data.marquee || "";
            document.getElementById('hero-img-div').style.backgroundImage = `url('${data.hero}')`;
            document.getElementById('tele-link').href = data.tele.startsWith('@') ? `https://t.me/${data.tele.substring(1)}` : data.tele;
            document.getElementById('insta-link').href = data.insta;
            document.getElementById('mail-link').href = `mailto:${data.email}`;
            document.getElementById('ai-name-display').innerText = data.aiName || "Rayhan AI";
            document.getElementById('ai-call-name').innerText = data.aiName + " Live";
            document.getElementById('ai-welcome-box').innerHTML = `<h3>Welcome to ${data.aiName}</h3><p>${data.aiWelcome || ''}</p>`;

            const grid = document.getElementById('app-grid'); grid.innerHTML = "";
            if(data.apps) {
                data.apps.forEach(app => {
                    let vBtn = app.videoLink ? `<button class="btn btn-video" onclick="window.open('${app.videoLink}')">How to Download?</button>` : '';
                    let showBtn = app.btnShow === 'none' ? 'none' : 'flex';
                    grid.innerHTML += `
                        <div class="card">
                            <img src="${app.pic}">
                            <h3>${app.title}</h3>
                            <p>${app.desc || ''}</p>
                            <div class="btn-group" style="display:${showBtn}">
                                <button class="btn" onclick="window.open('${app.link}')">${app.btnText || 'Access Now'}</button>
                                ${vBtn}
                            </div>
                        </div>`;
                });
            }
        });

        function showHome() { document.getElementById('ai-container').style.display = 'none'; document.body.style.overflow = 'auto'; }
        function showAI() { document.getElementById('ai-container').style.display = 'block'; document.body.style.overflow = 'hidden'; }

        // AI Logic
        const GROQ_KEY = "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";
        async function getGroq(text) {
            const res = await fetch("https://api.groq.com/openai/v1/chat/completions", {
                method: "POST",
                headers: { "Authorization": `Bearer ${GROQ_KEY}`, "Content-Type": "application/json" },
                body: JSON.stringify({ model: "llama-3.3-70b-versatile", messages: [{ role: "user", content: text }] })
            });
            const data = await res.json(); return data.choices[0].message.content;
        }

        async function askTextAI() {
            const input = document.getElementById('groq-input');
            const text = input.value.trim(); if(!text) return;
            const disp = document.getElementById('groq-display');
            disp.innerHTML += `<div style="text-align:right;"><span style="background:#6a1b9a; color:white; padding:10px 15px; border-radius:15px; display:inline-block;">${text}</span></div>`;
            input.value = "";
            const reply = await getGroq(text);
            disp.innerHTML += `<div style="text-align:left;"><span style="background:rgba(171,71,188,0.2); color:#e1bee7; padding:10px 15px; border-radius:15px; display:inline-block; border:1px solid rgba(171,71,188,0.3);">${reply}</span></div>`;
            disp.scrollTop = disp.scrollHeight;
        }

        let isLiveActive = false;
        const recognition = new (window.SpeechRecognition || window.webkitSpeechRecognition)();
        recognition.continuous = true; recognition.lang = 'bn-BD';
        function toggleLiveMode() {
            const overlay = document.getElementById('call-overlay');
            if (!isLiveActive) {
                isLiveActive = true; overlay.style.display = 'flex';
                recognition.start();
            } else {
                isLiveActive = false; overlay.style.display = 'none';
                recognition.stop(); window.speechSynthesis.cancel();
            }
        }
        recognition.onresult = async (e) => {
            const text = e.results[e.results.length - 1][0].transcript;
            document.getElementById('live-transcript').innerText = text;
            const reply = await getGroq(text);
            const utter = new SpeechSynthesisUtterance(reply);
            utter.lang = /[ক-য়]/.test(reply) ? 'bn-BD' : 'en-US';
            window.speechSynthesis.speak(utter);
        };

        // Matrix & Particles
        particlesJS("particles-js", { "particles": { "number": { "value": 40 }, "color": { "value": "#bc13fe" }, "move": { "enable": true, "speed": 2, "direction": "bottom" } } });
        const canvas = document.getElementById('matrix-canvas'); const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth; canvas.height = window.innerHeight;
        const drops = Array(Math.floor(canvas.width/16)).fill(1);
        function drawMatrix() {
            ctx.fillStyle = "rgba(10, 10, 10, 0.1)"; ctx.fillRect(0, 0, canvas.width, canvas.height);
            ctx.fillStyle = "#ab47bc"; ctx.font = "16px monospace";
            drops.forEach((y, i) => {
                ctx.fillText("01"[Math.floor(Math.random()*2)], i*16, y*16);
                if (y*16 > canvas.height && Math.random() > 0.975) drops[i] = 0; drops[i]++;
            });
        }
        setInterval(drawMatrix, 50);
        function applyClickEffect(e) { /* Ripple effect logic here */ }
    </script>
</body>
</html>
