# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the button, join!</button>

<button type="button" onclick="clicked2()">Click the button, 2!</button>

<script>console.log('00035');</script>

<script>
    const ws = new WebSocket('wss://strainlessly-transfusive-ahmed.ngrok-free.dev');

    ws.addEventListener('open', () => 
        { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
    
    ws.addEventListener('message', (event) => 
        { console.log(event.data);});
</script>

<script>
function clicked() {
    console.log('button clickwed');
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
function clicked2() {
    console.log('second buttonr');
    ws.send('{\"type\":\"button2\",\"client\":\"abrahma\"}'); 
};
</script>

<h1>Marble Name Generator</h1>

<button type="button" onclick="nameGen()">Name!</button>

<script>

function nameGen()
{
var fNames = Array("Red", "Orange", "Yellow", "Green", "Blue", "Purple", "Pink", "White", "Black", "Brown", "Gold", "Silver", "Bronze", "Copper", "Platinum", "Glass", "Metal", "Paper", "Plastic", "Wooden", "Hot", "Wet", "Windy", "Stinky", "Electric", "Salty", "Sour", "Sweet", "Savory", "Bitter", "Lavender", "Olive", "Huge", "Tiny", "Average", "Happy", "Sad", "Angry", "Lovely", "Devious", "Fancy", "Cursed", "Special", "Glitchy", "Shiny", "Bouncy", "Heavy", "Light", "Dark", "Coral", "Empty", "Single", "Double", "Triple", "Super", "Lucky", "Retro", "Neon", "Cute", "The", "Slow", "Fast", "Still", "Strong", "Weak", "Summer", "Winter", "Spring", "Fall", "Pretty", "Deadly", "Killer", "Agent", "Doctor", "Clear", "Digital", "Bloody", "Funny", "Rich", "Poor", "Good", "Evil", "Imaginary", "Impossible", "Actual", "Video", "Inch", "Final", "Mozzarella", "Marble", "Spicy", "Radioactive", "Jovial", "Innocent", "Mega", "Jazzy", "Crazy", "Free", "Clover", "Potato");

var fname = fNames[Math.floor(Math.random() * fNames.length)];
document.getElementById('fname').innerHTML = fname;

var sNames = Array("Red", "Orange", "Yellow", "Green", "Blue", "Purple", "Pink", "White", "Black", "Brown", "Gold", "Silver", "Bronze", "Copper", "Platinum", "Diamond", "Emerald", "Ruby", "Crystal", "Obsidian", "Rice", "Bread", "Cookie", "Cake", "Pasta", "Dog", "Cat", "Snail", "Fox", "Horse", "Bird", "Fish", "Ant", "Lion", "Spider", "Rain", "Tornado", "Tsunami", "Cloud", "Hurricane", "Pirate", "Ninja", "Wizard", "Samurai", "Robot", "Apple", "Banana", "Grape", "Cherry", "Lemon", "Dream", "Moon", "Sun", "Comet", "Sky", "Mushroom", "Flower", "Rock", "Tree", "Seed", "Angel", "Devil", "Unicorn", "Dragon", "Fairy", "Barbeque", "Pickle", "Mustard", "Mayo", "Ketchup", "Vanilla", "Chocolate", "Mint", "Sprinkle", "Stardust", "King", "Queen", "Royal", "Ballad", "Jester", "Honey", "Waffle", "Soup", "Egg", "Sandwich", "Heart", "Bone", "Gamble", "Soul", "Mania", "Nerd", "Comrade", "Trash", "Panic", "Snake", "Bullet", "Butter", "Pizza", "Sock", "Bee");

var sname = sNames[Math.floor(Math.random() * sNames.length)];
document.getElementById('sname').innerHTML = sname;
}

</script>

<span id="fname"></span>
<span id="sname"></span>

<input type="color" value="#ffffff" id="color1">
<input type="color" value="#ffffff" id="color2">
<input type="color" value="#ffffff" id="color3">

<!-- blank circle --> 
<svg width="256" height="256" viewBox="0 0 256 256">
    <circle cx="128" cy="128" r="125" stroke="none" stroke-width="0.5" fill="white" id="marble"/>
    <circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- yin yang -->
<svg width="256" height="256" viewBox="0 0 256 256">
  <path
    d="
      M 128 253
      A 125 125 0 0 1 128 3
      A 62.5 62.5 0 0 1 128 128
      A 62.5 62.5 1 0 0 128 253
      "
    fill= "black"
    id="yy1"
    stroke="none"
    stroke-width="0.5"
  />
   <path
    d="
      M 128 3
      A 125 125 0 0 1 128 253
      A 62.5 62.5 0 0 1 128 128
      A 62.5 62.5 1 0 0 128 3
      "
    fill= "white"
    id="yy2"
    stroke="none"
    stroke-width="0.5"
  />

<circle cx="128" cy="190.5" r="25" stroke="none" stroke-width="2" fill="black" id="yy3"/>
<circle cx="128" cy="65.5" r="25" stroke="none" stroke-width="2" fill="white" id="yy4"/>

<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- classic swirl marble -->
<svg width="256" height="256" viewBox="0 0 256 256">
  <path
    d="
      M 155.06329 112.375
      A 1 1 0 0 0 19.74682 190.5
      A 1 1 0 0 1 236.25318 65.5
      A 1 1 0 0 1 155.06329 112.375
      "
    fill= "white"
    id="m1"
    stroke="none"
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
    fill= "grey"
    id="m2"
    stroke="none"
    stroke-width="0.5"
  />
  
  <path
    d="
      M 100.93671 143.625
      A 1 1 0 0 0 236.25318 65.5
      A 1 1 0 0 1 19.74682 190.5
      A 1 1 0 0 1 100.93671 143.625
      "
    fill= "black"
    id="m3"
    stroke="none"
    stroke-width="0.5"
  />
  
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- smile --> 
<svg width="256" height="256" viewBox="0 0 256 256">
    
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
<svg width="256" height="256" viewBox="0 0 256 256">

<circle cx="128" cy="128" r="125" stroke="none" stroke-width="0.5" fill="black" id="s1"/>

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
fill="white"
id="s2"
stroke="white"
stroke-width="0.5"
/>

<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- cross --> 
<svg width="256" height="256" viewBox="0 0 256 256">

<circle cx="128" cy="128" r="125" stroke="none" stroke-width="0.5" fill="white" id="c1"/>

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
<svg width="256" height="256" viewBox="0 0 256 256">

<circle cx="128" cy="128" r="125" stroke="none" stroke-width="0.5" fill="white" id="p1"/>

  <path
    d="
      M 174.875 243.8781
      Q 118 222 100.71927 159.25
      L 159.25 128
      L 100.71929 96.75
      Q 118 34 174.875 12.1219
      C 280 60 280 200 174.875 243.8781
      "
    fill= "grey"
    id="p2"
    stroke="grey"
    stroke-width="0.5"
  />
  <path
    d="
      M 174.875 96.75
      A 0.5 1 0 0 1 174.875 49.875
      A 0.5 1 0 0 1 174.875 96.75
      "
    fill= "black"
    id="p3"
    stroke="black"
    stroke-width="0.5"
  />
  <path
    d="
      M 65.5 96.75
      A 0.5 1 0 0 1 65.5 49.875
      A 0.5 1 0 0 1 65.5 96.75
      "
    fill= "black"
    id="p4"
    stroke="black"
    stroke-width="0.5"
  />
  
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- donut --> 
<svg width="256" height="256" viewBox="0 0 256 256">
    <circle cx="128" cy="128" r="125" stroke="none" stroke-width="0.5" fill="black" id="d1"/>
    <circle cx="128" cy="128" r="50" stroke="none" stroke-width="0.5" fill="white" id="hole"/>
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

        desA1.style.stroke = event.target.value;
        desA2.style.stroke = event.target.value;
        desA3.style.stroke = event.target.value;
        desA4.style.stroke = event.target.value;
        desA5.style.stroke = event.target.value;
        desA6.style.stroke = event.target.value;
        desA7.style.stroke = event.target.value;
        desA8.style.stroke = event.target.value;
        desA9.style.stroke = event.target.value;
    })
let col2 = document.getElementById('color2');
let desB1 = document.getElementById('botC');
let desB2 = document.getElementById('yy2');
let desB3 = document.getElementById('yy4');
let desB4 = document.getElementById('m2');
let desB5 = document.getElementById('h2');
let desB6 = document.getElementById('h3');
let desB7 = document.getElementById('h4');
let desB8 = document.getElementById('s2');
let desB9 = document.getElementById('c2');
let desB10 = document.getElementById('p2');
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
