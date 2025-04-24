<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Portfolio</title>
    <style>
        /* General Styling */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f6f9;
            color: #333333;
        }

        header {
            background: #0f084b;
            color: white;
            padding: 20px 10px;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        header h1 {
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            margin-top: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 10px 15px;
            margin: 0 5px;
            background: #42cc8e;
            border-radius: 5px;
            transition: background 0.3s;
        }
        nav a:hover {
            background: #2991a3;
        }

        section {
            padding: 50px 10px;
            text-align: center;
        }
        .container {
            max-width: 800px;
            margin: auto;
        }

        /* Home Section */
        #home img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
            object-fit: cover;
            margin-top: 20px;
        }

        /* Skills Section */
        #skills ul {
            list-style: none;
            padding: 0;
        }
        #skills li {
            background: #e3e3f3;
            padding: 10px;
            margin: 10px auto;
            border-radius: 5px;
            max-width: 300px;
        }

        /* Projects Section */
        #projects .project {
            background: #eaeaf5;
            padding: 20px;
            margin: 20px auto;
            border-radius: 5px;
            max-width: 600px;
            text-align: left;
        }

        /* Education Section */
        #education ul {
            list-style: none;
            padding: 0;
        }
        #education li {
            background: #ececff;
            padding: 10px;
            margin: 10px auto;
            border-radius: 5px;
            max-width: 400px;
        }

        /* Contact Section */
        form {
            max-width: 400px;
            margin: auto;
        }
        form input, form textarea, form button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
            border: 1px solid #cccccc;
        }
        form button {
            background: #b1ff63;
            color: white;
            border: none;
            cursor: pointer;
            transition: background 0.3s;
        }
        form button:hover {
            background: #ccaa42;
        }

        footer {
            background: #6c63ff;
            color: rgb(122, 14, 14);
            padding: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <header>
        <h1>Student Portfolio</h1>
        <nav>
            <a href="#About">Home</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#education">Education</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section id="About">
        <div class="container">
            <h2>WELCOME</h2>
            <img src="soubrah.png" alt="Profile Picture">
            <p>Hello! I'm Saurabh, student of bachelor of technology in Computer Science .</p>
        </div>
    </section>

    <section id="skills">
        <div class="container">
            <h2>SKILLS</h2>
            <ul>
                <li>Programming: Python, Java, C++</li>
                <li>Web Development: HTML, CSS </li>
                <li>Design: remini, Canva</li>
                <li>Problem-Solving</li>
            </ul>
        </div>
    </section>

    <section id="projects">
        <div class="container">
            <h2>Projects</h2>
            <div class="project">
                <h3>Project 1: Personal Portfolio</h3>
                <p>A responsive portfolio showcasing my skills and projects. Built with HTML, CSS, and JavaScript.</p>
            </div>
            <div class="project">
                <h3>Project 2: Signature verification</h3>
                <p>An interactive project and successful project. Developed using Python</p>
            </div>
        </div>
    </section>

    <section id="education">
        <div class="container">
            <h2>Education</h2>
            <ul>
                <li>Bachelor of Science in Computer Science (2023-2027)</li>
                <li>secondary education (Science Stream, 2022-2023)</li>

            </ul>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Contact Me</h2>
            <form id="contactForm" onsubmit="submitForm(event)">
                <input type="text" id="name" name="name" placeholder="Your Name" required>
                <input type="email" id="email" name="email" placeholder="Your Email" required>
                <textarea id="message" name="message" rows="4" placeholder="Your Message" required></textarea>
                <button type="submit">Send</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Saurabh. All Rights Reserved.</p>
    </footer>

    <script>
        function submitForm(event) {
            event.preventDefault();
            alert('Thank you for reaching out! I will get back to you soon.');
        }
    </script>
</body>
</html>
