# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the button, final!</button>

<script>
function clicked() {
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<button type="button" onclick="clicked2()">Click the button, 2!</button>

<script>
function clicked2() {
    ws.send('{\"type\":\"button2\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
    const ws = new WebSocket('wss://strainlessly-transfusive-ahmed.ngrok-free.dev');

    ws.addEventListener('open', () => 
        { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
    
    ws.addEventListener('message', () => 
        { console.log(data);});
</script>
