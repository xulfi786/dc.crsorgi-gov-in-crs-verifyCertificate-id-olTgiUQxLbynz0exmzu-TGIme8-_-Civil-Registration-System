# dc.crsorgi-gov-in-crs-verifyCertificate-id-olTgiUQxLbynz0exmzu-TGIme8-_-Civil-Registration-System
Civil Registration System
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CRS DEMO - Civil Registration System</title>
  <link rel="icon" type="image/x-icon" href="https://crsorgi.gov.in/images/emblem-dark.png">
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      background-color: #e5e5e5;
    }
    header {
      background-color: #004080;
      color: white;
      padding: 10px 20px;
      display: flex;
      align-items: center;
      gap: 15px;
    }
    header img {
      height: 60px;
    }
    header div {
      display: flex;
      flex-direction: column;
    }
    nav {
      background-color: #0072c6;
      padding: 10px 20px;
    }
    nav a {
      color: white;
      margin-right: 15px;
      text-decoration: none;
      font-weight: bold;
    }
    .container {
      display: flex;
      max-width: 1200px;
      margin: 20px auto;
      background-color: white;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }
    aside {
      width: 220px;
      background-color: #f2f2f2;
      padding: 20px;
      border-right: 1px solid #ccc;
    }
    aside h3 {
      font-size: 16px;
      margin-bottom: 10px;
    }
    aside ul {
      list-style: none;
      padding: 0;
    }
    aside ul li {
      margin-bottom: 10px;
    }
    main {
      flex: 1;
      padding: 30px;
    }
    .disclaimer {
      color: red;
      font-size: 14px;
      text-align: center;
      margin-top: 20px;
    }
    .footer {
      background-color: #004080;
      color: white;
      text-align: center;
      padding: 15px;
      font-size: 14px;
      margin-top: 30px;
    }
    label, input {
      display: block;
      margin: 10px 0;
    }
    input[type="submit"] {
      background-color: #0072c6;
      color: white;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
    }
    .certificate {
      border: 2px solid #000;
      padding: 20px;
      margin-top: 20px;
      background: #fafafa;
      font-family: 'Georgia', serif;
    }
    .certificate h3 {
      text-align: center;
      text-transform: uppercase;
      border-bottom: 1px solid #000;
      padding-bottom: 10px;
      margin-bottom: 20px;
    }
    .certificate p {
      font-size: 16px;
      margin: 8px 0;
    }
  </style>
  <script>
    function showCertificate(event) {
      event.preventDefault();
      const certId = document.getElementById('cert-id').value.trim();
      const resultDiv = document.getElementById('result');

      if (certId === 'B20253000220004511') {
        resultDiv.innerHTML = `
          <div class="certificate">
            <h3>Government of India<br>Birth Certificate</h3>
            <p><strong>Registration No:</strong> B20253000220004511</p>
            <p><strong>Name:</strong> ZULFIQAR ALI WAZIR r</p>
            <p><strong>Gender:</strong> MALE</p>
            <p><strong>Date of Birth:</strong> 16 APRIL 2012</p>
</strong>16-04-2012<p>
            <p><strong>Place of Birth:</strong> DISTRICT HOSPITAL, KARGIL LADAKH</p>
            <p><strong>Father's Name:</strong> GULZAR ALI WAZIR</p>
            <p><strong>Mother's Name:</strong> SHAHAR BANOO</p>
            <p><strong>Permanent Address:</strong>  </p>
            <p><strong>Date of Registration:</strong> 20 MAY 2025</p>
            <p><strong>Registrar:</strong> KARGIL MUNICIPAL COMMITTE</p>
          </div>`;
      } else {
        resultDiv.innerHTML = `<p style="color:red;">No certificate found for ID: ${certId}</p>`;
      }
    }
  </script>
</head>
<body>
  <header>
    <img src="https://crsorgi.gov.in/images/emblem-dark.png" alt="India Emblem">
    <div>
      <h2>Civil Registration System</h2>
      <small>Office of the Registrar General, India | Ministry of Home Affairs</small>
    </div>
  </header>
  <nav>
    <a href="#">Home</a>
    <a href="#verify">Verify Certificate</a>
    <a href="#services">Services</a>
    <a href="#downloads">Downloads</a>
    <a href="#contact">Contact</a>
  </nav>
  <div class="container">
    <aside>
      <h3>Quick Links</h3>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Certificate Verification</a></li>
        <li><a href="#">Citizen Services</a></li>
        <li><a href="#">Help Manual</a></li>
        <li><a href="#">Official Contacts</a></li>
      </ul>
    </aside>
    <main>
      <h2>Verify Birth Certificate</h2>
      <form onsubmit="showCertificate(event)">
        <label for="cert-id">Enter Certificate ID:</label>
        <input type="text" id="cert-id" name="cert-id" placeholder="e.g. 123456" required>
        <input type="submit" value="Verify">
![image](https://github.com/user-attachments/assets/76354ced-3b64-4242-a85b-7a3c1ceb69bd)
