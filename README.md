<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
</head>

<body>
    <header class="header">
        <a href="#" class="logo"><span>Ha</span>la</a>
        <h2 id="active" aria-label="Toggle Navigation"><i id="menu" class='bx bx-menu'></i></h2>
        <nav class="navbar">
            <i id="x" class='bx bx-x' aria-label="Close Navigation"></i>
            <ul>
                <li><a href="#">Services</a></li>
                <li><a href="#">Experience</a></li>
                <li><a href="#">Projects</a></li>
                <li><a href="#">Education</a></li>
                <li><a href="#">Contact Me</a></li>
            </ul>
        </nav>
    </header>

    <section class="home">
        <div class="home-content">
            <h3>Hi! I’m Hala Zohbie <br>a <span class="text sec-text">frontend developer</span></h3>
            <p>I aim to leverage my programming and analytical skills to develop innovative software solutions that
                enhance business efficiency and achieve technical goals. I am committed to continually learning the
                latest technologies and trends in programming and working on projects that are both challenging and
                creative. I also aspire to work in an environment that fosters professional growth and personal skill
                development.</p>
            <div class="btn-box">
                <button class="btn-1">Hire Me</button>
                <button class="btn-2">Experience</button>
            </div>
        </div>
    </section>

    <section class="about">
        <div class="about-img">
            <img src="image.jpeg" alt="About Me Image">
        </div>
        <div class="about-content">
            <h2 class="heading">About <span>Me</span></h2>
            <h3>Frontend <span>Developer</span></h3>
            <p>"Hello! I’m Hala <span>Zohbie</span>, a passionate Front-End Developer with a knack for creating engaging
                and user-friendly web experiences. With a solid background in HTML, CSS, and JavaScript, I specialize in
                building responsive and visually appealing websites that function seamlessly across various devices and
                browsers."</p>
            <a href="#" class="btn-2">Experience</a>
        </div>
    </section>

    <section class="contact-form">
        <h2 class="contact-me">Contact <span>Me</span></h2>
        <form action="#">
            <div class="input-box">
                <input type="text" placeholder="Full Name" required>
                <input type="email" placeholder="Email" required>
            </div>
            <div class="input-box">
                <input type="tel" placeholder="Phone Number" required>
                <input type="text" placeholder="Subject" required>
            </div>
            <textarea name="message" id="message" cols="30" rows="10" placeholder="Your Message" required></textarea>
            <input type="submit" value="Send Message" class="btn-1">
        </form>
    </section>

    <footer class="footer">
        <div class="social">
            <a href="#" aria-label="Facebook"><i class='bx bxl-facebook-circle'></i></a>
            <a href="#" aria-label="LinkedIn"><i class='bx bxl-linkedin-square'></i></a>
            <a href="#" aria-label="Twitter"><i class='bx bxl-twitter'></i></a>
            <a href="#" aria-label="Instagram"><i class='bx bxl-instagram-alt'></i></a>
        </div>
        <ul class="list">
            <li><a href="#">FAQ</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">About Me</a></li>
            <li><a href="#">Contact</a></li>
            <li><a href="#">Privacy Policy</a></li>
        </ul>
        <p class="copyright">&copy; 2024 Hala | All Rights Reserved</p>
    </footer>

    <script>
        const navbare = document.querySelector(".navbar");
        const active = document.getElementById("active");
        const text = document.querySelector(".sec-text");

        const textLoad = () => {
            setTimeout(() => { text.innerHTML = "frontend developer"; }, 0);
            setTimeout(() => { text.innerHTML = "software developer"; }, 4480);
            setTimeout(() => { text.innerHTML = "web developer"; }, 9246);
        };

        textLoad();
        setInterval(textLoad, 13560);

        active.onclick = () => {
            navbare.style.right = "0";
        };

        const x = document.getElementById("x");
        x.onclick = () => {
            navbare.style.right = "-1000px";
        };
    </script>
</body>

</html>
