# Pizzaria
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pizzaria</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>

  <header>
    <h1>Pizzaria</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">Menu</a>
    <a href="customer_care.html">Customer Care</a>
  </nav>

  <section>
    <h2>Menu</h2>

    <!-- Menu items as needed -->

  </section>

  <section>
    <h2>Shopping Cart</h2>
    <ul id="cart"></ul>
    <p>Total: $<span id="total">0.00</span></p>
    <button onclick="placeOrder()">Place Order</button>
  </section>

  <section>
    <h2>Restaurant Location</h2>
    <p id="restaurantLocation">Loading...</p>
  </section>

  <footer>
    &copy; 2023 Pizzaria




      <!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pizzaria</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>

  <header>
    <h1>Pizzaria</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">Menu</a>
    <a href="customer_care.html">Customer Care</a>
  </nav>

  <section>
    <h2>Menu</h2>

    <!-- Menu items as needed -->

  </section>

  <section>
    <h2>Shopping Cart</h2>
    <ul id="cart"></ul>
    <p>Total: $<span id="total">0.00</span></p>
    <button onclick="placeOrder()">Place Order</button>
  </section>

  <section>
    <h2>Restaurant Location</h2>
    <p id="restaurantLocation">Loading...</p>
  </section>

  <footer>
    &copy; 2023 Pizzaria
  </footer>

  <script src="script.js"></script>
</body>

</html>

// Placeholder data for restaurant branches
const restaurantBranches = [
  { name: 'Main Branch', address: '123 Main St, City1, Country1', location: { latitude: 40.7128, longitude: -74.0060 } },
  { name: 'Branch 2', address: '456 Oak St, City2, Country2', location: { latitude: 34.0522, longitude: -118.2437 } },
  // Add more branches as needed
];

// Function to find and display the current location of the restaurant
async function findRestaurantLocation() {
  try {
    const restaurantLocation = await getCurrentLocation();
    document.getElementById('restaurantLocation').textContent = `Restaurant Location: ${restaurantLocation}`;
  } catch (error) {
    console.error('Error finding restaurant location:', error);
    document.getElementById('restaurantLocation').textContent = 'Error finding restaurant location';
  }
}

// Placeholder function for getting the current location (replace with actual logic)
function getCurrentLocation() {
  return new Promise((resolve, reject) => {
    // Simulate asynchronous location retrieval
    setTimeout(() => {
      const randomBranch = restaurantBranches[Math.floor(Math.random() * restaurantBranches.length)];
      resolve(randomBranch.address);
    }, 1000);
  });
}

// Call the function when the page loads
findRestaurantLocation();
styles.css:

css
Copy code
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

header, nav, section, footer {
  margin: 20px;
  padding: 20px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}

nav a {
  margin: 0 10px;
  text-decoration: none;
  color: #333;
}

nav a:hover {
  color: #ff5555;
}

section {
  margin-bottom: 20px;
}

button {
  background-color: #ff5555;
  color: #fff;
  padding: 10px 15px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button:hover {
  background-color: #cc0000;
}

  </footer>

  <script src="script.js"></script>
</body>

</html>
