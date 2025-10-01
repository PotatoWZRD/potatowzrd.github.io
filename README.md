# potatowzrd.github.io

<button type="button" onclick="clicked()">Click Me!</button>

<script>
function clicked() {
    ws.send("got it");
}
</script>

<script>
    const ws = new WebSocket('ws://localhost:3000');

    ws.addEventListener('open', () => { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
</script>
