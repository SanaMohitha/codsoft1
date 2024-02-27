<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="stylesheet.css">
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'> 

</head>
<body>
    <header class="header">
        <a href="#" class="logo">Portfolio</a>
        <nav class="navbar">
            <a href="#">Home</a>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#resume">Resume</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <section class="home">
        <div class="home-content">
            <div class="text-container">
                <h1>Sana Mohitha</h1>
                <h2>And I'm a Web Developer<span class="text"></span></h2>
                <p>Student at NSRIT College, passionate about crafting beautiful and functional web experiences.</p>
                <p>With a solid foundation in HTML, CSS, and JS, I'm dedicated to bringing creative ideas to life on the web.</p>
            </div>
            <div class="home-sci">
                <img src="mm.jpg" alt="Profile Image">
                <a href="#"><i class="bx bxl-facebook"></i></a>
                <a href="#"><i class="bx bxl-instagram"></i></a>
                <a href="#"><i class="bx bxl-linkedin"></i></a>
                <a href="#"><i class="bx bxl-whatsapp"></i></a>
            </div>
            <a href="#" class="btn-box">More About Me</a>
        </div>
    </section>
    <section id="about" class="about">
        <div class="about-content">
            <h2>About Me</h2>
            <p>I am a web developer with expertise in HTML, CSS, JavaScript, and various web development frameworks. I have experience in building responsive and user-friendly websites and web applications. My passion for coding and problem-solving drives me to continuously learn and improve my skills.</p>
        </div>
    </section>
    <section id="skills"class="skills">
        <div class="skills-content">
            <h2>Skills</h2>
            <ul>
                <li>HTML5</li>
                <li>CSS3</li>
                <li>JavaScript</li>
                
            </ul>
        </div>
    </section>
    <section id="projects" class="projects">
        <div class="projects-content">
            <h2>Projects</h2>
            <div class="project">
                <h3>BMI Calculator</h3>
                <p>The BMI Calculator App is a mobile application developed using Android Studio that enables users to calculate their Body Mass Index (BMI) quickly and accurately. BMI is a widely used metric to assess a person's body weight relative to their height and is commonly used as an indicator of overall health.</p>
                <img src="project1.jpg">
           
        </div>
    </section>
    <section id="resume"class="resume">
        <div class="resume-content">
            <h2>Resume</h2>
            <a href="your_resume.pdf" download>Download Resume (PDF)</a>
        </div>
    </section>
    <section id="contact" class="contact">
        <div class="contact-content">
            <h2>Contact Me</h2>
            <p>Email: mohithasana@gmail.com</p>
            <p>Phone: 9133868583</p>
        </div>
    </section>
    <footer class="footer">
        <p>&copy; 2024 Sana Mohitha. All rights reserved.</p>
        <nav class="footer-nav">
            <a href="#">Privacy Policy</a>
            <a href="#">Terms of Service</a>
        </nav>
    </footer>
    
</body>
</html>





stylesheet.css
*
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins',sans-serif;
}
body
{
    color:aliceblue;
    background-color: rgb(31, 31, 75);
}
.header
{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 20px 10%;
    background: transparent;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 1000;
}
.logo{
    position: relative;
    font-size: 25px;
    color: aliceblue;
    text-decoration: none;
    font-weight: 600;

}

.navbar a {
    display: inline-block;
    font-size: 25px;
    color: aliceblue;
    text-decoration:none ;
    font-weight: 500;
    margin-left: 35px;
    transition: .3s;
}
.navbar a:hover{
    color:rgb(29, 124, 179)
}
.home{
    position: relative;
    width: 100%;
    justify-content: space-between;
    height: 100vh;
   background-color: rgb(31, 31, 75);
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    padding: 70px 10% 0;

}
.home-content {
    display: flex;
    align-items: center;
    flex-direction: column; /* Add this line to stack items vertically */
}
.home-content h2{
    font-size: 32px;
    font-weight: 700;
}
.home-content h2 span{ 
    color: rgb(29, 124, 179);
}
.home-content h2 : :nth-of-type(2){
    margin-bottom 30px;
}
.home-content h1{
    font-size: 56px;
    font-weight: 700;
}
.home-content p{
    font-size: 20px;
}
.home-sci {
    margin-top: 20px;
    margin-right: 20px;
    text-align: center; /* Align text to center */
}
.home-sci img {
    width: 300px; /* Adjust width as needed */
    height: 300px; /* Adjust height as needed */
    border-radius: 50%; /* Create circular shape */
    margin-left: auto;
    transition: transform 0.3s ease; /* Add hover transition */
    position: absolute; /* Position the container relatively to its nearest positioned ancestor */
    right: 10%; /* Position it to the left side */
    top: 40%; /* Optionally adjust the top position */
}

.home-sci img:hover {
    transform: scale(1.1); 
    box-shadow: 0 0 5px lightskyblue,
    0 0 25px lightskyblue ,0 0 50px lightskyblue,
    0 0 100px lightskyblue ,0 0 200px lightskyblue/* Add hover effect */
}
.home-sci a{
    display: inline-flex;
    justify-self: center;
    align-items: center;
    width: 40px;
    height: 40px;
    background: transparent;
    border: 2px solid rgb(62, 135, 218);
    border-radius: 50%;
    font-size: 20px;
    color:rgb(62, 135, 218);
    text-decoration: none;
    margin: 30px 15px 30px 0 ;
}
.home-sci a:hover{
    background:rgb(62, 135, 218);
    color: black;
    box-shadow: 0 0 20px rgb(62, 135, 218);
}
.btn-box{
    display: inline-block;
    padding: 12px 28px;
    background: rgb(62, 135, 218);
    border-radius: 40px;
    font-size: 16px;
    color: black;
    letter-spacing: 1px;
    text-decoration: solid;
    font-weight: 600;

}
.btn-box:hover{
    box-shadow: 0 0 5px lightskyblue,
    0 0 25px lightskyblue ,0 0 50px lightskyblue,
    0 0 100px lightskyblue ,0 0 200px lightskyblue


}
.about-content{
    margin-top: 50px;

    padding: 20px;
    border-radius: 10px;
}
.about-content h2 {
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 20px;
}


.skills-content {
    margin-top: 50px;

    padding: 20px;
    border-radius: 10px;

}

.skills-content h2 {
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 20px;
}

.skills-content ul {
    list-style-type: none;
}

.skills-content li {
    font-size: 20px;
    margin-bottom: 10px;
}

.projects-content {
    margin-top: 50px;

    padding: 20px;
    border-radius: 10px;
}

.projects-content h2 {
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 20px;
}

.project {
    margin-bottom: 40px;
}

.project h3 {
    font-size: 24px;
    font-weight: 700;
    margin-bottom: 10px;
}

.project p {
    font-size: 18px;
}

.project img {
    width: 100%;
    max-width: 400px;
    height: auto;
    margin-top: 10px;
}

.resume-content {
    margin-top: 50px;
  
    padding: 20px;
    border-radius: 10px;
}

.resume-content h2 {
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 20px;
}

.resume-content a {
    display: inline-block;
    padding: 10px 20px;
    background-color: rgb(62, 135, 218);
    border-radius: 5px;
    font-size: 20px;
    color: black;
    text-decoration: none;
    font-weight: 600;
    transition: background-color 0.3s;
}

.resume-content a:hover {
    background-color: rgb(29, 124, 179);
}

.contact-content {
    margin-top: 50px;
   
    padding: 20px;
    border-radius: 10px;
}

.contact-content h2 {
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 20px;
}

.contact-content p {
    font-size: 20px;
    margin-bottom: 10px;
}

.footer {
    margin-top: 50px;
    background-color: rgb(31, 31, 75);
    color: aliceblue;
    text-align: center;
    padding: 20px;
}

.footer p {
    font-size: 16px;
}

.footer-nav {
    margin-top: 20px;
}

.footer-nav a {
    font-size: 16px;
    color: aliceblue;
    text-decoration: none;
    margin: 0 10

