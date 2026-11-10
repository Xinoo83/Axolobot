<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>AxolotlBot Controller</title>

<style>
body {
    background: #ffe6f2;
    text-align: center;
    font-family: Arial;
}

button {
    background: #ff99cc;
    border: none;
    padding: 15px 25px;
    margin: 10px;
    border-radius: 20px;
    font-size: 20px;
    color: white;
    cursor: pointer;
}

button:hover {
    background: #ff66b3;
}

#xinoo {
    width: 200px;
    margin: 20px;
}

#status {
    font-size: 20px;
    font-weight: bold;
}
</style>

</head>

<body>

<h1>Robolot</h1>

<p id="status">🔴 Non connecté</p>

<button id="connectBtn">Connecter Xinoo</button>

<br>

<img id="xinoo" src="image/xinoo.jpg" alt="Xinoo">

<br>

<button onclick="sendCommand('z')">Avancer</button>
<br>

<button onclick="sendCommand('q')">Gauche</button>
<button onclick="sendCommand('d')">Droite</button>

<br>

<button onclick="sendCommand('s')">Reculer</button>

<br>

<button onclick="sendCommand('P')">Parler</button>
<button onclick="sendCommand('x')">Stop</button>

<script>

let device, server, service, characteristic;

document.getElementById("connectBtn").onclick = async () => {

    try {

        device = await navigator.bluetooth.requestDevice({
            filters: [{ name: "AxolotlBot" }],
            optionalServices: ["6e400001-b5a3-f393-e0a9-e50e24dcca9e"]
        });

        server = await device.gatt.connect();

        service = await server.getPrimaryService(
            "6e400001-b5a3-f393-e0a9-e50e24dcca9e"
        );

        characteristic = await service.getCharacteristic(
            "6e400002-b5a3-f393-e0a9-e50e24dcca9e"
        );

        document.getElementById("xinoo").src =
            "image/xinooconnecter.jpg";

        document.getElementById("status").innerText =
            "🟢 AxolotlBot connecté";

        document.getElementById("connectBtn").innerText =
            "✅ Connecté";

        alert("AxolotlBot connecté !");

    } catch(error) {

        alert("Erreur : " + error);

    }
};

async function sendCommand(cmd) {

    if (!characteristic) {
        alert("Pas connecté !");
        return;
    }

    await characteristic.writeValue(
        new TextEncoder().encode(cmd)
    );
}

</script>

</body>
</html>
