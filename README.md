# Odoo_hackathon
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SKILL SWAP</title>
  <!--custom cdn link!-->  

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">

    <!--custom css file link-->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!--header section starts-->
<header class="header">
    <section class="flex">
        <a href="#home" class="logo">SKILL SWAP</a>
        <nav class="navbar">
            <a href="#home">home</a>
            <a href="#about">about</a>
            <a href="#reviews">reviews</a>
            <a href="#contact">contact</a>
            <a href="login.html" class="login-btn-header">Login</a>
            <a href="profile.html" class="nav-link">Profile</a>
            <a href="public-profile.html">Public Profile</a>
           

           

        </nav>
        <div id="menu-btn" class="fas fa-bars"></div>
    </section>
</header>









     <!--header section ends-->

     <!-- home section starts -->
<section class="home" id="home">
    <div class="container">
        <div class="filters">
            <select name="availability" class="dropdown">
                <option value="">Availability</option>
                <option value="available">Available</option>
                <option value="unavailable">Unavailable</option>
            </select>
            <input type="text" placeholder="Search skills..." class="search-bar">
            <button class="search-btn">Search</button>
        </div>

        <div class="profile-cards">

            <!-- Profile Card 1 -->
            <div class="profile-card">
                <div class="profile-info">
                    <div class="photo">Profile Photo</div>
                    <div class="details">
                        <h3>Mare Demo</h3>
                        <p><strong>Skills Offered:</strong> JavaScript, Python</p>
                        <p><strong>Skills Wanted:</strong> Music, Graphic Design</p>
                        <p>Rating: 3.4 / 5</p>
                    </div>
                </div>
               <label for="show-login-popup" class="request-btn">Request</label>


            </div>

            <!-- Repeat for other users -->
            <div class="profile-card">
                <div class="profile-info">
                    <div class="photo">Profile Photo</div>
                    <div class="details">
                        <h3>Michelle</h3>
                        <p><strong>Skills Offered:</strong> JavaScript, Python</p>
                        <p><strong>Skills Wanted:</strong> Music, Graphic Design</p>
                        <p>Rating: 2.5 / 5</p>
                    </div>
                </div>
              <label for="show-login-popup" class="request-btn">Request</label>


            </div>

            <div class="profile-card">
                <div class="profile-info">
                    <div class="photo">Profile Photo</div>
                    <div class="details">
                        <h3>Joe Wills</h3>
                        <p><strong>Skills Offered:</strong> JavaScript, Python</p>
                        <p><strong>Skills Wanted:</strong> Music, Graphic Design</p>
                        <p>Rating: 4.0 / 5</p>
                    </div>
                </div>
            <label for="show-login-popup" class="request-btn">Request</label>


            </div>

        </div>
    </div>
</section>
<!-- home section ends -->

<div class="pagination">
    <button class="page-btn" disabled>&laquo; Prev</button>
    <button class="page-number active">1</button>
    <button class="page-number">2</button>
    <button class="page-number">3</button>
    <button class="page-btn">Next &raquo;</button>
</div>


<!-- Login Required Popup -->
<div class="login-popup" id="login-popup">
  <div class="login-popup-content">
    <p>Please login to send a request.</p>
    <a href="login.html" class="login-popup-btn">Go to Login</a>
  </div>
</div>
<input type="checkbox" id="show-login-popup" hidden>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login | Skill SWAP</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <header class="header">
        <section class="flex">
            <a href="/" class="logo">Skill Swap Platform</a>
            <nav class="navbar">
                <a href="/">Home</a>
            </nav>
        </section>
    </header>

    <!-- Login Form Section -->
    <section class="login-section">
        <form action="/login" method="POST" class="login-form">
            <h2>Login</h2>

            <label for="email">Email</label>
            <input type="email" name="email" id="email" required placeholder="Enter your email">

            <label for="password">Password</label>
            <input type="password" name="password" id="password" required placeholder="Enter your password">

            <button type="submit" class="login-btn">Login</button>

            <a href="/forgot-password" class="forgot-link">Forgot username/password?</a>
        </form>
    </section>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>User Profile | Skill Swap</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Header -->
  <header class="header">
    <section class="flex">
      <a href="#" class="logo">Skill Swap Platform</a>

      <div class="header-controls">
        <a href="#" class="save-btn">Save</a>
        <a href="#" class="discard-btn">Discard</a>
        <a href="#" class="nav-link">Swap request</a>
        <a href="index.html" class="nav-link">Home</a>
        <div class="profile-avatar">👤</div>
      </div>
    </section>
  </header>

  <!-- Profile Form Section -->
  <section class="profile-section">
    <form class="profile-form">

      <div class="left-side">
        <label>Name</label>
        <input type="text" />

        <label>Location</label>
        <input type="text" />

        <label>Skills Offered</label>
        <div class="skills">
          <span class="skill-tag">Graphic Design <span class="remove">✕</span></span>
          <span class="skill-tag">Video Editing <span class="remove">✕</span></span>
          <span class="skill-tag">Photoshop <span class="remove">✕</span></span>
        </div>

        <label>Availability</label>
        <input type="text" value="weekends"/>

        <label>Profile</label>
        <input type="text" value="Public"/>
      </div>

      <div class="right-side">
        <div class="photo-box">
          <div class="photo">Profile Photo</div>
          <p class="photo-options">Add/Edit <span class="remove-photo">Remove</span></p>
        </div>

        <label>Skills Wanted</label>
        <div class="skills">
          <span class="skill-tag">Python <span class="remove">✕</span></span>
          <span class="skill-tag">Design <span class="remove">✕</span></span>
          <span class="skill-tag">HR <span class="remove">✕</span></span>
        </div>
      </div>

    </form>
  </section>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Public Profile | Skill Swap</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Header -->
  <header class="header">
    <section class="flex">
      <a href="#" class="logo">SKILL SWAP </a>

      <div class="header-controls">
      
       
        <a href="index.html" class="nav-link">Home</a>
        <button onclick="window.location.href='choose.html'" class="request-btn">Request</button>
        <div class="profile-avatar">👤</div>
      </div>
    </section>
  </header>

  <!-- Public Profile Content -->
  <section class="public-profile">
    <div class="profile-box">

      <div class="left">
        <h2>Marc Demo</h2>

        <div class="info-block">
          <strong>Skills Offered:</strong>
          <p>JavaScript, Python</p>
        </div>

        <div class="info-block">
          <strong>Skills Wanted:</strong>
          <p>Graphic Design, Music</p>
        </div>

        <div class="info-block">
          <strong>Rating and Feedback:</strong>
          <p>⭐ 3.8/5 — "Very helpful and responsive!"</p>
        </div>
      </div>

      <div class="right">
        <div class="photo-circle">Profile Photo</div>
      </div>
      <div class="info-block">
    <strong>Feedback:</strong>
    <ul class="feedback-list">
      <li>"Very friendly and helpful!"</li>
      <li>"Good communication skills."</li>
      <li>"Delivered on time and taught well."</li>
    </ul>
  </div>

    </div>
  </section>

</body>
</html>





:root{
    --green:#00E77F;
    --white:#FFF;
    --light-white:#aaa;
    --black:#3d3d3d;
    --light-bg:#4b4b4b
}
*{
    font-family: 'Rubik',sans-serif;
    margin: 0;  
    padding: 0;
    box-sizing:border-box ;
    outline: no;
}

::-webkit-scrollbar{
    height: .5rem;
    width: 1rem;

}
::-webkit-scrollbar-track{
    background-color: transparent;
}
::-webkit-scrollbar-thumb{
    background-color: var(--green);
    border-radius: 5rem;

}
body{
    background-color: var(--black);
}
section{
    max-width: 1200px;
    margin: 0 auto;
    padding: 2rem;

}
.header{
    position: fixed;
    top: 0;left: 0;right: 0;
    z-index: 1000;
    background-color: var(--light-bg);
}
.header .flex{
    position: relative;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.header .flex .logo{
    font-size: 2.5rem;
    color: var(--white);
}
.header .flex .navbar a{
    margin-left: 2rem;
    color: var(--light-white);
    font-size: 2rem;

}
.header .flex .navbar a:hover{
    color: var(--green);
}
#menu-btn{
    cursor: pointer;
    color: var(--white);
    font-size: 2.5rem;
    display: none;
}
#menu-btn.fa-times{
    transform: rotate(180deg);
}








/*media queries*/
@media(max-width:991px){
    html{
        font-size: 55%;

    }
}
@media(max-width:768px){
    
    #menu-btn{
     display: inline-block;
   }
    .header .flex .navbar{
     position: absolute;
     top: 99%; left:0; right: 0;
     border-top: .1rem solid var(--light-white);
     border-bottom: 1rem solid var(--light-white);
     background-color: var(--light-bg);

}   


}
   /* .header .flex .navbar a{
     display: block;
     margin: 2rem;

}*/
        


@media(max-width:450px){
    html{
        font-size: 50%;
        
    }
}


@import url('https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300..900;1,300..900&display=swap');

:root{
    --green:#00E77F;
    --white:#FFF;
    --light-white:#aaa;
    --black:#3d3d3d;
    --light-bg:#4b4b4b;


}

*{
    font-family: 'Rubik',sans-serif;
    margin: 0;padding: 0;
    box-sizing: border-box;
    outline: none;border:none;
    text-decoration: none;
    transition: 2s linear;
    text-transform: capitalize;
}
*::selection{
    background-color: var(--black);
    color:var(--black);
}

html{
    font-size: 62.5%;
    overflow-x: hidden;
    scroll-behavior:smooth ;
    scroll-padding-top: 8rem;
}

::-webkit-scrollbar {
    height: .5rem;
    width: 1rem;
}
::-webkit-scrollbar-track {
    background-color: var(--black);
}
::-webkit-scrollbar-thumb {
    background-color: var(--green);
    border-radius: 5rem;
}

.header {
    background: var(--black);
    color: var(--white);
    position: fixed;
    width: 100%;
    top: 0;
    left: 0;
    z-index: 1000;
    padding: 1rem 2rem;
}
.header .flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.navbar a {
    margin: 0 1rem;
    font-size: 1.5rem;
    color: var(--white);
}
#menu-btn {
    font-size: 2rem;
    color: var(--white);
    cursor: pointer;
}

/*login*/
.login-btn-header {
    padding: 0.8rem 1.6rem;
    font-size: 1.4rem;
    background-color: var(--green);
    color: #000;
    border-radius: 0.5rem;
    text-align: center;
    white-space: nowrap;
}
.login-btn-header:hover {
    background-color: #00c76d;
}


.home {
    padding: 10rem 2rem 2rem;
    background-color: #000;
    color: var(--white);
}
.container {
    max-width: 1200px;
    margin: auto;
}
.filters {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin-bottom: 2rem;
    align-items: center;
}
.dropdown,
.search-bar,
.search-btn {
    padding: 1rem;
    font-size: 1.5rem;
    border-radius: 0.5rem;
    border: none;
}
.search-btn {
    background-color: var(--green);
    color: #000;
    cursor: pointer;
}
.profile-cards {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}
.profile-card {
    background-color: var(--light-bg);
    border: 1px solid var(--light-white);
    border-radius: 1rem;
    padding: 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}
.profile-info {
    display: flex;
    gap: 1.5rem;
    align-items: center;
}
.photo {
    background: var(--white);
    color: var(--black);
    width: 7rem;
    height: 7rem;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
}
.details h3 {
    font-size: 2rem;
    margin-bottom: 0.5rem;
}
.details p {
    font-size: 1.4rem;
    margin: 0.2rem 0;
}
.request-btn {
    background-color: var(--green);
    color: #000;
    padding: 1rem 2rem;
    font-size: 1.4rem;
    border-radius: 0.5rem;
    cursor: pointer;
}
/* Popup styles */
.login-popup {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  display: none;
  justify-content: center;
  align-items: center;
  z-index: 1000;
}

.login-popup-content {
  background: #fff;
  padding: 30px;
  text-align: center;
  border-radius: 10px;
  width: 80%;
  max-width: 300px;
}

.login-popup-btn {
  display: inline-block;
  margin-top: 15px;
  padding: 8px 16px;
  background-color: #4CAF50;
  color: #fff;
  text-decoration: none;
  border-radius: 5px;
}

/* Show popup when checkbox is checked */
#show-login-popup:checked + .login-popup {
  display: flex;
}



/*login page*/

.login-section{
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #000;
    padding: 2rem;
}
.login-form {
    background-color: var(--light-bg);
    border-radius: 1rem;
    padding: 3rem 4rem;
    width: 100%;
    max-width: 400px;
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.1);
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}
.login-form h2 {
    text-align: center;
    color: var(--white);
    font-size: 2.4rem;
    margin-bottom: 1rem;
}
.login-form label {
    color: var(--white);
    font-size: 1.4rem;
}
.login-form input {
    padding: 1rem;
    font-size: 1.5rem;
    border-radius: 0.5rem;
    border: none;
    background-color: var(--white);
}
.login-btn {
    padding: 1rem;
    font-size: 1.6rem;
    background-color: var(--green);
    color: #000;
    border-radius: 0.5rem;
    cursor: pointer;
    margin-top: 1rem;
}
.forgot-link {
    color: #6EC1E4;
    font-size: 1.3rem;
    text-align: center;
    text-decoration: underline;
    margin-top: 1rem;
}

/*profile*/
/* ========== Profile Page Styles ========== */

.profile-section {
    margin-top: 8rem;
    padding: 2rem;
    background-color: #000;
    color: var(--white);
    display: flex;
    justify-content: center;
}

.profile-form {
    display: flex;
    flex-wrap: wrap;
    gap: 3rem;
    width: 100%;
    max-width: 1000px;
    justify-content: space-between;
    border: 1px solid var(--white);
    border-radius: 1rem;
    padding: 3rem;
}

.left-side,
.right-side {
    flex: 1 1 45%;
    display: flex;
    flex-direction: column;
    gap: 1.8rem;
}

.profile-form label {
    font-size: 1.6rem;
}

.profile-form input {
    padding: 0.8rem 1.2rem;
    font-size: 1.5rem;
    border-radius: 0.6rem;
    border: 1px solid var(--white);
    background-color: transparent;
    color: var(--white);
}

.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
}

.skill-tag {
    background-color: var(--light-bg);
    border-radius: 2rem;
    padding: 0.4rem 1.2rem;
    font-size: 1.3rem;
    display: flex;
    align-items: center;
    gap: 0.4rem;
    border: 1px solid var(--green);
}

.remove {
    color: red;
    font-weight: bold;
    cursor: pointer;
}

/* Profile Photo Section */
.photo-box {
    text-align: center;
    margin-top: 2rem;
}

.photo {
    width: 10rem;
    height: 10rem;
    border-radius: 50%;
    background-color: var(--white);
    color: var(--black);
    display: flex;
    align-items: center;
    justify-content: center;
    margin: auto;
    font-size: 1.2rem;
}

.photo-options {
    margin-top: 1rem;
    font-size: 1.3rem;
    color: var(--white);
}

.remove-photo {
    color: red;
    cursor: pointer;
}

/* Header Buttons */
.header-controls {
    display: flex;
    align-items: center;
    gap: 1.5rem;
}

.save-btn {
    color: limegreen;
    font-size: 1.5rem;
    text-decoration: none;
}

.discard-btn {
    color: red;
    font-size: 1.5rem;
    text-decoration: none;
}

.nav-link {
    color: var(--white);
    font-size: 1.4rem;
    text-decoration: none;
}

.profile-avatar {
    width: 3.5rem;
    height: 3.5rem;
    border-radius: 50%;
    background: #fff;
    color: #000;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.6rem;
}

/* Mobile Responsive  */
@media (max-width: 768px) {
    .profile-form {
        flex-direction: column;
    }

    .left-side, .right-side {
        width: 100%;
    }

    .header-controls {
        flex-wrap: wrap;
        gap: 1rem;
    }
}


/* ======== Public Profile Page ======== */
.public-profile {
    padding: 15rem;
    margin-top: 8rem;
    background-color: #000;
    color: var(--white);
    display: flex;
    justify-content: center;
    border-radius: 1%;
}

.profile-box {
    border: 1px solid var(--white);
    border-radius: 1rem;
    padding: 3rem;
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    width: 100%;
    max-width: 1000px;
    justify-content: space-between;
}

.left {
    flex: 1 1 60%;
}

.right {
    flex: 1 1 30%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.left h2 {
    font-size: 2.4rem;
    margin-bottom: 1.5rem;
}

.info-block {
    margin-bottom: 1.5rem;
    
}
.feedback-list {
  list-style-type: disc;
  margin-left: 2rem;
  font-size: 1.3rem;
  line-height: 1.8rem;
  color: var(--light-white);
}

.info-block p {
    font-size: 1.4rem;
    margin-top: 0.4rem;
}

/* Profile Photo */
.photo-circle {
    width: 12rem;
    height: 12rem;
    border-radius: 50%;
    background-color: var(--white);
    color: var(--black);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.2rem;
}

/* Request button (top left) */
.request-btn-header {
    padding: 0.6rem 1.4rem;
    background-color: var(--green);
    color: #000;
    border-radius: 2rem;
    font-size: 1.3rem;
    text-align: center;
    text-decoration: none;
}

/* Mobile responsive */
@media (max-width: 768px) {
    .profile-box {
        flex-direction: column;
        padding: 2rem;
    }

    .right {
        justify-content: flex-start;
    }

    .photo-circle {
        margin-top: 1rem;
    }
}


.choose-request {
  padding: 6rem 3rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.request-form {
  background: var(--light-bg);
  padding: 3rem;
  border-radius: 1rem;
  max-width: 500px;
  width: 100%;
  color: var(--white);
  font-size: 1.4rem;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  box-shadow: 0 0 10px rgba(255, 255, 255, 0.05);
}

.request-form h2 {
  text-align: center;
  margin-bottom: 1rem;
  font-size: 2rem;
}

.request-form label {
  font-weight: 500;
}

.request-form select,
.request-form textarea {
  padding: 1rem;
  border-radius: 0.5rem;
  border: none;
  font-size: 1.4rem;
  width: 100%;
}

.submit-btn {
  background-color: var(--green);
  color: #000;
  font-size: 1.4rem;
  padding: 1rem;
  border-radius: 2rem;
  border: none;
  cursor: pointer;
  margin-top: 1rem;
  width: 100%;
}

<!-- choose.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Skill Swap - Send Request</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header class="header">
    <section class="flex">
      <a href="index.html" class="logo">Skill Swap Platform</a>
    </section>
  </header>

  <section class="choose-request">
    <form class="request-form">
      <h2>Send Skill Swap Request</h2>

      <label for="offered-skill">Choose one of your offered skills</label>
      <select id="offered-skill" required>
        <option value="" disabled selected>Select a skill</option>
        <option value="JavaScript">JavaScript</option>
        <option value="Python">Python</option>
        <option value="Photoshop">Photoshop</option>
      </select>

      <label for="wanted-skill">Choose one of their wanted skills</label>
      <select id="wanted-skill" required>
        <option value="" disabled selected>Select a skill</option>
        <option value="Graphic Design">Graphic Design</option>
        <option value="Music">Music</option>
      </select>

      <label for="message">Message</label>
      <textarea id="message" rows="5" placeholder="Write your message..."></textarea>

      <button type="submit" class="submit-btn">Submit</button>
    </form>
  </section>
</body>
</html>





  
