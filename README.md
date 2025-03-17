<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Recipe Delight</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f4f4f4; }
        .container { width: 80%; margin: 20px auto; padding: 20px; background: white; box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1); border-radius: 8px; }
        nav a { margin: 0 15px; text-decoration: none; color: #007bff; font-weight: bold; }
        h1, h2 { color: #333; }
        button { background: #007bff; color: white; border: none; padding: 10px 15px; border-radius: 5px; cursor: pointer; }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to Recipe Delight</h1>
        <nav>
            <a href="login.html">Login</a>
            <a href="signup.html">Sign Up</a>
            <a href="home.html">Home</a>
        </nav>
    </div>
</body>
</html>


https://github.com/shafiusymp/recipe-website.git 
Features:
•	Main Page: Welcomes users to the recipe website.
•	Login Page: Users can log in (with an alert message on successful login).
•	Sign-up Page: A simple form for new users.
•	Home Page: Displays menu items (recipes).
•	Product Page: If selling recipe ingredients, this will list them.
•	Checkout Page: Allows users to confirm their purchase.

Folder Structure
recipe-website/
│── index.html (Main Page)
│── login.html (Login Page)
│── signup.html (Sign-up Page)
│── home.html (Home Page)
│── product.html (Products Page - optional)
│── checkout.html (Checkout Page - optional)
│── styles.css (CSS for styling)
│── script.js (JavaScript functionality)
│── images/ (folder for images)

1. Main Page (index.html)
html
CopyEdit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recipe Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to My Recipe Website</h1>
        <nav>
            <a href="login.html">Login</a>
            <a href="signup.html">Sign Up</a>
        </nav>
    </header>
</body>
</html>

2. Login Page (login.html)
html
CopyEdit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h2>Login</h2>
    <form onsubmit="return login()">
        <label>Email:</label>
        <input type="email" required>
        <label>Password:</label>
        <input type="password" required>
        <button type="submit">Login</button>
    </form>
    <script>
        function login() {
            alert("Login successfully!");
            window.location.href = "home.html";
            return false;
        }
    </script>
</body>
</html>

3. Sign-up Page (signup.html)
html
CopyEdit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h2>Sign Up</h2>
    <form>
        <label>Name:</label>
        <input type="text" required>
        <label>Email:</label>
        <input type="email" required>
        <label>Password:</label>
        <input type="password" required>
        <button type="submit">Sign Up</button>
    </form>
</body>
</html>

4. Home Page (home.html)
html
CopyEdit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Recipe Menu</h1>
        <nav>
            <a href="product.html">Products</a>
            <a href="checkout.html">Checkout</a>
        </nav>
    </header>
    <section>
        <h2>Popular Recipes</h2>
        <ul>
            <li>Spaghetti Bolognese</li>
            <li>Fried Rice</li>
            <li>Grilled Chicken</li>
        </ul>
    </section>
</body>
</html>

5. Product Page (product.html - optional)
html
CopyEdit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Products</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h2>Ingredients for Sale</h2>
    <ul>
        <li>Tomatoes - $5</li>
        <li>Rice - $10</li>
        <li>Chicken - $15</li>
    </ul>
    <a href="checkout.html">Go to Checkout</a>
</body>
</html>

6. Checkout Page (checkout.html - optional)
html
CopyEdit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Checkout</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h2>Checkout</h2>
    <p>Thank you for your purchase!</p>
</body>
</html>

7. CSS Styling (styles.css)
css
CopyEdit
body {
    font-family: Arial, sans-serif;
    background-color: #f8f8f8;
    text-align: center;
}

h1, h2 {
    color: #333;
}

nav a {
    margin: 10px;
    text-decoration: none;
    color: blue;
}

form {
    background: white;
    padding: 20px;
    display: inline-block;
    border-radius: 5px;
}

button {
    background: green;
    color: white;
    padding: 10px;
    border: none;
}

