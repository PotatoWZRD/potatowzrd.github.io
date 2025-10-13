# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the button, join!</button>

<button type="button" onclick="clicked2()">Click the button, 2!</button>

<script>console.log('00028');</script>

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
    <circle cx="128" cy="128" r="125" stroke="none" stroke-width="2" fill="white" id="marble"/>
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
    stroke-width="2"
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
    stroke-width="2"
  />

<circle cx="128" cy="190.5" r="25" stroke="none" stroke-width="2" fill="black" id="yy3"/>
<circle cx="128" cy="65.5" r="25" stroke="none" stroke-width="2" fill="white" id="yy4"/>

<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- classic swirl marble -->
<svg width="256" height="256" viewBox="0 0 256 256">
  <path
    d="
      M 100.93671 143.625
      A 1 1 0 0 0 236.25318 65.5
      A 1 1 0 0 1 155.06329 112.375
      A 1 1 0 0 0 19.74682 190.5
      A 1 1 0 0 1 100.93671 143.625
      "
    fill= "pink"
    id="m1"
    stroke="none"
    stroke-width="2"
  />
  
  <path
    d="
      M 100.93671 143.625
      A 1 1 0 0 0 236.25318 65.5
      A 1 1 0 0 1 19.74682 190.5
      A 1 1 0 0 1 100.93671 143.625
      "
    fill= "orange"
    id="m2"
    stroke="none"
    stroke-width="2"
  />
  
  <path
    d="
      M 155.06329 112.375
      A 1 1 0 0 0 19.74682 190.5
      A 1 1 0 0 1 236.25318 65.5
      A 1 1 0 0 1 155.06329 112.375
      "
    fill= "purple"
    id="m3"
    stroke="none"
    stroke-width="2"
  />
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<!-- blank circle --> 
<svg width="256" height="256" viewBox="0 0 256 256">
  <path
    d="
      M 253 128
      A 125 125 0 0 1 3 128
      A 62.5 62.5 0 0 1 128 128
      A 62.5 62.5 1 0 0 253 128
      "
    fill= "white"
    id="topC"
    stroke="black"
    stroke-width="2"
  />
   <path
    d="
      M 3 128
      A 125 125 0 0 1 253 128
      A 62.5 62.5 0 0 1 128 128
      A 62.5 62.5 1 0 0 3 128
      "
    fill= "white"
    id="botC"
    stroke="black"
    stroke-width="2"
  />
<circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="none" id="outline"/>
</svg>

<script>
let col1 = document.getElementById('color1')
let desA1 = document.getElementById('marble')
let desA2 = document.getElementById('yy1')
let desA3 = document.getElementById('yy3')
let desA4 = document.getElementById('m1')
    col1.addEventListener('input', (event) => {
        desA1.style.fill = event.target.value;
        desA2.style.fill = event.target.value;
        desA3.style.fill = event.target.value;
        desA4.style.fill = event.target.value;
    })
let col2 = document.getElementById('color2');
let desB1 = document.getElementById('botC');
let desB2 = document.getElementById('yy2')
let desB3 = document.getElementById('yy4')
let desB4 = document.getElementById('m2')
    col2.addEventListener('input', (event) => {
        desB1.style.fill = event.target.value;
        desB2.style.fill = event.target.value;
        desB3.style.fill = event.target.value;
        desB4.style.fill = event.target.value;
    })
let col3 = document.getElementById('color3');
let desC1 = document.getElementById('m3');
    col3.addEventListener('input', (event) => {
        desC1.style.fill = event.target.value;
    })
</script>  
