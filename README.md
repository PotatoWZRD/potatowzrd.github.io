# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the butweton, we!</button>

<script>
function clicked() {
    alert("buttone cliecked!");
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
    const ws = new WebSocket('ws:///127.0.0.1:4040/');

    ws.addEventListener('open', () => { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
</script>
