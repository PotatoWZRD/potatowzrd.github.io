# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the button, join!</button>

<button type="button" onclick="clicked2()">Click the button, 2!</button>

<script>console.log('00018');</script>

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

<input type="color" value="#ffffff" id="test1">
<input type="color" value="#ffffff" id="test2">

<!-- yin yang -->
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

<circle cx="65.5" cy="128" r="31.25" stroke="black" stroke-width="2" fill="white" id="topC"/>

<circle cx="190.5" cy="128" r="31.25" stroke="black" stroke-width="2" fill="white" id="botC"/>
</svg>

<!-- blank circle --> 
<svg width="256" height="256" viewBox="0 0 256 256">
    <circle cx="128" cy="128" r="125" stroke="black" stroke-width="2" fill="white" id="topC"/>
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
</svg>

<script>
let des1 = document.getElementById('topC')
let col1 = document.getElementById('test1')
    col1.addEventListener('input', (event) => {
        des1.style.fill = event.target.value;
    })
let des2 = document.getElementById('botC');
let col2 = document.getElementById('test2');
    col2.addEventListener('input', (event) => {
        des2.style.fill = event.target.value;
    })
</script>  
