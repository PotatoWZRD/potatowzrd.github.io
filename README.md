# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the button, fun!</button>

<button type="button" onclick="clicked2()">Click the button, 2!</button>

<script>
    const ws = new WebSocket('wss://strainlessly-transfusive-ahmed.ngrok-free.dev');

    ws.addEventListener('open', () => 
        { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
    
    ws.addEventListener('message', (event) => 
        { console.log(event.data);});
</script>

<script>
function clicked() {
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
function clicked2() {
    ws.send('{\"type\":\"button2\",\"client\":\"abrahma\"}'); 
};
</script>

