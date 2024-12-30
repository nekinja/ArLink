Project Name: my-first-app
Branch: main
Install Command: npm ci  # or yarn install
Build Command: npm run build  # or yarn build
Output Directory: dist  # or build
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Crypto Analyst Dashboard</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #ffffff;
        }

        header {
            background-color: #1e88e5;
            padding: 1rem;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 2rem;
        }

        main {
            padding: 2rem;
        }

        .crypto-card {
            background-color: #1f1f1f;
            border: 1px solid #333;
            border-radius: 8px;
            padding: 1rem;
            margin-bottom: 1rem;
        }

        .crypto-card h2 {
            margin: 0 0 0.5rem;
        }

        .crypto-card .price {
            font-size: 1.5rem;
            color: #4caf50;
        }

        .crypto-card .change {
            font-size: 1.2rem;
        }

        footer {
            text-align: center;
            padding: 1rem;
            background-color: #1e88e5;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Crypto Analyst Dashboard</h1>
    </header>

    <main>
        <div id="crypto-container">
            <div class="crypto-card">
                <h2>Bitcoin (BTC)</h2>
                <p class="price" id="btc-price">$0.00</p>
                <p class="change" id="btc-change">Change: 0%</p>
            </div>

            <div class="crypto-card">
                <h2>Ethereum (ETH)</h2>
                <p class="price" id="eth-price">$0.00</p>
                <p class="change" id="eth-change">Change: 0%</p>
            </div>
        </div>
    </main>

    <footer>
        <p>Crypto Analyst &copy; 2024</p>
    </footer>

    <script>
        async function fetchCryptoData() {
            const apiUrl = "https://api.coingecko.com/api/v3/simple/price?ids=bitcoin,ethereum&vs_currencies=usd&include_24hr_change=true";
            try {
                const response = await fetch(apiUrl);
                const data = await response.json();

                document.getElementById('btc-price').textContent = `$${data.bitcoin.usd}`;
                document.getElementById('btc-change').textContent = `Change: ${data.bitcoin.usd_24h_change.toFixed(2)}%`;

                document.getElementById('eth-price').textContent = `$${data.ethereum.usd}`;
                document.getElementById('eth-change').textContent = `Change: ${data.ethereum.usd_24h_change.toFixed(2)}%`;
            } catch (error) {
                console.error("Error fetching crypto data:", error);
            }
        }

        // Fetch data on page load and refresh every 60 seconds
        fetchCryptoData();
        setInterval(fetchCryptoData, 60000);
    </script>
</body>
</html>
