<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Institute of Digital Risk</title>

    <link rel="stylesheet" href="style.css">

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

</head>

<body>

    <header>

        <div class="logo">IDR</div>

        <nav>
            <a href="#about">About</a>
            <a href="#services">Services</a>
            <a href="#community">Community</a>
            <a href="#contact">Contact</a>
        </nav>

    </header>

    <section class="hero">

        <h1>Advancing the Future of Digital Risk</h1>

        <p>
            The Institute of Digital Risk trains and deploys the next generation of digital
            risk professionals through academic partnerships and real-world industry projects.
        </p>

        <button class="btn">Explore Programs</button>

    </section>

    <section id="about">

        <h2 class="section-title">About IDR</h2>

        <p>
            The Institute of Digital Risk (IDR) is an industry-led training and deployment
            institute focused on digital, cyber and technology risk. Our mission is to
            prepare professionals for high-consequence environments where security,
            governance and compliance are critical.
        </p>

        <p>
            Working closely with university partners and industry experts, IDR combines
            academic insight with real-world implementation projects, ensuring that
            graduates develop practical experience in managing digital risk frameworks.
        </p>

    </section>

    <section id="services">

        <h2 class="section-title">Our Model</h2>

        <div class="cards">

            <div class="card">
                <h3>Academy</h3>
                <p>
                    Bootcamps and professional training programs designed to prepare students and
                    practitioners for digital risk careers.
                </p>
            </div>

            <div class="card">
                <h3>Innovation & Incubation</h3>
                <p>
                    Research and development of next-generation risk models, AI governance
                    frameworks and digital trust technologies.
                </p>
            </div>

            <div class="card">
                <h3>Advisory Services</h3>
                <p>
                    Helping organisations implement industry frameworks such as NIST, ISO 27001
                    and NIS2 for secure digital operations.
                </p>
            </div>

        </div>

    </section>

    <section>

        <h2 class="section-title">Train → Hire → Innovate → Deploy</h2>

        <div class="pipeline">

            <div class="step">
                <h4>Train</h4>
                <p>Bootcamps</p>
            </div>

            <div class="step">
                <h4>Hire</h4>
                <p>Industry placement</p>
            </div>

            <div class="step">
                <h4>Innovate</h4>
                <p>Research projects</p>
            </div>

            <div class="step">
                <h4>Deploy</h4>
                <p>Enterprise solutions</p>
            </div>

        </div>

    </section>

    <section id="community">

        <h2 class="section-title">Our Community</h2>

        <p>
            IDR supports a growing community of students, early-career professionals and
            industry practitioners working in sectors such as financial services,
            technology companies and critical infrastructure.
        </p>

    </section>

    <section id="contact">

        <h2 class="section-title">Register Interest</h2>

        <form class="contact-form">

            <input type="text" placeholder="Name" required>

            <input type="email" placeholder="Email" required>

            <textarea rows="4" placeholder="Message"></textarea>

            <button class="btn">Submit</button>

        </form>

    </section>

    <footer>

        <p>© 2026 Institute of Digital Risk</p>

    </footer>

    <script src="script.js"></script>

</body>

</html>



* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    line-height: 1.6;
    color: #111;
}

header {
    position: sticky;
    top: 0;
    background: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 40px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    z-index: 100;
}

.logo {
    font-weight: 600;
    font-size: 20px;
    color: #FF6B00;
}

nav a {
    margin-left: 20px;
    text-decoration: none;
    color: #111;
}

nav a:hover {
    color: #FF6B00;
}

.hero {
    height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: linear-gradient(to right, #111, #333);
    color: white;
    padding: 20px;
}

.hero h1 {
    font-size: 40px;
    margin-bottom: 15px;
}

.hero p {
    max-width: 600px;
    margin-bottom: 20px;
}

.btn {
    background: #FF6B00;
    color: white;
    padding: 12px 25px;
    border: none;
    cursor: pointer;
    border-radius: 4px;
}

.btn:hover {
    background: #e65c00;
}

section {
    padding: 70px 10%;
}

.section-title {
    font-size: 28px;
    margin-bottom: 20px;
}

.cards {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

.card {
    flex: 1;
    min-width: 250px;
    background: #f5f5f5;
    padding: 25px;
    border-radius: 8px;
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-5px);
}

.pipeline {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    margin-top: 20px;
}

.step {
    flex: 1;
    text-align: center;
    min-width: 120px;
}

.contact-form {
    display: flex;
    flex-direction: column;
    max-width: 400px;
}

.contact-form input,
.contact-form textarea {
    margin-bottom: 10px;
    padding: 10px;
    border: 1px solid #ccc;
}

footer {
    background: #111;
    color: white;
    text-align: center;
    padding: 20px;
}

@media(max-width:768px) {

    .hero h1 {
        font-size: 28px;
    }

    .cards {
        flex-direction: column;
    }

}



document.querySelectorAll('nav a').forEach(link => {

    link.addEventListener('click', function(e) {

        e.preventDefault()

        const target = document.querySelector(this.getAttribute('href'))

        target.scrollIntoView({
            behavior: 'smooth'
        })

    })

})