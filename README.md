# potatowzrd.github.io

<button type="button" onclick="clicked()">Click Seth!</button>

<script>
function clicked() {
    console.log('test');
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
    const ws = new WebSocket('ws://localhost:3000');

    ws.addEventListener('open', () => { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
</script>
