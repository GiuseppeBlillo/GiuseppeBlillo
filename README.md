<div align="center">
 
<h3>Look at my Codewars Badge:</h3>
<p>
<a href="https://www.codewars.com/users/JoeBlillo" target="blank"><img align="center" src="https://www.codewars.com/users/JoeBlillo/badges/large" alt="Codewars Lillo" height="50" width="400" /></a>
</p>
</div><br>

<hr><br>
<div>
<img align="left" alt="GIF" width="300" src="https://i.pinimg.com/originals/e4/26/70/e426702edf874b181aced1e2fa5c6cde.gif"/>
  
<div align="right">
<h3>:mag:About Me</h3>
<br>
<p>  I’m a Java Developer Student :computer:</p><br>
<p>  I’m currently attending a Java course on <a href="https://www.develhope.co/"> Develhope</a> :books:</p><br>
<p>  My hobbies are playing videogames and listening music :musical_note:</p><br>
<p>  I'm a gym passionate 💪</p>
<br>


</div>

</div>

<hr>
<br>
<div align="center">
<h3>:wrench:Languages and Tools</h3>
<code><img height="40" src="https://www.vectorlogo.zone/logos/java/java-icon.svg"></code>
<code><img height="40" src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Git_icon.svg"></code>
<code><img height="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg"></code>
<code><img height="40" src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg"></code>
<code><img height="40" src="https://www.vectorlogo.zone/logos/nodejs/nodejs-icon.svg"></code>
<code><img height="40" src="https://upload.wikimedia.org/wikipedia/commons/3/38/HTML5_Badge.svg"></code>
</div>
<br>
<hr>

<br>

<div align="center">
    <head>     
        <style>
        /* Import Google font - Poppins */
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap');
        * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Poppins', sans-serif;
        }
        body {
        display: flex;
        align-items: center;
        justify-content: center;
        min-height: 100vh;
                }
        .wrapper {
        padding: 35px 40px;
        border-radius: 20px;
        background: #141414;
        }
        .wrapper header {
        display: flex;
        color: #B2B2B2;
        align-items: center;
        justify-content: space-between;
        }
        header h2 {
        font-size: 1.6rem;
        }
        header .column {
        display: flex;
        align-items: center;
        }
        header span {
        font-weight: 500;
        margin-right: 15px;
        font-size: 1.19rem;
        }
        header input {
        outline: none;
        border-radius: 30px;
        }
        .volume-slider input {
        accent-color: #fff;
        }
        .keys-checkbox input {
        height: 30px;
        width: 60px;
        cursor: pointer;
        appearance: none;
        position: relative;
        background: #4B4B4B
        }
        .keys-checkbox input::before {
        content: "";
        position: absolute;
        top: 50%;
        left: 5px;
        width: 20px;
        height: 20px;
        border-radius: 50%;
        background: #8c8c8c;
        transform: translateY(-50%);
        transition: all 0.3s ease;
        }
        .keys-checkbox input:checked::before {
        left: 35px;
        background: #fff;
        }
        .piano-keys {
        display: flex;
        list-style: none;
        margin-top: 40px;
        }
        .piano-keys .key {
        cursor: pointer;
        user-select: none;
        position: relative;
        text-transform: uppercase;
        }
        .piano-keys .black {
        z-index: 2;
        width: 44px;
        height: 140px;
        margin: 0 -22px 0 -22px;
        border-radius: 0 0 5px 5px;
        background: linear-gradient(#333, #000);
        }
        .piano-keys .black.active {
        box-shadow: inset -5px -10px 10px rgba(255,255,255,0.1);
        background:linear-gradient(to bottom, #000, #434343);
        }
        .piano-keys .white {
        height: 230px;
        width: 70px;
        border-radius: 8px;
        border: 1px solid #000;
        background: linear-gradient(#fff 96%, #eee 4%);
        }
        .piano-keys .white.active {
        box-shadow: inset -5px 5px 20px rgba(0,0,0,0.2);
        background:linear-gradient(to bottom, #fff 0%, #eee 100%);
        }
        .piano-keys .key span {
        position: absolute;
        bottom: 20px;
        width: 100%;
        color: #A2A2A2;
        font-size: 1.13rem;
        text-align: center;
        }
        .piano-keys .key.hide span {
        display: none;
        }
        .piano-keys .black span {
        bottom: 13px;
        color: #888888;
        }
        @media screen and (max-width: 815px) {
        .wrapper {
            padding: 25px;
        }
        header {
            flex-direction: column;
        }
        header :where(h2, .column) {
            margin-bottom: 13px;
        }
        .volume-slider input {
            max-width: 100px;
        }
        .piano-keys {
            margin-top: 20px;
        }
        .piano-keys .key:where(:nth-child(9), :nth-child(10)) {
            display: none;
        }
        .piano-keys .black {
            height: 100px;
            width: 40px;
            margin: 0 -20px 0 -20px;
        }
        .piano-keys .white {
            height: 180px;
            width: 60px;
        }
        }
        @media screen and (max-width: 615px) {
        .piano-keys .key:nth-child(13),
        .piano-keys .key:nth-child(14),
        .piano-keys .key:nth-child(15),
        .piano-keys .key:nth-child(16),
        .piano-keys .key :nth-child(17) {
            display: none;
        }
        .piano-keys .white {
            width: 50px;
        }
    }
        </style>
    <script>
    const pianoKeys = document.querySelectorAll(".piano-keys .key"),
    volumeSlider = document.querySelector(".volume-slider input"),
    keysCheckbox = document.querySelector(".keys-checkbox input");
    let allKeys = [],
    audio = new Audio(`tunes/a.wav`); // by default, audio src is "a" tune
    const playTune = (key) => {
        audio.src = `tunes/${key}.wav`; // passing audio src based on key pressed 
        audio.play(); // playing audio
        const clickedKey = document.querySelector(`[data-key="${key}"]`); // getting clicked key element
        clickedKey.classList.add("active"); // adding active class to the clicked key element
        setTimeout(() => { // removing active class after 150 ms from the clicked key element
            clickedKey.classList.remove("active");
        }, 150);
    } 
    pianoKeys.forEach(key => {
        allKeys.push(key.dataset.key); // adding data-key value to the allKeys array
        // calling playTune function with passing data-key value as an argument
        key.addEventListener("click", () => playTune(key.dataset.key));
    });
    const handleVolume = (e) => {
        audio.volume = e.target.value; // passing the range slider value as an audio volume
    }
    const showHideKeys = () => {
        // toggling hide class from each key on the checkbox click
        pianoKeys.forEach(key => key.classList.toggle("hide"));
    }
    const pressedKey = (e) => {
        // if the pressed key is in the allKeys array, only call the playTune function
        if(allKeys.includes(e.key)) playTune(e.key);
    }
    keysCheckbox.addEventListener("click", showHideKeys);
    volumeSlider.addEventListener("input", handleVolume);
    document.addEventListener("keydown", pressedKey);
    </script>
</head>
    <body>
            <div class="wrapper">
                <header>
                    <h2>PIANO</h2>
                    <div class="column volume-slider">
                        <span>Volume</span><input type="range" min="0" max="1" value="0.5" step="any">
                    </div>
                    <div class="column keys-checkbox">
                        <span>Keys</span><input type="checkbox" checked>
                    </div>
                </header>
                <ul class="piano-keys">
                    <li class="key white" data-key="a"><span>a</span></li>
                    <li class="key black" data-key="w"><span>w</span></li>
                    <li class="key white" data-key="s"><span>s</span></li>
                    <li class="key black" data-key="e"><span>e</span></li>
                    <li class="key white" data-key="d"><span>d</span></li>
                    <li class="key white" data-key="f"><span>f</span></li>
                    <li class="key black" data-key="t"><span>t</span></li>
                    <li class="key white" data-key="g"><span>g</span></li>
                    <li class="key black" data-key="y"><span>y</span></li>
                    <li class="key white" data-key="h"><span>h</span></li>
                    <li class="key black" data-key="u"><span>u</span></li>
                    <li class="key white" data-key="j"><span>j</span></li>
                    <li class="key white" data-key="k"><span>k</span></li>
                    <li class="key black" data-key="o"><span>o</span></li>
                    <li class="key white" data-key="l"><span>l</span></li>
                    <li class="key black" data-key="p"><span>p</span></li>
                    <li class="key white" data-key=";"><span>;</span></li>
                </ul>
            </div>
    </body>
</div>
