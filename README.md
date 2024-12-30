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
    <title>Crypto Update</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }
        header {
            background-color: #1a1a2e;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background: white;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .crypto-table {
            width: 100%;
            border-collapse: collapse;
        }
        .crypto-table th, .crypto-table td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        .crypto-table th {
            background-color: #4caf50;
            color: white;
        }
        .crypto-table tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #1a1a2e;
            color: white;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Crypto Update</h1>
        <p>Stay updated with the latest cryptocurrency prices</p>
    </header>
    <div class="container">
        <table class="crypto-table">
            <thead>
                <tr>
                    <th>Cryptocurrency</th>
                    <th>Price (USD)</th>
                    <th>24h Change</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Bitcoin (BTC)</td>
                    <td>$26,000</td>
                    <td>+2.3%</td>
                </tr>
                <tr>
                    <td>Ethereum (ETH)</td>
                    <td>$1,800</td>
                    <td>-1.2%</td>
                </tr>
                <tr>
                    <td>Binance Coin (BNB)</td>
                    <td>$245</td>
                    <td>+0.8%</td>
                </tr>
            </tbody>
        </table>
    </div>
    <footer>
        <p>&copy; 2024 Crypto Update. All rights reserved.</p>
    </footer>
</body>
</html>
