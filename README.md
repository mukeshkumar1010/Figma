# Ex09 Event Registration Web Application
## Date: 13.05.2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sports Day Events</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      color: white;
    }
    section {
      display: none;
      height: 100vh;
      padding: 50px 20px;
      text-align: center;
      background-size: cover;
      background-position: center;
    }
    section.active {
      display: block;
    }
    .btn {
      display: inline-block;
      margin: 10px;
      padding: 12px 24px;
      background: #007bff;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      cursor: pointer;
    }
    .form-input {
      width: 80%;
      margin: 10px auto;
      padding: 10px;
      border-radius: 5px;
      border: none;
      display: block;
    }
    .logo {
      width: 100px;
      margin-bottom: 20px;
    }
    ul.event-list {
      list-style: none;
      padding: 0;
    }
    ul.event-list li {
      font-size: 20px;
      margin: 10px 0;
    }

    /* Backgrounds */
    #home { background-image: url('login_bg.jpg'); }
    #events { background-image: url('events_bg.jpg'); }
    #register { background-image: url('form_bg.jpg'); }
    #thankyou { background-image: url('thankyou_bg.jpg'); }
  </style>
</head>
<body>

<!-- Home/Login Page -->
<section id="home" class="active">
  <img src="logo.png" alt="College Logo" class="logo">
  <h1>SPORTS DAY EVENTS</h1>
  <div>
    <span class="btn" onclick="showPage('events')">Login</span>
    <span class="btn" onclick="showPage('events')">Register</span>
  </div>
</section>

<!-- Events List Page -->
<section id="events">
  <h2>SPORTS DAY EVENTS</h2>
  <ul class="event-list">
    <li>CRICKET</li>
    <li>BADMINTON</li>
    <li>VOLLEYBALL</li>
    <li>100 MTS</li>
    <li>KHO KHO</li>
    <li>FOOTBALL</li>
  </ul>
  <div>
    <span class="btn" onclick="showPage('register')">Register for Event</span>
  </div>
</section>

<!-- Registration Form Page -->
<section id="register">
  <h2>EVENTS REGISTRATION FORM</h2>
  <form onsubmit="event.preventDefault(); showPage('thankyou');">
    <input type="text" class="form-input" placeholder="Name" required>
    <input type="text" class="form-input" placeholder="Gender" required>
    <input type="number" class="form-input" placeholder="Age" required>
    <input type="text" class="form-input" placeholder="Reg No" required>
    <input type="text" class="form-input" placeholder="Department" required>
    <input type="tel" class="form-input" placeholder="Contact No" required>
    <button type="submit" class="btn">Register</button>
  </form>
</section>

<!-- Thank You Page -->
<section id="thankyou">
  <h1>THANK YOU</h1>
  <p>We are all waiting for your participation for events</p>
</section>

<!-- JavaScript to switch sections -->
<script>
  function showPage(pageId) {
    document.querySelectorAll('section').forEach(section => {
      section.classList.remove('active');
    });
    document.getElementById(pageId).classList.add('active');
  }
</script>

</body>
</html>
```

## OUTPUT:
![Screenshot 2025-05-13 220426](https://github.com/user-attachments/assets/26233604-36e2-4ca5-80de-5fa9ec490e35)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
