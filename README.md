<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Register | Stress Support</title>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: "Segoe UI", sans-serif;
      background: linear-gradient(145deg, #d6e4f0, #f0f4f8);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      perspective: 1000px;
    }

    .form-card {
      background-color: #ffffff;
      padding: 40px 30px;
      border-radius: 15px;
      width: 100%;
      max-width: 400px;
      box-shadow: 0 20px 30px rgba(0, 0, 0, 0.1);
      transform: rotateY(0deg);
      transition: transform 0.6s ease, box-shadow 0.4s ease;
    }

    .form-card:hover {
      transform: rotateY(3deg);
      box-shadow: 0 25px 45px rgba(0, 0, 0, 0.15);
    }

    h2 {
      text-align: center;
      margin-bottom: 30px;
      color: #333;
    }

    label {
      margin-top: 15px;
      display: block;
      font-weight: 600;
      color: #444;
    }

    input,
    select {
      width: 100%;
      padding: 12px;
      margin-top: 5px;
      border-radius: 8px;
      border: 1px solid #ccc;
      background-color: #f9f9f9;
      font-size: 15px;
    }

    button {
      width: 100%;
      padding: 14px;
      margin-top: 25px;
      background: linear-gradient(135deg, #007bff, #0056b3);
      color: #fff;
      font-weight: bold;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    button:hover {
      background: linear-gradient(135deg, #0056b3, #003f7f);
    }

    .thank-you {
      text-align: center;
      font-size: 18px;
      font-weight: 600;
      color: green;
      margin-top: 25px;
      display: none;
    }

    @media (max-width: 480px) {
      .form-card {
        padding: 30px 20px;
      }
    }
  </style>
</head>
<body>

  <div class="form-card">
    <h2>Register</h2>

    <form id="registrationForm">
      <label for="phone">Phone Number</label>
      <input type="tel" id="phone" name="phone" placeholder="e.g. 9876543210" required>

      <label for="age">Age</label>
      <input type="number" id="age" name="age" min="10" max="120" placeholder="Enter your age" required>

      <label for="gender">Gender</label>
      <select id="gender" name="gender" required>
        <option value="">-- Select Gender --</option>
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="non-binary">Non-binary</option>
        <option value="prefer-not">Prefer not to say</option>
      </select>

      <button type="submit">Submit</button>
    </form>

    <div class="thank-you" id="thankYouMessage">
      ✅ Thank you for your participation!
    </div>
  </div>

  <script>
    const form = document.getElementById("registrationForm");
    const thankYouMessage = document.getElementById("thankYouMessage");

    form.addEventListener("submit", function(event) {
      event.preventDefault();
      form.style.display = "none";
      thankYouMessage.style.display = "block";
    });
  </script>

</body>
</html>
created by "Ayushman Agarwal"
