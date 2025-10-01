# potatowzrd.github.io

<button type="button" onclick="clicked()">Click Set2h!</button>

<script>
function clicked() {
    alert("buttone cliecked!");
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
    const ws = new WebSocket('ws://192.168.136.1:3000');

    ws.addEventListener('open', () => { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
</script>
