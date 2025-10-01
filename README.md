# potatowzrd.github.io

<button type="button" onclick="clicked()">Click Me!</button>

<script>
function clicked() {
  alert("Hello! I am an alert box!");
}
</script>

<script>
    const ws = new WebSocket('ws://localhost:3000');

    ws.addEventListener('open', () => {
        console.log('Connected to WebSocket server');
        ws.send('Hello from the client!');
    });

    ws.addEventListener('message', () => {
        console.log('got it');
    });
</script>
