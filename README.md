<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>متجر منوش</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            direction: rtl;
            background-color: #f4f4f9;
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            padding: 15px 0;
            text-align: center;
        }
        header h1 {
            margin: 0;
            font-size: 36px;
        }
        .container {
            width: 90%;
            margin: 20px auto;
        }
        .products {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }
        .product-card {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 250px;
            padding: 20px;
            text-align: center;
            transition: transform 0.2s;
        }
        .product-card:hover {
            transform: scale(1.05);
        }
        .product-image img {
            width: 100%;
            border-radius: 8px;
        }
        .product-name {
            font-size: 18px;
            margin: 10px 0;
        }
        .product-price {
            font-size: 20px;
            color: #2ecc71;
        }
        .add-to-cart {
            background-color: #3498db;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
            margin-top: 10px;
            transition: background-color 0.3s;
        }
        .add-to-cart:hover {
            background-color: #2980b9;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

<header>
    <h1>متجر منوش</h1>
    <p>أفضل المنتجات لاحتياجاتك اليومية</p>
</header>

<div class="container">
    <section>
        <h2 style="text-align: center;">منتجاتنا</h2>
        <div class="products">
            <div class="product-card">
                <div class="product-image">
                    <img src="https://via.placeholder.com/250" alt="منتج 1">
                </div>
                <div class="product-name">منتج 1</div>
                <div class="product-price">100 ريال</div>
                <button class="add-to-cart" onclick="addToCart('منتج 1', 100)">أضف إلى السلة</button>
            </div>
            <div class="product-card">
                <div class="product-image">
                    <img src="https://via.placeholder.com/250" alt="منتج 2">
                </div>
                <div class="product-name">منتج 2</div>
                <div class="product-price">150 ريال</div>
                <button class="add-to-cart" onclick="addToCart('منتج 2', 150)">أضف إلى السلة</button>
            </div>
            <div class="product-card">
                <div class="product-image">
                    <img src="https://via.placeholder.com/250" alt="منتج 3">
                </div>
                <div class="product-name">منتج 3</div>
                <div class="product-price">200 ريال</div>
                <button class="add-to-cart" onclick="addToCart('منتج 3', 200)">أضف إلى السلة</button>
            </div>
        </div>
    </section>
</div>

<footer>
    <p>&copy; 2024 متجر منوش | جميع الحقوق محفوظة</p>
</footer>

<script>
    let cart = [];

    function addToCart(productName, productPrice) {
        cart.push({ name: productName, price: productPrice });
        alert(`${productName} أُضيف إلى السلة. لديك الآن ${cart.length} منتج في السلة.`);
    }
</script>

</body>
</html>
- [ ] 
