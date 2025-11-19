# Advanced-Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet" />
    <link rel="stylesheet" href="style.css">
    </head>
<body>

    <header>
        <h2>My Portfolio</h2>
        <nav>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="hero-text">
            <h1> Hi,I am </h1>
            <h2>Full Stack Developer</h2>
            <p>Building modern web applications with MERN stack.</p>
           
        </div>
        <img src="image.png" alt="Profile Image" />
    </section>

    <section class="about" id="about">
        <h2>About Me</h2>
        <p>Hello! My name is Sambhav Agarwal, and I am currently learning web development. This is my first portfolio website where I showcase my passion for creating interactive and responsive web pages. I am a student at KR Mangalam University, pursuing a B.Tech degree, and I am deeply interested in technology and coding. I love exploring new skills every day, and I always aim to improve my knowledge in the field of web development. With a hardworking and consistent mindset, I am determined to grow as a developer and build crective projects that makes real impact.</p>
    </section>

    <section class="skills" id="skills">
        <h2> My Skills</h2><br>
        <div class="skills-grid">
            <div class="skill-card">HTML<br><span>Beginner</span></div>
            <div class="skill-card">CSS<br><span>Beginner</span></div>
            <div class="skill-card">JavaScript<br><span>Learning</span></div>
           
        </div>
    </section>

    <section class="projects" id="projects">
        <h2>Projects</h2><br>
        <div class="project-grid">

            <div class="project-card">
                <img src="project 1.png" alt=" Project 1">
                <h3>Project 1</h3> 
                <p>A simple Html and css web pages</p>
                </div>

            <div class="project-card">
                <img src="project 2.png" alt="Project 2">
                <h3>Project 2</h3>
                <p>Another awesome mini project</p>
            
        </div>
    </section>

    <section class="contact" id="contact">
        <div clasas="contact-box"> 
            <h2>Contact Me</h2><br>
            <form>
                <input type="text" placeholder="Your Name" required />
                <input type="email" placeholder="Your Email" required />
                <textarea rows="4" placeholder="Your Message"></textarea>
                <button>Send </button>
            </form>
        </div>
    </section>

    <footer>
        © 2025 Sambhav Agarwal | All Rights Reserved
    </footer>

    <a href="#" class="back-to-top">Back to Top</a>
 

</body>
</html>


STYLES APPLIED
/* External CSS for Responsive Portfolio Website */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "Poppins", sans-serif;
    background: #f9f9f9;
    color: #333;
    line-height: 1.6;
}

/* HEADER */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 5%;
    background: blue;
    color: white;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 100;
}

header nav a {
    margin-left: 2rem;
    text-decoration: none;
    font-size: 1rem;
    color:white;
    transition: color 0.3s ease;
}

header nav a:hover {
    color: #007bff;
   
}

/* HERO SECTION */
.hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 4rem 5%;
}

.hero-text h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero-text h2 {
    font-size: 3rem;
    color: #007bff;
    animation: colorChange 3s infinite alternate;
}

@keyframes colorChange {
    from { color: #007bff; }
    to { color: #ff4b5c; }
}

.hero-text p {
    max-width: 450px;
    margin: 1rem 0;
    font-size: 1rem;
}

.hero-text button {
    padding: 0.8rem 2rem;
    font-size: 1rem;
    border: none;
    border-radius: 5px;
    background: #007bff;
    color: #fff;
    cursor: pointer;
    transition: transform 0.3s ease;
}

.hero-text button:hover {
    transform: scale(1.1);
}

.hero img {
    width: 300px;
    border-radius: 50%;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

/* ABOUT */
.about {
    padding: 4rem 5%;
}

.about h2 {
    font-size: 2.2rem;
    margin-bottom: 1rem;
}

/* SKILLS GRID */
.skills {
    padding: 4rem 5%;
    background: #fff;
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1.5rem;
    
}

.skill-card {
    text-align: center;
    padding: 1.5rem;
    background: blue;
    color: white;
    border-radius: 10px;
    transition: transform 0.3s ease;
    box-shadow: 0 4px 12px rgb(169, 6, 123);
}

.skill-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 8px 20px rgb(169, 6, 123);
   }


/* PROJECTS */
.projects {
    padding: 4rem 5%;
    text-align: center;
}

.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
}

.project-card {
    background: #fff;
    padding: 1.5rem;
    border-radius: 15px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.15);
    transition: transform 0.3s ease , box-shadow 0.3s ease;
}

.project-card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 25px rgba(0,0,0,0.2);
}
/* Project Images */
.project-card img {
    width: 100%;
    height: 180px;
    border-radius: 10px;
    object-fit: cover;
    margin-bottom: 1rem;
}

.project-card h3 {
    margin-bottom: 0.5rem;
    font-size: 1.3rem;
}

.project-card p {
    color: #555;
    font-size: 0.95rem;
}

   /* CONTACT — centered box */ 
.contact {
    padding: 6rem 0;
    background: #f1f1f1;
    display: flex;
    justify-content: center;   /* centers horizontally */
    align-items: center;     /* vertical alignment */
}

.contact-box {
    background: white;
    padding: 2rem;
    width: 520px;
    border-radius: 12px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    
}

form input, form textarea {
    width: 100%;
    padding: 0.9rem;
    margin: 0.9rem 0;
    border: 2px solid skyblue;
    border-radius: 1rem;
}
/* Textarea height  */
form textarea {
    height: 130px;
}

form button {
    padding: 0.9rem;
    background: blue;
    color: white;
    border: none;
    font-size: 1.1rem;
    border-radius: 6px;
    width: 100%;
    cursor: pointer;
}     
/* Button hover */
form button:hover {
    background: #0b2f6b;
}

/* FOOTER */
footer {
    text-align: center;
    padding: 1.5rem;
    background: blue;
    color: white;
}

/* RESPONSIVE */
@media (max-width: 768px) {
    .hero {
        flex-direction: column;
        text-align: center;
    }
    .hero img {
        margin-top: 2rem;
    }
}
/* Back To Top */
.back-to-top {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: blue;
    padding: 10px 18px;
    color: white;
    border-radius: 6px;
    text-decoration: none;
}
