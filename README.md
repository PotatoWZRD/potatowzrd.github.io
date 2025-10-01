# potatowzrd.github.io

<button type="button" onclick="clicked()">Click the button, 432!</button>

<script>
function clicked() {
    alert("buttone cliecked!");
    ws.send('{\"type\":\"button\",\"client\":\"abrahma\"}'); 
};
</script>

<script>
    const ws = new WebSocket('"ws://yummy-parks-relate.loca.lt/"');

    ws.addEventListener('open', () => { console.log('Connected to WebSocket server'); ws.send('{\"type\":\"connect\",\"client\":\"client\"}'); });
</script>
