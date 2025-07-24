
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Release the Stress - Registration</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f4f8;
      padding: 20px;
    }
    .container {
      max-width: 600px;
      margin: auto;
      background-color: #ffffff;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    h2 {
      text-align: center;
      color: #333;
    }
    label {
      display: block;
      margin-top: 15px;
      color: #555;
    }
    input, textarea, select {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    textarea {
      height: 150px;
    }
    button {
      margin-top: 20px;
      background-color: #0077cc;
      color: white;
      border: none;
      padding: 12px;
      width: 100%;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #005fa3;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Share What’s On Your Mind</h2>
    <form action="/submit" method="POST">
      <label for="name">Your Name</label>
      <input type="text" id="name" name="name" placeholder="Enter your name" required>

      <label for="gender">Gender</label>
      <select id="gender" name="gender" required>
        <option value="">--Select--</option>
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="non-binary">Non-binary</option>
        <option value="prefer-not">Prefer not to say</option>
      </select>

      <label for="phone">Phone Number (Optional)</label>
      <input type="tel" id="phone" name="phone" placeholder="Enter your phone number">

      <label for="feelings">Why Are You Feeling Stressed?</label>
      <textarea id="feelings" name="feelings" placeholder="Write your thoughts here..." required></textarea>

      <button type="submit">Submit</button>
    </form>
  </div>
</body>
</html>
