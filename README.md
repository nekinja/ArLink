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
    <title>AO NFT Marketplace</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        header {
            background-color: #1e1e2f;
            color: white;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        header .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }
        header nav a {
            color: white;
            margin: 0 1rem;
            text-decoration: none;
        }
        header nav a:hover {
            text-decoration: underline;
        }
        .hero {
            text-align: center;
            padding: 4rem 2rem;
            background-color: #3b3b4f;
            color: white;
        }
        .hero h1 {
            font-size: 2.5rem;
        }
        .hero p {
            font-size: 1.2rem;
            margin-top: 1rem;
        }
        .marketplace {
            padding: 2rem;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        .nft-card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.2s;
        }
        .nft-card:hover {
            transform: scale(1.05);
        }
        .nft-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .nft-card .details {
            padding: 1rem;
        }
        .nft-card .details h3 {
            margin: 0;
            font-size: 1.2rem;
        }
        .nft-card .details p {
            margin: 0.5rem 0;
            color: #666;
        }
        .nft-card .details button {
            background-color: #1e1e2f;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            cursor: pointer;
        }
        .nft-card .details button:hover {
            background-color: #333;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #1e1e2f;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">AO NFT Marketplace</div>
        <nav>
            <a href="#">Home</a>
            <a href="#">Marketplace</a>
            <a href="#">About</a>
            <a href="#">Contact</a>
        </nav>
    </header>

    <section class="hero">
        <h1>Welcome to AO NFT Marketplace</h1>
        <p>Discover, collect, and sell extraordinary NFTs.</p>
    </section>

    <section class="marketplace">
        <div class="nft-card">
            <img src="https://via.placeholder.com/300" alt="NFT">
            <div class="details">
                <h3>NFT Title</h3>
                <p>Price: 0.5 ETH</p>
                <button>Buy Now</button>
            </div>
        </div>
        <div class="nft-card">
            <img src="https://via.placeholder.com/300" alt="NFT">
            <div class="details">
                <h3>NFT Title</h3>
                <p>Price: 1.2 ETH</p>
                <button>Buy Now</button>
            </div>
        </div>
        <div class="nft-card">
            <img src="https://via.placeholder.com/300" alt="NFT">
            <div class="details">
                <h3>NFT Title</h3>
                <p>Price: 2.0 ETH</p>
                <button>Buy Now</button>
            </div>
        </div>
    </section>

    <footer>
        &copy; 2024 AO NFT Marketplace. All rights reserved.
    </footer>
</body>
</html>
