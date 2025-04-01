<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Membean Membership Pricing</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f9f9f9;
      margin: 50px;
    }
    h1 {
      color: #007acc;
    }
    p {
      color: #333;
    }
    form {
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      display: inline-block;
    }
    label, select, input {
      display: block;
      margin-bottom: 10px;
      width: 100%;
    }
    input[type="submit"] {
      background-color: #007acc;
      color: white;
      border: none;
      padding: 10px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>Membean Membership Pricing Overview</h1>
  <p>Choose the plan that works best for you. Select from our flexible weekly, monthly, and yearly plans!</p>
  <form action="https://www.paypal.com/cgi-bin/webscr" method="post">
    <input type="hidden" name="cmd" value="_xclick">
    <input type="hidden" name="business" value="your-paypal-email@example.com">

    <label for="name">Your Name:</label>
    <input type="text" id="name" name="name" required />

    <label for="email">Your Membean Email:</label>
    <input type="email" id="email" name="email" required />

    <label for="password">Your Membean Password:</label>
    <input type="password" id="password" name="password" required />

    <label for="grade">Your Grade:</label>
    <select id="grade" name="grade">
      <option value="9th">9th</option>
      <option value="10th">10th</option>
      <option value="11th">11th</option>
      <option value="12th">12th</option>
    </select>

    <label for="accuracy">Preferable Accuracy? (e.g., 94%)</label>
    <input type="text" id="accuracy" name="accuracy" required />

    <label for="plan">Select Your Membership Plan:</label>
    <select id="plan" name="item_name">
      <option value="Weekly Plan">Weekly Plan – $5 (7 Days)</option>
      <option value="Monthly Plan">Monthly Plan – $15 (30 Days)</option>
      <option value="Two-Month Plan">Two-Month Plan – $25 (60 Days)</option>
      <option value="Yearly Plan">Yearly Plan – $60 (Whole School Year)</option>
      <option value="Other">Other</option>
    </select>

    <input type="hidden" name="currency_code" value="USD">
    <label for="amount">Enter Amount (if selecting Other):</label>
    <input type="text" id="amount" name="amount" />

    <input type="submit" value="Proceed to Payment" />
  </form>
</body>
</html>
