<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Zee Hair Products - Natural, Sulfate-Free, and Eco-Friendly Hair Care for Modern Women.">
    <title>Zee Hair Products - Home</title>
    <link rel="stylesheet" href="assets/styles/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h1>Welcome to Zee Hair Products</h1>
            <p>Natural hair care for the modern woman</p>
        </section>

        <section class="problem-solution">
            <h2>Why Choose Zee Hair Products?</h2>
            <p><strong>Problem:</strong> 75% of women use hair products with harsh chemicals that damage their hair, scalp, and the environment.</p>
            <p><strong>Solution:</strong> Zee Hair Products offer natural, effective, and affordable hair care with eco-friendly formulas.</p>
        </section>

        <section class="products">
            <h2>Our Products</h2>
            <div class="product-cards">
                <div class="card">
                    <h3>Sulfate-Free Shampoos</h3>
                    <img src="assets/images/shampoo.jpg" alt="Shampoo">
                </div>
                <div class="card">
                    <h3>Eco-Friendly Hair Masks</h3>
                    <img src="assets/images/hair-mask.jpg" alt="Hair Mask">
                </div>
                <div class="card">
                    <h3>Natural Ingredients</h3>
                    <img src="assets/images/ingredients.jpg" alt="Natural Ingredients">
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Zee Hair Products. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Learn more about Zee Hair Products and our mission to offer eco-friendly, sulfate-free hair care products.">
    <title>About Zee Hair Products</title>
    <link rel="stylesheet" href="assets/styles/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="about">
            <h1>About Zee Hair Products</h1>
            <p>We are dedicated to providing natural hair care solutions that are sulfate-free, eco-friendly, and affordable.</p>
        </section>

        <section class="team">
            <h2>Our Team</h2>
            <div class="team-member">
                <h3>Zinhle Ndlovu - Founder & CEO</h3>
                <p>Email: nomathembazinhle383@gmail.com | Contact: 0767004548</p>
            </div>
            <div class="team-member">
                <h3>Lwandile Ndlangamandla - Marketing Manager</h3>
                <p>Contact: 0739388330</p>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Zee Hair Products. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Get in touch with Zee Hair Products for inquiries, customer service, or business partnerships.">
    <title>Contact Zee Hair Products</title>
    <link rel="stylesheet" href="assets/styles/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="contact">
            <h1>Contact Us</h1>
            <p>If you have any questions or inquiries, feel free to reach out to us!</p>
            <form id="contact-form">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message:</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit">Submit</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Zee Hair Products. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
/* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

header {
    background-color: #333;
    padding: 10px;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style-type: none;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

.hero {
    text-align: center;
    background-color: #f4f4f4;
    padding: 50px;
}

h1, h2 {
    color: #333;
}

.product-cards {
    display: flex;
    justify-content: space-around;
    margin-top: 20px;
}

.card {
    background-color: #fff;
    padding: 20px;
    border: 1px solid #ddd;
    text-align: center;
}

.card img {
    width: 100px;
    height: 100px;
    object-fit: cover;
}

footer {
    text-align: center;
    background-color: #333;
    color: white;
    padding: 10px 0;
}

/* Media Queries for Responsiveness */
@media (max-width: 768px) {
    .product-cards {
        flex-direction: column;
        align-items: center;
    }

    nav ul {
        flex-direction: column;
    }
}
document.getElementById('contact-form').addEventListener('submit', function(event) {
    event.preventDefault();
    
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;

    if (!name || !email || !message) {
        alert("All fields are required!");
    } else {
        alert("Thank you for your message!");
        this.reset();
    }
});
