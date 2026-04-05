<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Krest Eyewear | Luxury Frames & Lenses</title>
  <style>
    :root {
      --primary: #5a2d82; /* Deep Purple */
      --accent: #ff8800;  /* Vibrant Orange */
      --light: #ffffff;
      --background: #f9f7fc;
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: var(--background);
      color: #222;
      line-height: 1.6;
    }

    header {
      background: var(--primary);
      color: var(--light);
      padding: 1.5rem 2rem;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 2rem;
      letter-spacing: 2px;
    }

    nav {
      background: var(--accent);
      padding: 0.8rem;
      text-align: center;
    }

    nav a {
      color: var(--light);
      text-decoration: none;
      margin: 0 1rem;
      font-size: 1rem;
      font-weight: 500;
    }

    section {
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
      background: var(--light);
      margin-top: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 3px 6px rgba(0, 0, 0, 0.1);
    }

    h2 {
      color: var(--primary);
      border-bottom: 3px solid var(--accent);
      padding-bottom: 0.5rem;
    }

    .products {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem;
    }

    .product {
      flex: 1 1 45%;
      background: #f5f2fa;
      padding: 1rem;
      border-left: 5px solid var(--accent);
      border-radius: 8px;
    }

    form {
      display: grid;
      gap: 1rem;
      margin-top: 1rem;
    }

    input, select, textarea, button {
      padding: 0.7rem;
      font-size: 1rem;
      border-radius: 6px;
      border: 1px solid #ccc;
    }

    button {
      background: var(--accent);
      color: var(--light);
      font-weight: 600;
      border: none;
      transition: 0.3s;
      cursor: pointer;
    }

    button:hover {
      background: var(--primary);
    }

    footer {
      text-align: center;
      background: var(--primary);
      color: var(--light);
      padding: 1.5rem;
      margin-top: 2rem;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 1rem;
    }

    table th, table td {
      border: 1px solid #ddd;
      padding: 0.6rem;
      text-align: left;
    }

    table th {
      background: #f3eafc;
    }

    #message, #reminder {
      margin-top: 1rem;
      padding: 0.8rem;
      border-radius: 6px;
      background: #eafaf1;
      color: #222;
      display: none;
    }
  </style>
</head>
<body>

<header>
  <h1>KREST EYEWEAR</h1>
  <p>Luxury Vision • Precision Design • Countrywide Delivery</p>
</header>

<nav>
  <a href="#about">About</a>
  <a href="#products">Products</a>
  <a href="#book">Book & Checkout</a>
  <a href="#records">Records</a>
  <a href="#contact">Contact</a>
</nav>

<section id="about">
  <h2>About Krest Eyewear</h2>
  <p>
    At <strong>Krest Eyewear</strong>, we blend innovation and craftsmanship to deliver luxury eyewear built for clarity and confidence. 
    Each frame is precision-engineered and paired with premium lenses to give you the best possible vision.
  </p>
</section>

<section id="products">
  <h2>Our Collections</h2>
  <div class="products">
    <div class="product">
      <h3>Premium Frames</h3>
      <p>From <strong>$3,500</strong></p>
      <ul>
        <li>Executive Classic – Rectangular Build</li>
        <li>Modern Aviator – Titanium Style</li>
        <li>Couture Round – Artisan Handmade</li>
        <li>Signature Minimal – Rimless Elegance</li>
      </ul>
    </div>
    <div class="product">
      <h3>Lenses</h3>
      <p>From <strong>$2,500</strong> depending on prescription</p>
      <ul>
        <li>Prescription Lenses (Single/Progressive)</li>
        <li>Blue-Light Filtering</li>
        <li>Anti-Reflective & UV Coated</li>
        <li>Transition or Polarized Options</li>
      </ul>
    </div>
  </div>
</section>

<section id="book">
  <h2>Book & Checkout</h2>
  <form id="checkout-form">
    <label>Full Name</label>
    <input type="text" id="name" required>

    <label>Email</label>
    <input type="email" id="email" required>

    <label>Phone Number</label>
    <input type="tel" id="phone" required>

    <label>Delivery Address</label>
    <textarea id="address" rows="3" required></textarea>

    <label>Frame Selection</label>
    <select id="frame">
      <option>Executive Classic - $3,500</option>
      <option>Modern Aviator - $3,700</option>
      <option>Couture Round - $3,900</option>
      <option>Signature Minimal - $4,000</option>
    </select>

    <label>Lens Type</label>
    <select id="lens">
      <option>Prescription - $2,500+</option>
      <option>Blue Light Filter - $2,800</option>
      <option>Transition - $3,000</option>
      <option>Polarized - $3,200</option>
    </select>

    <label>Prescription Notes</label>
    <textarea id="prescription" rows="3"></textarea>

    <button type="submit">Record Booking</button>
  </form>

  <div id="message">✅ Booking recorded successfully!</div>
  <div id="reminder">📅 Reminder: Your annual check-up is due!</div>
</section>

<section id="records">
  <h2>Client Records</h2>
  <table id="records-table">
    <thead>
      <tr>
        <th>Name</th>
        <th>Contact</th>
        <th>Frame</th>
        <th>Lens</th>
        <th>Prescription</th>
        <th>Next Check-Up</th>
      </tr>
    </thead>
    <tbody></tbody>
  </table>
</section>

<footer id="contact">
  <p>📞 +254 706 409 408 | 📧 kresteyewear@gmail.com</p>
  <p>© 2024 Krest Eyewear. All Rights Reserved.</p>
</footer>

<script>
const form = document.getElementById('checkout-form');
const tableBody = document.querySelector('#records-table tbody');
const message = document.getElementById('message');
const reminder = document.getElementById('reminder');

function loadRecords() {
  const records = JSON.parse(localStorage.getItem('krestRecords')) || [];
  tableBody.innerHTML = '';
  const today = new Date();

  records.forEach(r => {
    const nextCheck = new Date(r.nextCheck);
    const row = document.createElement('tr');
    row.innerHTML = `
      <td>${r.name}</td>
      <td>${r.phone}<br>${r.email}</td>
      <td>${r.frame}</td>
      <td>${r.lens}</td>
      <td>${r.prescription}</td>
      <td>${nextCheck.toDateString()}</td>
    `;
    tableBody.appendChild(row);

    // Show reminder if past due
    if (today >= nextCheck && !r.reminderShown) {
      reminder.style.display = 'block';
      r.reminderShown = true;
      localStorage.setItem('krestRecords', JSON.stringify(records));
    }
  });
}

form.addEventListener('submit', e => {
  e.preventDefault();
  const now = new Date();
  const nextYear = new Date();
  nextYear.setFullYear(now.getFullYear() + 1);

  const record = {
    name: document.getElementById('name').value,
    email: document.getElementById('email').value,
    phone: document.getElementById('phone').value,
    address: document.getElementById('address').value,
    frame: document.getElementById('frame').value,
    lens: document.getElementById('lens').value,
    prescription: document.getElementById('prescription').value,
    date: now,
    nextCheck: nextYear
  };

  const records = JSON.parse(localStorage.getItem('krestRecords')) || [];
  records.push(record);
  localStorage.setItem('krestRecords', JSON.stringify(records));

  message.style.display = 'block';
  setTimeout(() => message.style.display = 'none', 3000);
  form.reset();
  loadRecords();
});

loadRecords();
</script>

</body>
</html>
