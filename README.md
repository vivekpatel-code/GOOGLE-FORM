<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Google Form Clone</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f1f3f4;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
    }

    .form-container {
      background: #fff;
      margin: 40px;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
      width: 100%;
      max-width: 500px;
    }

    h2 {
      text-align: center;
      color: #202124;
    }

    label {
      font-weight: bold;
      display: block;
      margin: 15px 0 5px;
    }

    input, textarea, select {
      width: 100%;
      padding: 10px;
      border: 1px solid #dadce0;
      border-radius: 8px;
      font-size: 14px;
      outline: none;
    }

    input:focus, textarea:focus {
      border: 1px solid #4285F4;
      box-shadow: 0 0 3px #4285F4;
    }

    .gender {
      display: flex;
      gap: 20px;
      margin-top: 5px;
    }

    .gender input {
      width: auto;
    }

    button {
      margin-top: 20px;
      width: 100%;
      padding: 12px;
      background: #4285F4;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    button:hover {
      background: #357ae8;
    }
  </style>
</head>
<body>
  <div class="form-container">
    <h2>Simple Google Form</h2>
    <form>
      <label for="name">Full Name</label>
      <input type="text" id="name" name="name" placeholder="Enter your full name" required>

      <label for="email">Email Address</label>
      <input type="email" id="email" name="email" placeholder="Enter your email" required>

      <label>Gender</label>
      <div class="gender">
        <label><input type="radio" name="gender" value="male" required> Male</label>
        <label><input type="radio" name="gender" value="female"> Female</label>
        <label><input type="radio" name="gender" value="other"> Other</label>
      </div>

      <label for="message">Message</label>
      <textarea id="message" name="message" rows="4" placeholder="Type your message here"></textarea>

      <button type="submit">Submit</button>
    </form>
  </div>
</body>
</html>

