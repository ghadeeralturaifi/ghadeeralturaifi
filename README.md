<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cipriani Restaurant</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
            color: #333;
        }
        header {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 1rem 0;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #34495e;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 1rem 2rem;
            display: block;
        }
        nav a:hover {
            background-color: #1abc9c;
        }
        section {
            padding: 2rem;
            text-align: center;
        }
        .menu img {
            width: 200px;
            height: auto;
            border-radius: 10px;
            margin: 10px;
        }
        .gallery img {
            width: 250px;
            height: auto;
            border-radius: 10px;
            margin: 10px;
        }
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 1rem 0;
            margin-top: 2rem;
        }
        .social-media a {
            margin: 0 10px;
            color: #ecf0f1;
            text-decoration: none;
            font-size: 1.5rem;
        }
        .social-media a:hover {
            color: #1abc9c;
        }
        form {
            max-width: 400px;
            margin: 0 auto;
            text-align: left;
            background-color: #ffffff;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        form label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
        }
        form input, form select, form button {
            width: 100%;
            padding: 0.75rem;
            margin-bottom: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }
        form button {
            background-color: #3498db;
            color: white;
            border: none;
            cursor: pointer;
        }
        form button:hover {
            background-color: #2980b9;
        }
        table {
            margin: 20px auto;
            border-collapse: collapse;
            width: 80%;
        }
        table, th, td {
            border: 1px solid #ccc;
        }
        th, td {
            padding: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Cipriani Restaurant</h1>
        <p>Experience the finest Italian cuisine</p>
    </header>

    <nav>
        <a href="#menu">Menu</a>
        <a href="#reservation">Reservation</a>
        <a href="#gallery">Gallery</a>
        <a href="#branches">Our Branches</a>
    </nav>

    <section id="menu" class="menu">
        <h2>Our Exquisite Menu</h2>
        <p>Discover our curated selection of Italian delicacies.</p>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/58oia61564916529.jpg" alt="Soup">
            <p>Soup</p>
        </div>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/wrpwuu1511786491.jpg" alt="Ratatouille">
            <p>Ratatouille</p>
        </div>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/xxtsvx1511814083.jpg" alt="Hummus">
            <p>Hummus</p>
        </div>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/wtsvxx1511296896.jpg" alt="Lasagna">
            <p>Lasagna</p>
        </div>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/uyqrrv1511553350.jpg" alt="Potato balls">
            <p>Potato balls</p>
        </div>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/usywpp1511189717.jpg" alt="Pasta">
            <p>Pasta</p>
        </div>
    </section>

    <section id="reservation" class="reservation">
        <h2>Make a Reservation</h2>
        <form action="/reserve" method="POST">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your name" required>

            <label for="branch">Branch:</label>
            <select id="branch" name="branch" required>
                <option value="" disabled selected>Select a branch</option>
                <option value="Dubai">Dubai - Sheikh Mohammed Blvd</option>
                <option value="Riyadh">Riyadh - King Fahd Road</option>
                <option value="New York">New York - Fifth Avenue</option>
            </select>

            <label for="date">Date:</label>
            <input type="date" id="date" name="date" required>

            <label for="time">Time:</label>
            <input type="time" id="time" name="time" required>

            <label for="guests">Number of Guests:</label>
            <input type="number" id="guests" name="guests" min="1" max="20" required>

            <button type="submit">Reserve Now</button>
        </form>
    </section>

    <section id="drinks" class="drinks">
        <h2>Our Drinks</h2>
        <p>Explore our selection of hot and cold beverages:</p>
        <table>
            <tr>
                <th rowspan="2">Type</th>
                <th colspan="2">Options</th>
            </tr>
            <tr>
                <td>Hot Drinks</td>
                <td>Cold Drinks</td>
            </tr>
            <tr>
                <td>Coffee</td>
                <td>Espresso</td>
                <td>Iced Coffee</td>
            </tr>
            <tr>
                <td>Tea</td>
                <td>Green Tea</td>
                <td>Iced Tea</td>
            </tr>
        </table>
    </section>

    <section id="gallery" class="gallery">
        <h2>Gallery</h2>
        <p>Explore the ambiance and our culinary masterpieces.</p>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/58oia61564916529.jpg" alt="Restaurant Interior">
            <p>Restaurant Interior</p>
        </div>
        <div>
            <img src="https://www.themealdb.com/images/media/meals/wrpwuu1511786491.jpg" alt="Italian Dish">
            <p>Italian Dish</p>
        </div>
    </section>

    <section id="branches" class="branches">
        <h2>Our Branches</h2>
        <p>Visit us at our various locations:</p>
        <ul>
            <li>📍 Dubai - Sheikh Mohammed Blvd</li>
            <li>📍 Riyadh - King Fahd Road</li>
            <li>📍 New York - Fifth Avenue</li>
        </ul>
    </section>

    <footer>
        <p>&copy; 2024 Cipriani Restaurant. All rights reserved.</p>
        <div class="social-media">
            <a href="https://www.instagram.com/cipriani" target="_blank" title="Instagram">
                <i class="fab fa-instagram" style="font-size: 30px; color: #ecf0f1; margin: 0 10px;"></i>
            </a>
            <a href="https://twitter.com/cipriani" target="_blank" title="Twitter">
                <i class="fab fa-twitter" style="font-size: 30px; color: #ecf0f1; margin: 0 10px;"></i>
            </a>
        </div>
    </footer>
</body>
</html>
