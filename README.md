<!DOCTYPE html>
<html lang="bn">
<head>
 <meta charset="UTF-8">
  <title>তোফায়েল ডেলিভারি সার্ভিস</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #28a745;
      color: white;
      padding: 20px;
      text-align: center;
    }
    form {
      max-width: 500px;
      margin: 40px auto;
      background: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    input, textarea, button {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border-radius: 6px;
      border: 1px solid #ccc;
    }
    button {
      background-color: #28a745;
      color: white;
      font-size: 16px;
      border: none;
    }
    button:hover {
      background-color: #218838;
    }
  </style>
</head>
<body>

<header>
  <h1>তোফায়েল ডেলিভারি সার্ভিস</h1>
  <p>গফরগাঁও-এর যেকোনো নিত্য প্রয়োজনীয় জিনিস এখন আপনার দোরগোড়ায়</p>
</header>

<form id="orderForm">
  <label>আপনার নাম:</label>
  <input type="text" id="name" placeholder="আপনার নাম" required>

  <label>মোবাইল নম্বর:</label>
  <input type="text" id="phone" placeholder="01776781213" required>

  <label>যা লাগবে:</label>
  <textarea id="item" placeholder="যে জিনিসটি দরকার..." required></textarea>

  <label>আপনার ঠিকানা:</label>
  <textarea id="address" placeholder="বিস্তারিত ঠিকানা..." required></textarea>

  <button type="submit">WhatsApp-এ অর্ডার পাঠান</button>
</form>

<script>
  document.getElementById("orderForm").addEventListener("submit", function(e) {
    e.preventDefault();
    const name = document.getElementById("name").value;
    const phone = document.getElementById("phone").value;
    const item = document.getElementById("item").value;
    const address = document.getElementById("address").value;

    const message = `🔔 নতুন অর্ডার:\n\n👤 নাম: ${name}\n📞 মোবাইল: ${phone}\n🛒 চাহিদা: ${item}\n
