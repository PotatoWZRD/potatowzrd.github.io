# potatowzrd.github.io

<button type="button" onclick="clicked()">Click Me!</button>

<script>
function clicked() {
    ws.addEventListener('message', () => {
        console.log('got it');
    });
}
</script>

<script>
    const ws = new WebSocket('ws://localhost:3000');


    ws.addEventListener('message', () => {
        console.log('got it');
    });
</script>
