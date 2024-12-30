# ArLink
My first app on AO
Project Name: my-first-app
Branch: main
Install Command: npm ci  # or yarn install
Build Command: npm run build  # or yarn build
Output Directory: dist  # or build
<!DOCTYPE html>
<img src="https://github.com/nekinja/ArLink/commit/0831d23c911bd647c3fef20dcf99acbe9be0a544" alt="v vana" />
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Web Sederhana</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>join wait list now</h1>
    </header>
    <main>
        <p>the next AIdata project on AO</p>
        <button id="alertButton">Klik Saya!</button>
    </main>
    <footer>
        <p>&copy; 2024 Airlinkprohect</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #007BFF;
    color: white;
    padding: 1em 0;
    text-align: center;
}

main {
    padding: 2em;
    text-align: center;
}

button {
    padding: 10px 20px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #218838;
}

footer {
    text-align: center;
    padding: 1em 0;
    background-color: #007BFF;
    color: white;
    position: fixed;
    bottom: 0;
    width: 100%;
}
document.getElementById('alertButton').addEventListener('click', function() {
    alert('Tombol telah diklik!');
});

