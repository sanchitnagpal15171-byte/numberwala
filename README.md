<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VIP Vehicle Numbers India</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Roboto', sans-serif; margin: 0; padding: 0; background: #f5f5f5; color: #333; }
        header { background: #1c1c1c; color: #fff; padding: 20px; text-align: center; }
        nav a { color: #fff; margin: 0 15px; text-decoration: none; font-weight: 500; }
        section { padding: 50px 20px; max-width: 1200px; margin: auto; }
        h2 { text-align: center; margin-bottom: 30px; }
        .numbers { display: flex; flex-wrap: wrap; justify-content: center; gap: 15px; }
        .number-card { background: #fff; padding: 20px; border-radius: 10px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); width: 120px; text-align: center; font-weight: bold; font-size: 24px; }
        form { background: #fff; padding: 20px; border-radius: 10px; max-width: 500px; margin: auto; box-shadow: 0 2px 8px rgba(0,0,0,0.1); }
        input, select, textarea, button { width: 100%; padding: 12px; margin: 8px 0; border-radius: 6px; border: 1px solid #ccc; font-size: 16px; }
        button { background: #ff6b00; color: #fff; border: none; cursor: pointer; font-weight: bold; }
        button:hover { background: #e65a00; }
        footer { background: #1c1c1c; color: #fff; text-align: center; padding: 20px; margin-top: 50px; }
        .search-box { text-align: center; margin-bottom: 30px; }
        @media(max-width:768px){ .numbers{ flex-direction: column; align-items: center; } }
    </style>
</head>
<body>

<header>
    <h1>VIP Vehicle Numbers India</h1>
    <nav>
        <a href="#home">Home</a>
        <a href="#search">Search Numbers</a>
        <a href="#book">Book Now</a>
        <a href="#pricing">Pricing</a>
    </nav>
</header>

<section id="home">
    <h2>Find Your Dream Vehicle Number</h2>
    <p style="text-align:center; max-width:800px; margin:auto;">We help you search and book exclusive VIP/fancy vehicle numbers. Make your car or bike stand out with the perfect number plate!</p>
</section>

<section id="search">
    <h2>Search Available Fancy Numbers</h2>
    <div class="search-box">
        <input type="text" id="searchInput" placeholder="Enter number to check availability (e.g. 1111)">
        <button onclick="searchNumber()">Check Availability</button>
    </div>
    <div class="numbers" id="numbersList">
        <!-- Number cards will appear here -->
    </div>
</section>

<section id="book">
    <h2>Book Your VIP Number</h2>
    <form id="bookingForm">
        <input type="text" placeholder="Full Name" id="name" required>
        <input type="text" placeholder="Phone Number" id="phone" required>
        <select id="vehicle" required>
            <option value="">Select Vehicle Type</option>
            <option value="Car">Car</option>
            <option value="Bike">Bike</option>
            <option value="Truck">Truck</option>
        </select>
        <input type="text" placeholder="Desired Number" id="number" required>
        <textarea placeholder="Additional Notes (optional)" id="notes"></textarea>
        <button type="button" onclick="submitBooking()">Book via WhatsApp</button>
    </form>
</section>

<section id="pricing">
    <h2>Service Pricing</h2>
    <p style="text-align:center; max-width:700px; margin:auto;">Our service fee ranges from <strong>₹500 – ₹5000</strong> depending on the rarity of the number. We handle the booking and guide you through the official process.</p>
</section>

<footer>
    <p>&copy; 2026 VIP Vehicle Numbers India | Designed to help you get your dream number</p>
</footer>

<script>
const availableNumbers = ["0001","1111","0786","9999","0070","1234","5555","2222","3333","4444"];

function displayNumbers(numbers){
    const numbersList = document.getElementById('numbersList');
    numbersList.innerHTML = '';
    if(numbers.length === 0){
        numbersList.innerHTML = '<p style="text-align:center; width:100%;">No numbers available.</p>';
        return;
    }
    numbers.forEach(num => {
        const div = document.createElement('div');
        div.className = 'number-card';
        div.textContent = num;
        numbersList.appendChild(div);
    });
}

// Initially show all numbers
displayNumbers(availableNumbers);

function searchNumber(){
    const query = document.getElementById('searchInput').value.trim();
    if(!query) { alert('Enter a number to check.'); return; }
    const filtered = availableNumbers.filter(n => n.includes(query));
    displayNumbers(filtered);
}

function submitBooking(){
    const name = document.getElementById('name').value;
    const phone = document.getElementById('phone').value;
    const vehicle = document.getElementById('vehicle').value;
    const number = document.getElementById('number').value;
    const notes = document.getElementById('notes').value;

    if(!name || !phone || !vehicle || !number){
        alert('Please fill all required fields.');
        return;
    }

    const message = `Hello! I want to book a VIP number.\n\nName: ${name}\nPhone: ${phone}\nVehicle: ${vehicle}\nDesired Number: ${number}\nNotes: ${notes}`;
    const whatsappURL = `https://wa.me/911234567890?text=${encodeURIComponent(message)}`; // Replace with your WhatsApp
    window.open(whatsappURL, '_blank');
}
</script>

</body>
</html>
