<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Memory Vault - Custom Printing</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #222;
            color: #fff;
            text-align: center;
            padding: 50px 0;
        }
        header h1 {
            font-size: 3rem;
            margin: 0;
        }
        header p {
            font-size: 1.2rem;
            margin-top: 10px;
        }
        section {
            padding: 60px 20px;
            text-align: center;
        }
        section h2 {
            font-size: 2rem;
            margin-bottom: 20px;
        }
        .products {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 30px;
        }
        .product-card {
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            width: 250px;
            padding: 20px;
            text-align: center;
        }
        .product-card img {
            width: 100%;
            border-radius: 8px;
        }
        .product-card h3 {
            font-size: 1.5rem;
            margin-top: 15px;
        }
        .product-card p {
            font-size: 1rem;
            color: #666;
            margin-top: 10px;
        }
        .cta-btn {
            background-color: #0069d9;
            color: white;
            padding: 15px 30px;
            font-size: 1.1rem;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 30px;
            display: inline-block;
        }
        .cta-btn:hover {
            background-color: #0056b3;
        }
        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 20px;
        }
        .order-form {
            background-color: #fff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            width: 400px;
            margin: 50px auto;
        }
        .order-form input, .order-form select, .order-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        .order-form button {
            background-color: #28a745;
            color: white;
            padding: 12px 20px;
            font-size: 1.2rem;
            border: none;
            border-radius: 5px;
            width: 100%;
        }
        .order-form button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <header>
        <h1>Memory Vault</h1>
        <p>Your custom printing destination for sweaters, t-shirts, tote bags, and caps.</p>
    </header>

    <section>
        <h2>Our Products</h2>
        <div class="products">
            <div class="product-card">
                <img src="https://via.placeholder.com/250x250.png?text=Sweater" alt="Sweater">
                <h3>Sweaters</h3>
                <p>Personalized sweaters for all occasions. Your design, our print.</p>
            </div>
            <div class="product-card">
                <img src="https://via.placeholder.com/250x250.png?text=T-shirt" alt="T-shirt">
                <h3>T-Shirts</h3>
                <p>Custom t-shirts to express your style. Create your own unique design.</p>
            </div>
            <div class="product-card">
                <img src="https://via.placeholder.com/250x250.png?text=Tote+Bag" alt="Tote Bag">
                <h3>Tote Bags</h3>
                <p>Eco-friendly tote bags with your custom design. Great for shopping or gifting!</p>
            </div>
            <div class="product-card">
                <img src="https://via.placeholder.com/250x250.png?text=Cap" alt="Cap">
                <h3>Caps</h3>
                <p>Stylish caps with personalized prints. Perfect for casual wear or sports.</p>
            </div>
        </div>

        <a href="#order-form" class="cta-btn">Request an Order</a>
    </section>

    <section id="order-form">
        <h2>Place Your Order</h2>
        <form class="order-form" action="https://printify.com/order" method="POST" target="_blank">
            <label for="product">Choose Product</label>
            <select id="product" name="product">
                <option value="sweater">Sweater</option>
                <option value="tshirt">T-shirt</option>
                <option value="totebag">Tote Bag</option>
                <option value="cap">Cap</option>
            </select>

            <label for="design">Describe Your Design</label>
            <textarea id="design" name="design" placeholder="Describe the design you want" rows="4"></textarea>

            <label for="quantity">Quantity</label>
            <input type="number" id="quantity" name="quantity" min="1" placeholder="How many pieces?" required>

            <label for="email">Email Address</label>
            <input type="email" id="email" name="email" placeholder="Your email address" required>

            <button type="submit">Submit Order</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Memory Vault. All rights reserved. | <a href="https://printify.com" target="_blank" style="color: #fff;">Powered by Printify</a></p>
    </footer>
</body>
</html>
