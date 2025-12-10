# potatowzrd.github.io

<script>
    console.log('00060');
</script>

<script>
function nameGen()
{
    var fNames = Array("Red", "Orange", "Yellow", "Green", "Blue", "Purple", "Pink", "White", "Black", "Brown", "Gold", "Silver", "Bronze", "Copper", "Platinum", "Glass", "Metal", "Paper", "Plastic", "Wooden", "Hot", "Wet", "Windy", "Stinky", "Electric", "Salty", "Sour", "Sweet", "Savory", "Bitter", "Lavender", "Olive", "Huge", "Tiny", "Average", "Happy", "Sad", "Angry", "Lovely", "Devious", "Fancy", "Cursed", "Special", "Glitchy", "Shiny", "Bouncy", "Heavy", "Light", "Dark", "Coral", "Empty", "Single", "Double", "Triple", "Super", "Lucky", "Retro", "Neon", "Cute", "The", "Slow", "Fast", "Still", "Strong", "Weak", "Summer", "Winter", "Spring", "Fall", "Pretty", "Deadly", "Killer", "Agent", "Doctor", "Clear", "Digital", "Bloody", "Funny", "Rich", "Poor", "Good", "Evil", "Imaginary", "Impossible", "Actual", "Video", "Inch", "Final", "Mozzarella", "Marble", "Spicy", "Radioactive", "Jovial", "Innocent", "Mega", "Jazzy", "Crazy", "Free", "Clover", "Potato", "Squishy", "Maximum");
    
    var sNames = Array("Red", "Orange", "Yellow", "Green", "Blue", "Purple", "Pink", "White", "Black", "Brown", "Gold", "Silver", "Bronze", "Copper", "Platinum", "Diamond", "Emerald", "Ruby", "Crystal", "Obsidian", "Rice", "Bread", "Cookie", "Cake", "Pasta", "Dog", "Cat", "Snail", "Fox", "Horse", "Bird", "Fish", "Ant", "Lion", "Spider", "Rain", "Tornado", "Tsunami", "Cloud", "Hurricane", "Pirate", "Ninja", "Wizard", "Samurai", "Robot", "Apple", "Banana", "Grape", "Cherry", "Lemon", "Dream", "Moon", "Sun", "Comet", "Sky", "Mushroom", "Flower", "Rock", "Tree", "Seed", "Angel", "Devil", "Unicorn", "Dragon", "Fairy", "Barbeque", "Pickle", "Mustard", "Mayo", "Ketchup", "Vanilla", "Chocolate", "Mint", "Sprinkle", "Stardust", "King", "Queen", "Royal", "Ballad", "Jester", "Honey", "Waffle", "Soup", "Egg", "Sandwich", "Heart", "Bone", "Gamble", "Soul", "Mania", "Nerd", "Comrade", "Trash", "Panic", "Snake", "Bullet", "Butter", "Pizza", "Sock", "Bee", "Seagull");
    
    var fname = fNames[Math.floor(Math.random() * fNames.length)];
    var sname = sNames[Math.floor(Math.random() * sNames.length)];
    var finalName = fname + " " + sname;
    document.getElementById('finalName').innerHTML = finalName;
}
</script>

<h1>Marble Generator</h1>

<button type="button" onclick="nameGen()">Reroll Name</button>

<span id="finalName"></span>

<script>
    nameGen();
</script>

<script>
    const ws = new WebSocket('wss://strainlessly-transfusive-ahmed.ngrok-free.dev');

    ws.addEventListener('open', () => 
        { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
    
    ws.addEventListener('message', (event) => 
        { console.log(event.data);});
</script>

<input type="color" value="#ffffff" id="color1">
<input type="color" value="#000000" id="color2">
<input type="color" value="#808080" id="color3">

<p>Choose Your Template</p>

<select id="templates">
    <option>Basic</option>
    <option>Yin Yang</option>
    <option>Swirl</option>
    <option>Happy</option>
    <option>Star</option>
    <option>Cross</option>
    <option>Sun & Moon</option>
    <option>Donut</option>
    <option>Cowprint</option>
</select>

<button type="button" style="width:200px;height:100px;" onclick="joinClick()">JOIN!</button>

<button type="button" style="width:200px;height:100px;" onclick="clickedf()">JUMP!</button>

<!-- data to send when joining -->
<script>
function joinClick() {
    console.log('button clicked');

    var name = document.getElementById('finalName').innerText;
    var design = document.getElementById('templates').value;
    var c1 = document.getElementById('color1').value;
    var c2 = document.getElementById('color2').value;
    var c3 = document.getElementById('color3').value;
    ws.send('{\"type\":\"button\",\"client\":\"butter\", \"name\":\"'+name+'\", \"design\":\"'+design+'\", \"color1\":\"'+c1+'\", \"color2\":\"'+c2+'\", \"color3\":\"'+c3+'\"}');   
    console.log('{\"type\":\"button\",\"client\":\"butter\", \"name\":\"'+name+'\", \"design\":\"'+design+'\", \"color1\":\"'+c1+'\", \"color2\":\"'+c2+'\", \"color3\":\"'+c3+'\"}');   
};
</script>

<script>
function clickedf() {
    console.log('fire button');
    ws.send('{\"type\":\"button2\",\"client\":\"butter\"}'); 
};
</script>
<script>
function clickeds() {
    console.log('sword button');
    ws.send('{\"type\":\"button3\",\"client\":\"butter\"}'); 
};
</script>
<script>
function clickedb() {
    console.log('bomb button');
    ws.send('{\"type\":\"button4\",\"client\":\"butter\"}'); 
};
</script>

<!-- blank circle --> 
<svg width="128" height="128" viewBox="0 0 256 256">
    <circle cx="128" cy="128" r="125" stroke="white" stroke-width="0.5" fill="white" id="marble"/>
    <circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- yin yang -->
<svg width="128" height="128" viewBox="0 0 256 256">
  <path
    d="
      M 128 253
      A 125 125 0 0 1 128 3
      A 62.5 62.5 0 0 1 128 128
      A 62.5 62.5 1 0 0 128 253
      "
    fill= "white"
    id="yy1"
    stroke="white"
    stroke-width="0.5"
  />
   <path
    d="
      M 128 3
      A 125 125 0 0 1 128 253
      A 62.5 62.5 0 0 1 128 128
      A 62.5 62.5 1 0 0 128 3
      "
    fill= "black"
    id="yy2"
    stroke="black"
    stroke-width="0.5"
  />

<circle cx="128" cy="190.5" r="25" stroke="white" stroke-width="2" fill="white" id="yy3"/>
<circle cx="128" cy="65.5" r="25" stroke="black" stroke-width="2" fill="black" id="yy4"/>

<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- classic swirl marble -->
<svg width="128" height="128" viewBox="0 0 256 256">
  <path
    d="
      M 155.06329 112.375
      A 1 1 0 0 0 19.74682 190.5
      A 1 1 0 0 1 236.25318 65.5
      A 1 1 0 0 1 155.06329 112.375
      "
    fill= "white"
    id="m1"
    stroke="white"
    stroke-width="0.5"
  />
    
  <path
    d="
      M 100.93671 143.625
      A 1 1 0 0 0 236.25318 65.5
      A 1 1 0 0 1 155.06329 112.375
      A 1 1 0 0 0 19.74682 190.5
      A 1 1 0 0 1 100.93671 143.625
      "
    fill= "black"
    id="m2"
    stroke="black"
    stroke-width="0.5"
  />
  
  <path
    d="
      M 100.93671 143.625
      A 1 1 0 0 0 236.25318 65.5
      A 1 1 0 0 1 19.74682 190.5
      A 1 1 0 0 1 100.93671 143.625
      "
    fill= "grey"
    id="m3"
    stroke="grey"
    stroke-width="0.5"
  />
  
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- smile --> 
<svg width="128" height="128" viewBox="0 0 256 256">
    
<circle cx="128" cy="128" r="125" stroke="none" stroke-width="0.5" fill="white" id="h1"/>
    
  <path
    d="
      M 88.9375 112.375
      A 0.5 1 0 0 1 88.9375 49.875
      A 0.5 1 0 0 1 88.9375 112.375
      "
    fill= "black"
    id="h2"
    stroke="black"
    stroke-width="0.5"
  />
  <path
    d="
      M 167.0625 112.375
      A 0.5 1 0 0 1 167.0625 49.875
      A 0.5 1 0 0 1 167.0625 112.375
      "
    fill= "black"
    id="h3"
    stroke="black"
    stroke-width="0.5"
  />
  <path
    d="
      M 49.875 143.625
      A 1 0.35 0 0 0 206.125 143.625
      A 1 1 0 0 1 49.875 143.625
      "
    fill= "black"
    id="h4"
    stroke="black"
    stroke-width="0.5"
  />
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- star --> 
<svg width="128" height="128" viewBox="0 0 256 256">

<circle cx="128" cy="128" r="125" stroke="white" stroke-width="0.5" fill="white" id="s1"/>

<path
    d="
        M 128 3
        L 156.06425 87.37288
        L 246.88206 87.37288
        L 173.40891 142.75425
        L 201.47316 228.12712
        L 128 175.74575
        L 54.52684 228.12712
        L 82.59109 142.75425
        L 9.11794 87.37288
        L 99.93575 87.37288
        L 128 3
    "     
fill="black"
id="s2"
stroke="black"
stroke-width="0.5"
/>

<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- cross --> 
<svg width="128" height="128" viewBox="0 0 256 256">

<circle cx="128" cy="128" r="125" stroke="white" stroke-width="0.5" fill="white" id="c1"/>

  <path
    d="
      M 159.25 249.03073
      L 159.25 159.25
      L 249.03073 159.25
      A 1 10 0 0 0 249.03073 96.75
      L 159.25 96.75
      L 159.25 6.96927
      A 10 1 0 0 0 96.75 6.96927
      L 96.75 96.75
      L 6.96927 96.75
      A 1 10 0 0 0 6.96927 159.25
      L 96.75 159.25
      L 96.75 249.03073
      A 10 1 0 0 0 159.25 249.03073
      "
    fill= "black"
    id="c2"
    stroke="black"
    stroke-width="0.5"
  />
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- sun&moon --> 
<svg width="128" height="128" viewBox="0 0 256 256">

<circle cx="128" cy="128" r="125" stroke="white" stroke-width="0.5" fill="white" id="p1"/>

  <path
    d="
      M 174.875 243.8781
      Q 118 222 100.71927 159.25
      L 159.25 128
      L 100.71929 96.75
      Q 118 34 174.875 12.1219
      C 280 60 280 200 174.875 243.8781
      "
    fill= "black"
    id="p2"
    stroke="black"
    stroke-width="0.5"
  />
  <path
    d="
      M 174.875 96.75
      A 0.5 1 0 0 1 174.875 49.875
      A 0.5 1 0 0 1 174.875 96.75
      "
    fill= "grey"
    id="p3"
    stroke="grey"
    stroke-width="0.5"
  />
  <path
    d="
      M 65.5 96.75
      A 0.5 1 0 0 1 65.5 49.875
      A 0.5 1 0 0 1 65.5 96.75
      "
    fill= "grey"
    id="p4"
    stroke="grey"
    stroke-width="0.5"
  />
  
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- donut --> 
<svg width="128" height="128" viewBox="0 0 256 256">
<circle cx="128" cy="128" r="125" stroke="white" stroke-width="0.5" fill="white" id="d1"/>
<circle cx="128" cy="128" r="50" stroke="black" stroke-width="2" fill="white" id="hole"/>
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- mushroom --> 
<svg width="128" height="128" viewBox="0 0 256 256">

<circle cx="128" cy="128" r="125" stroke="white" stroke-width="0.5" fill="white" id="j1"/>

  <path
    d="
      M 7.1 95.5
      C 27.6 103.5 18.6 85.6 35.8 84.5
      C 57.2 83.2 48 103.3 68.8 96.6
      C 92.9 81.2 56.5 66.5 83 44.4
      C 92 36 111.9 39.7 118.6 28.3
      C 125 16 126 3 114 3.78467
      C 63 6 15 56 7.1 95.5
      "
    fill= "black"
    id="j2"
    stroke="black"
    stroke-width="0.5"
  />

  <path
    d="
      M 3.69 141.11749
      C 2.3 136.2 9.4 148.7 20 146
      C 31.8 144.5 40.3 127.9 55.3 136.5
      C 69.8 147 55.3 161.7 68 180
      C 75 194.6 97 188 100 207
      C 100 220 94 239 83 244.61904
      C 40 230 3 177 3.69 141.11749
      "
    fill= "black"
    id="j3"
    stroke="black"
    stroke-width="0.5"
  />
  
  <path
    d="
      M 170 245.73275 
      Q 182 182 235 192.62198
      Q 206 235 170 245.73275
      "
    fill= "black"
    id="j4"
    stroke="black"
    stroke-width="0.5"
  />
  
  <path
    d="
      M 118 148
      C 93.7 128 116.6 124 127 120
      C 147.5 108.5 133 94.5 146 89
      C 175.7 83.4 153 104.7 180 125
      C 192.5 136 204.5 136.4 200 148
      C 188 171.2 171.4 149.8 155 150
      C 133 158 133 155 118 148
      "
    fill= "black"
    id="j5"
    stroke="black"
    stroke-width="0.5"
  />
  
  <path
    d="
      M 220 92
      C 202 81 215 71 201 53
      C 193 39 165 41 163 27
      Q 160 16 171 10.62879
      C 203 18 243 65 245 84
      Q 242.4 96.1 220 92
      "
    fill= "black"
    id="j6"
    stroke="black"
    stroke-width="0.5"
  />
  
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<script>
let col1 = document.getElementById('color1');
let desA1 = document.getElementById('marble');
let desA2 = document.getElementById('yy1');
let desA3 = document.getElementById('yy3');
let desA4 = document.getElementById('m1');
let desA5 = document.getElementById('h1');
let desA6 = document.getElementById('s1');
let desA7 = document.getElementById('c1');
let desA8 = document.getElementById('p1');
let desA9 = document.getElementById('d1');
let desA10 = document.getElementById('j1');
    col1.addEventListener('input', (event) => {
        desA1.style.fill = event.target.value;
        desA2.style.fill = event.target.value;
        desA3.style.fill = event.target.value;
        desA4.style.fill = event.target.value;
        desA5.style.fill = event.target.value;
        desA6.style.fill = event.target.value;
        desA7.style.fill = event.target.value;
        desA8.style.fill = event.target.value;
        desA9.style.fill = event.target.value;
        desA10.style.fill = event.target.value;

        desA1.style.stroke = event.target.value;
        desA2.style.stroke = event.target.value;
        desA3.style.stroke = event.target.value;
        desA4.style.stroke = event.target.value;
        desA5.style.stroke = event.target.value;
        desA6.style.stroke = event.target.value;
        desA7.style.stroke = event.target.value;
        desA8.style.stroke = event.target.value;
        desA9.style.stroke = event.target.value;
        desA10.style.stroke = event.target.value;
    })
let col2 = document.getElementById('color2');
let desB1 = document.getElementById('p2');
let desB2 = document.getElementById('yy2');
let desB3 = document.getElementById('yy4');
let desB4 = document.getElementById('m2');
let desB5 = document.getElementById('h2');
let desB6 = document.getElementById('h3');
let desB7 = document.getElementById('h4');
let desB8 = document.getElementById('s2');
let desB9 = document.getElementById('c2');
let desB10 = document.getElementById('j2');
let desB11 = document.getElementById('j3');
let desB12 = document.getElementById('j4');
let desB13 = document.getElementById('j5');
let desB14 = document.getElementById('j6');
    col2.addEventListener('input', (event) => {
        desB1.style.fill = event.target.value;
        desB2.style.fill = event.target.value;
        desB3.style.fill = event.target.value;
        desB4.style.fill = event.target.value;
        desB5.style.fill = event.target.value;
        desB6.style.fill = event.target.value;
        desB7.style.fill = event.target.value;
        desB8.style.fill = event.target.value;
        desB9.style.fill = event.target.value;
        desB10.style.fill = event.target.value;
        desB11.style.fill = event.target.value;
        desB12.style.fill = event.target.value;
        desB13.style.fill = event.target.value;
        desB14.style.fill = event.target.value;
        
        desB1.style.stroke = event.target.value;
        desB2.style.stroke = event.target.value;
        desB3.style.stroke = event.target.value;
        desB4.style.stroke = event.target.value;
        desB5.style.stroke = event.target.value;
        desB6.style.stroke = event.target.value;
        desB7.style.stroke = event.target.value;
        desB8.style.stroke = event.target.value;
        desB9.style.stroke = event.target.value;
        desB10.style.stroke = event.target.value;
        desB11.style.stroke = event.target.value;
        desB12.style.stroke = event.target.value;
        desB13.style.stroke = event.target.value;
        desB14.style.stroke = event.target.value;
    })
let col3 = document.getElementById('color3');
let desC1 = document.getElementById('m3');
let desC2 = document.getElementById('p3');
let desC3 = document.getElementById('p4');
    col3.addEventListener('input', (event) => {
        desC1.style.fill = event.target.value;
        desC2.style.fill = event.target.value;
        desC3.style.fill = event.target.value;
        
        desC1.style.stroke = event.target.value;
        desC2.style.stroke = event.target.value;
        desC3.style.stroke = event.target.value;
    })
</script>
