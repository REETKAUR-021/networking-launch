<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Networking Lunch</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }
    .header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 40px;
      border-bottom: 1px solid #ccc;
      background-color: white;
      margin: 0;
      font-family: Arial, sans-serif;
    }

    .logo img {
      height: 45px;
    }

    .nav-links {
      display: flex;
      gap: 20px;
    }

    .nav-links a {
      text-decoration: none;
      color: #000;
      font-size: 14px;
      font-size: 17px;
      text-transform: uppercase;
    }

      .top-nav {
      display: flex;
      justify-content: flex-end;
      align-items: center;
      gap: 15px;
      padding:  10px 20px;
      background-color: #001c5a;
      color: white;
      font-size: 16px;
      margin: 0;
    }
    
    .top-nav a {
      color: white;
      text-decoration: none;
    }

    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 60px 80px;
      flex-wrap: wrap;
      margin: 0;
      font-family: Arial, sans-serif;
      color: white;
      background-color:  #001c5a; 
    }

    .left-section {
      max-width: 600px;
    }

    .left-section h1 {
      font-size: 48px;
      margin: 0;
      line-height: 1.2;
      font-weight: 900;
    }

    .left-section p {
      font-size: 16px;
      margin-top: 20px;
      font-weight: 600;
    }

    .right-section {
      max-width: 300px;
      color: #b0b8d1;
      text-align: center;
    }

    .right-section h2 {
      color: black;
      font-size: 25px;
      font-weight: bolder;
      margin-bottom: 10px;
    }

    .right-section p {
      font-size: 14px;
      line-height: 1.5;
      color: grey;
    }

    @media (max-width: 768px) {
      .container {
        flex-direction: column;
        text-align: center;
      }

      .right-section {
        margin-top: 40px;
      }
    }

    .content {
      padding: 40px 20px;
      background-color: whitesmoke;
      text-align: center;
      justify-content: center;
      margin: 40px 30px;
      
    }

    .content h2 {
      text-align: center;
      color: #001c5a;
      margin-bottom: 20px;
      font-weight: bold;
    }

    .content p {
      max-width: 800px;
      margin: auto;
      text-align: center;
      margin-bottom: 40px;
      color: #333;
    }

    .cards {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
    }

    .card {
      background: white;
      border-radius: 10px;
      padding: 20px;
      width: 280px;
      text-align: left;
    }

    .card img {
        width: 100%;
        height: auto;
      background-color: #000;
      color: white;
      font-size: 16px;
      padding: 60px 0;
    }

    
    @media (max-width: 768px) {
  .cards {
    grid-template-columns: 1fr; /* stack 1 card per row on small screens */
    }
  }

  .info-boxes{
    display: flex;
      justify-content: center;
      gap: 20px;
      margin: 20px auto;
      flex-wrap: wrap;
  }

    .info-box {
      background:  #001c5a;
      color: white;
      padding: 20px;
      /* margin: 10px auto; */
      border-radius: 5px;
      width: 500px;
      /* text-align: center; */
    }

    .info-box span {
      color: #76f96b;
      display: block;
      margin-top: 10px;
      font-weight: bold;
    }

    .speakers-section {
      padding: 40px 20px;
      text-align: center;
    }

    .speakers-section h2 {
      color:  #001c5a;
      margin-bottom: 20px;
      font-weight: bold;
    }

    .speaker-card {
      display: inline-block;
      margin: 10px;
      width: 200px;
    }

    .speaker-card img {
      width: 100%;
      background-color: #000;
      padding:  0;
      border: 1px solid black;
      height: 100%;
    }

    .speaker-info {
      margin-top: 10px;
      text-align: center;
    }

    .agenda-section {
      background: #e3ebe4;
      padding: 20px;
      border: 10px;
    }
    .agenda-section h2 {
      color: #001a57;
      margin-bottom: 20px;
      border-left: 3px solid #2db100;
      text-align: left;
    }
    .agenda-table {
      width: 100%;
      border-collapse: collapse;
    }
    .agenda-table td {
      border: 1px solid #ccc;
      padding: 10px;
      vertical-align: top;
    }
    .agenda-table td:first-child {
      background-color: #001a57;
      color: white;
      font-weight: bold;
      width: 100px;
    }
    @media (max-width: 600px) {
      .event-section {
        flex-direction: column;
        align-items: center;
      }
      .info-box {
        font-size: 14px;
      }
    }

    /* Section Title */
    h3 {
      padding-left: 20px;
      margin-top: 40px;
      color: #001c5a;
      border-left: 6px solid #2db100;
      margin: 30px;
      font-weight: bolder;
      font-size: large;
      margin-left: 180px;
    }

    /* Speaker Section */
    .speakers {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 20px;
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: #fff;
      color: #000;
      width: 100%;
      height: 100%;
    }

    .speaker-card {
      width: 260px;
      text-align: center;
      height: 350px;
    }

    .speaker-card img {
      width: 100%;
      background: #000;
      height: 150px;
      object-fit: cover;
    }

    .speaker-name {
      font-weight: bold;
      margin: 10px 0 5px;
      text-align: left;
    }

    .speaker-title {
      font-size: 0.9rem;
      color: #555;
      text-align: left;
    }

    /* Countdown Section */
    .countdown-section {
      background: #2db100;
      color: white;
      padding: 40px 20px;
      text-align: center;
    }

    .countdown-section h2 {
      color: white;
      border-left: none;
      margin-bottom: 10px;
      padding-left: 20px;
      margin-top: 40px;
      border-left: 6px solid white;
      margin: 30px;
      font-weight: bolder;
      font-size: large;
      margin-left: 180px;
      text-align: left;
    }

    .countdown-desc {
      max-width: 700px;
      margin: 0 auto 30px;
      font-size: 1rem;
      line-height: 1.5;
      text-align: left;
      justify-content: left;
      border-left: none;
      margin-left: 180px;
    }

    .pi{
      margin: 0 auto 30px;
      text-align: left;
      border-left: none;
      margin-left: 180px;
    }

    .countdown-timer {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
    }

    .time-box {
      background: #1a8c00;
      padding: 20px;
      border: 5px;
      width: 250px;
      height: 150px;
      color: white;
    }

    .time-box h3 {
      font-size: 2rem;
      margin: 0;
    }

    .time-box p {
      margin: 5px 0 0;
      font-weight: bold;
    }
    
    .reserve-btn {
      background-color:  #001c5a;
      color: white;
      padding: 12px 24px;
      font-weight: bold;
      text-transform: uppercase;
      border: none;
      border: 4px;
      cursor: pointer;
      display: flex;
      justify-content: flex-start;
      align-items: center;
      margin-left: 180px;
    }

    @media (max-width: 768px) {
      .speaker-card {
        width: 100%;
        max-width: 320px;
      }

      .time-box {
        min-width: 45%;
      }
    }

    @media (max-width: 480px) {
      .time-box {
        min-width: 100%;
      }
    }

    .videos-section {
      padding: 40px 20px;
      background: white;
      height: 50px;
    }

    .videos-section h2 {
      color:  #001c5a;
      border-left: 4px solid #2db100;
      padding-left: 10px;
      margin-bottom: 30px;
    }

    .video-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
    }

    .video-card {
      max-width: 320px;
      flex: 1 1 300px;
      background-color: #fff;
    }

    .video-card iframe {
      width: 100%;
      height: auto;
      background: #000;
    }

    .video-label {
      font-size: 12px;
      color: gray;
      margin-top: 10px;
    }

    .video-title {
      font-weight: bold;
      color:  #001c5a;
      margin: 5px 0;
    }

    .video-desc {
      font-size: 0.9rem;
      color: #333;
      margin-bottom: 10px;
    }

    .watch-now img {
      width: 90px;
      height: 90px;
    }

    @media (max-width: 768px) {
      .video-card {
        flex: 1 1 100%;
      }
    }

    .section-title {
      border-left: 5px solid green;
      padding-left: 10px;
      margin: 30px 20px;
      font-size: 28px;
      font-weight: bold;
      color: #1a1a75;
    }

    
    .image-row {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 600px;
      padding: 20px;
    }

    .image-box {
      width: 300px;
      text-align: center;
    }

    .image-box img {
      width: 100%;
      height: auto;
    }

    .image-box h4 {
      font-size: 14px;
      margin-top: 10px;
      color: black;
      border: none;
      text-align: left;
    }

    .image-box h3 {
      font-size: 18px;
      font-weight: bold;
      color: #001c5a;
      margin: 10px 0;
      border: none;
      text-align: left;
    }

    footer {
      background:  #001c5a;
      color: white;
      padding: 30px 20px;
      height: 400px;
      
    }

    footer .footer-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      gap: 30px;
      font-size: larger;
    }

    .footer-column h4 {
      font-size: 20px;
      margin-bottom: 10px;
    }

    .footer-column p, .footer-column a {
      font-size: 14px;
      margin: 4px 0;
      text-decoration: none;
      color: white;
    }

    .footer-column a:hover {
      text-decoration: underline;
    }

    .social-icons a {
      margin-right: 10px;
      color: white;
      font-size: 20px;
    }

    .copyright {
      text-align: left;
      font-size: 13px;
      padding-top: 20px;
      border-top: 1px solid #ccc;
      margin-top: 20px;
      color: white;
    }

    @media (max-width: 768px) {
      .image-row, .text-row, .footer-container {
        flex-direction: column;
        align-items: center;
      }
    }

  </style>
</head>
<body>
  <div class="top-nav">
    <a href="#">BLOG</a>
    <a href="#">ABOUT</a>
    <a href="#">CONTACT US</a>
    <span>1-800-756-4960</span>
  </div>
  <header class="header">
    <div class="logo">
      <img src="https://media.licdn.com/dms/image/v2/D4E0BAQGVskimCS992w/company-logo_200_200/company-logo_200_200/0/1723226554790/servicemax_logo?e=2147483647&v=beta&t=JlVsD7E6aep2RtyothgMcif43q_AZ1Glr4CLNocNMdQ" alt="Service-max Logo" />
    </div>
    <nav class="nav-links">
      <a href="#">Blog</a>
      <a href="#">About</a>
      <a href="#">Contact Us</a>
    </nav>
  </header>

  <div class="container">
    <div class="left-section">
      <h1>A NETWORKING<br>LUNCH WITH A<br>HIGH-TECH FOCUS</h1>
      <p>OCTOBER 13TH 2021 | 11:45 - 14:00 CEST</p>
    </div>
    <div class="right-section">
      <h2>Ready to See More?</h2>
      <p>Ex vocibus urbanitas tincidunt duo. Simul dicam ea qui, novum voluptua gloriatur sed ea, ea usu erat postea reprehendunt.</p>
    </div>
  </div>

  <section class="content">
    <h2>A Networking Lunch with a High-Tech Focus</h2>
    <p>
      ServiceMax and Salesforce are pleased to be hosting a networking lunch with a High-Tech Focus held at the High-Tech Campus in Eindhoven. This informal event will be an opportunity for you to network with your peers whilst learning more about ways to reimagine your service organisation, driving increased customer satisfaction and revenue growth. During this activity we will discuss, amongst other things , some of the key challenges which are faced by organisations within the High-Tech sector , including:
    </p>
    <div class="cards">
      <div class="card">
        <img src="https://res.cloudinary.com/jerrick/image/upload/c_scale,f_jpg,q_auto/63df5b43227cb3001dcfcc22.png" alt="Tech Image"/>
        <p>The increasingly complex technological environment.</p>
      </div>
      <div class="card">
        <img src="https://www.telefonica.com/en/wp-content/uploads/sites/5/2024/01/pexels-photo-1108572-e1706694279617.jpeg?w=1200" alt="Tech Image "/>
        <p>The increasingly complex technological environment.</p>
      </div>
      <div class="card">
        <img src="https://imsnucleii.com/storage/2024/02/Measuring-the-hidden-cost-of-IT-downtime.webp" alt="Tech Image" />
        <p>The significant cost of downtime for buyers of service.</p>
      </div>
      <div class="card">
        <img src="https://horn-it.com/wp-content/uploads/2024/12/Costs-of-IT-Downtime.png" alt="Tech Image">
        <p>The significant cost of downtime for buyers of service.</p>
      </div>
      <div class="card">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRm3TdAczdgI3AnC_jB5mtvngxIO7zpnTwLcQ&s" alt="Tech Image " />
        <p>The significant cost of downtime for buyers of high-tech equipment.</p>
      </div>
      <div class="card">
        <img src="https://media.noria.com/sites/Uploads/2017/12/22/f36bd2af-3d7a-44f8-acfd-d694cf432f21_Images_UnscheduledDowntimeWrath_1234x694_extra_large.jpeg" alt="Tech Image " />
        <p>The significant cost of downtime for buyers of high-tech equipment.</p>
      </div>
    </div>
  
  <section class="info-boxes">
    <div class="info-box">
      <strong>DATE: OCTOBER 13TH 2021</strong><br/>
      TIME: 11:45 - 14:00 CEST
      <span>ADD TO CALENDAR >></span>
    </div>
    <div class="info-box">
      <strong>LOCATION: HIGH TECH CAMPUS 1(E), THE STRIP, 5656 AE EINDHOVEN</strong>
      <span>VIEW ON MAP >></span>
    </div>
  </section>

    <div class="agenda-section">
      <h2>Agenda</h2>
      <table class="agenda-table">
        <tr>
          <td>9:00 AM</td>
          <td>Lorem ipsum dolor sit amet, consectetur adipiscing</td>
        </tr>
        <tr>
          <td>9:30 AM</td>
          <td>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip</td>
        </tr>
        <tr>
          <td>10:00 AM</td>
          <td>Lorem ipsum dolor sit amet, consectetur adipiscing</td>
        </tr>
        <tr>
          <td>10:30 AM</td>
          <td>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla</td>
        </tr>
        <tr>
          <td>11:30 AM</td>
          <td>Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim</td>
        </tr>
        <tr>
          <td>12:30 AM</td>
          <td>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod</td>
        </tr>
      </table>
    </div>
  </section>

  <h3>Our Speakers</h3><br>
  <div class="speakers">
    <div class="speaker-card">
      <img src="https://media.licdn.com/dms/image/v2/D4E03AQEQXxX6g73wBw/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1690404645713?e=2147483647&v=beta&t=qeGsxmVMjRK-VsUNnc7nFrcQCLHrHFP5tv4DFwEV-7U" alt="Speaker">
      <div class="speaker-name">Neil Barua</div>
      <div class="speaker-title">Chief Executive Officer, ServiceMax</div>
    </div>
    <div class="speaker-card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS68rRgLW9v465U5ZQANbENjup5GOw2wfZteQ&s" alt="Speaker">
      <div class="speaker-name">Neil Barua</div>
      <div class="speaker-title">Chief Executive Officer, ServiceMax</div>
    </div>
    <div class="speaker-card">
      <img src="https://res.cloudinary.com/engineering-com/image/fetch/h_175,fl_sanitize,f_auto,fl_lossy,q_auto,g_face:center,w_240,c_fill/https://www.engineering.com/wp-content/uploads/2024/06/122_image001.jpg" alt="Speaker">
      <div class="speaker-name">Neil Barua</div>
      <div class="speaker-title">Chief Executive Officer, ServiceMax</div>
    </div>
    <div class="speaker-card">
      <img src="https://servicecouncil.com/wp-content/uploads/2021/11/ServiceMax-Neil-Barua-Outdoor-126-800px-social.jpg" alt="Speaker">
      <div class="speaker-name">Neil Barua</div>
      <div class="speaker-title">Chief Executive Officer, ServiceMax</div>
    </div>
  </div>

  <div class="countdown-section">
    <h2>Countdown block</h2>
    <p class="countdown-desc">
      Lorem ipsum, dolor sit amet consectetur adipiscing elit. Doloribus nemo vero minus! Necessitatibus ea consequatur sit laudantium voluptatem, voluptates natus vero hic quas! Accusantium nostrum, sunt sequi pariatur illum eos nesciunt necessitatibus.
    </p>
    <p style="font-weight:bold; margin-bottom: 20px;" class="pi">EVENT WILL START IN</p>
    <div class="countdown-timer">
      <div class="time-box">
        <h3 id="days">00</h3>
        <p>DAYS</p>
      </div>
      <div class="time-box">
        <h3 id="hours">00</h3>
        <p>HOURS</p>
      </div>
      <div class="time-box">
        <h3 id="minutes">00</h3>
        <p>MINUTES</p>
      </div>
      <div class="time-box">
        <h3 id="seconds">00</h3>
        <p>SECONDS</p>
      </div>
    </div>
    <br>
    <button class="reserve-btn">RESERVE MY SEAT</button>
  </div>
  
  <script>
    // Set the target date
    const targetDate = new Date("june 10, 2025 00:00:00").getTime();

    // Function to update the countdown timer
    function updateTimer() {
      const now = new Date().getTime();  // Get the current time
      const distance = targetDate - now;  // Get the difference from the target date

      // Calculate time components
      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);

      // Update the HTML
      document.getElementById("days").textContent = days < 10 ? "0" + days : days;
      document.getElementById("hours").textContent = hours < 10 ? "0" + hours : hours;
      document.getElementById("minutes").textContent = minutes < 10 ? "0" + minutes : minutes;
      document.getElementById("seconds").textContent = seconds < 10 ? "0" + seconds : seconds;

      // If the countdown is finished
      if (distance < 0) {
        clearInterval(timerInterval);  // Stop the timer
        document.querySelector(".countdown-timer").innerHTML = "EXPIRED";  // Display the message
      }
    }

    // Update the timer immediately on page load
    updateTimer();
    
    // Update the timer every second
    const timerInterval = setInterval(updateTimer, 1000);
  </script>


    <!-- Videos Section -->
    <div class="videos-section">
      <h2>Videos</h2>
      <div class="video-grid">
        <div class="video-card">
          <iframe width="560" height="315" src="https://www.youtube.com/embed/RIZZ352dU64?si=_N5VL9Hj6YX3xp_d" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
          <div class="video-label">VIDEO</div>
          <div class="video-title">Lorem ipsum dolor sit amet, consectetur adipiscing elit</div><br>
          <div class="video-desc">Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
          <div class="watch-now">
          <img src="https://i.fbcd.co/products/resized/resized-750-500/23eeb00c6621039b01312656125471e24dcba325ebd10c04c98c2550dc0949e1.jpg" alt="Watch Icon">
          </div>
        </div>
        <div class="video-card">
          <iframe width="560" height="315" src="https://www.youtube.com/embed/CHByDKUdPJ4?si=SphbTn2aTssNsUPH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
          <div class="video-label">VIDEO</div>
          <div class="video-title">Lorem ipsum dolor sit amet, consectetur adipiscing elit</div><br>
          <div class="video-desc">Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
          <div class="watch-now">
          <img src="https://i.fbcd.co/products/resized/resized-750-500/23eeb00c6621039b01312656125471e24dcba325ebd10c04c98c2550dc0949e1.jpg" alt="Watch Icon">
          </div>
        </div>
        <div class="video-card">
          <iframe width="560" height="315" src="https://www.youtube.com/embed/CHByDKUdPJ4?si=SphbTn2aTssNsUPH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
          <div class="video-label">VIDEO</div>
          <div class="video-title">Lorem ipsum dolor sit amet, consectetur adipiscing elit</div><br>
          <div class="video-desc">Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
          <div class="watch-now">
          <img src="https://i.fbcd.co/products/resized/resized-750-500/23eeb00c6621039b01312656125471e24dcba325ebd10c04c98c2550dc0949e1.jpg" alt="Watch Icon">
          </div>
        </div>

      </div>
      
      <div class="section-title">Images</div>
      <div class="image-row">
        <div class="image-box">
          <img src="https://t4.ftcdn.net/jpg/02/20/30/11/360_F_220301105_MzErCk0IVgajn30EWFP2mnsO37gCosL0.jpg" alt="Image 1">
          <h4>LOREM IPSUM</h4>
          <h3>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.</h3>
        </div>
        <div class="image-box">
          <img src="https://media.istockphoto.com/id/1004229704/photo/woman-using-a-cordless-drill.jpg?s=612x612&w=0&k=20&c=7UXAD7PfQApwB8gVJM4LR099Tt6JeHCLd-1N0iXwCM8=" alt="Image 2">
          <h4>LOREM IPSUM</h4>
          <h3>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.</h3>
        </div>
      </div>

      <footer>
        <div class="footer-container">
          <div class="footer-column">
            <div class="logo">
              <img src="https://media.licdn.com/dms/image/v2/D4E0BAQGVskimCS992w/company-logo_200_200/company-logo_200_200/0/1723226554790/servicemax_logo?e=2147483647&v=beta&t=JlVsD7E6aep2RtyothgMcif43q_AZ1Glr4CLNocNMdQ" alt="Service-max Logo" />
            </div>
            <h4>CONNECT WITH US</h4>
            <div class="social-icons">
              <a href="#" class="icon"><i class="fab fa-twitter"></i></a>
              <a href="#" class="icon"><i class="fab fa-instagram"></i></a>
              <a href="#" class="icon"><i class="fab fa-linkedin-in"></i></a>
              <a href="#" class="icon"><i class="fab fa-youtube"></i></a>

            </div>
          </div>
    
          <div class="footer-column">
            <h4>GET IN TOUCH</h4>
            <p>1-800-756-4980</p>
            <p>+44 (0) 20 3846 7320</p>
            <p>1-925-391-3516 (support)</p>
            <p>+44 (0) 20 3785 9805 (support)</p>
          </div>
    
          <div class="footer-column">
            <h4>OTHER RESOURCES</h4>
            <a href="#">Contact Us</a><br>
            <a href="#">Support</a><br>
            <a href="#">Sitemap</a>
          </div>
    
          <div class="footer-column">
            <h4>LOGIN</h4>
            <a href="#">ServiceMax Login</a><br>
            <a href="#">Zinc Login</a><br>
            <a href="#">Customer Community Login</a>
          </div>
        </div><br>
        <div class="copyright">
          © 2022 ServiceMax.com. All Rights Reserved.
        </div>
      </footer>
    

</body>
</html>
