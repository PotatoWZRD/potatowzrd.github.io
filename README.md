# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the bgfutweton, we!</button>

<script>
function clicked() {
    alert("buttone cliecked!");
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
    const ws = new WebSocket('wss://strainlessly-transfusive-ahmed.ngrok-free.dev');

    ws.addEventListener('open', () => { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
</script>
