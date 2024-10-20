# Data-Science-Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My Data Science Portfolio</title>
    <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #2c3e50;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            margin: 0;
            padding: 10px;
            background-color: #34495e;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
        }
        nav a:hover {
            color: #f39c12;
        }
        .container {
            padding: 20px;
        }
        .intro {
            text-align: center;
            margin-bottom: 40px;
        }
        .project {
            background-color: white;
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

    <header>
        <h1>My Data Science Portfolio</h1>
        <p>Welcome to my portfolio showcasing my data-driven projects!</p>
    </header>

    <nav>
        <a href="#about">About Me</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container">
        <!-- Introduction Section -->
        <section id="about" class="intro">
            <h2>About Me</h2>
            <p>Hello! I'm a data science enthusiast with a passion for analyzing complex datasets to drive impactful insights. 
            I specialize in using Python, SQL, and data visualization tools like Power BI to solve real-world problems. This portfolio contains a few of my exciting projects.</p>
        </section>

        <!-- Project Section -->
        <section id="projects">
            <h2>Featured Project: Climate Change Data Analysis</h2>
            <div class="project">
                <h3>Interactive Chart: Global Temperature Rise</h3>
                <p>Below is an interactive chart showcasing the global rise in temperature over time:</p>
                <div id="myPlot" style="width:100%;height:500px;"></div>
                <script>
                    var trace1 = {
                        x: [1880, 1900, 1920, 1940, 1960, 1980, 2000, 2020],
                        y: [-0.2, -0.1, 0.0, 0.1, 0.2, 0.3, 0.5, 0.8],
                        mode: 'lines+markers',
                        type: 'scatter',
                        name: 'Global Temperature Rise'
                    };

                    var data = [trace1];

                    var layout = {
                        title: 'Global Temperature Anomaly Over Time',
                        xaxis: { title: 'Year' },
                        yaxis: { title: 'Temperature Anomaly (°C)' }
                    };

                    Plotly.newPlot('myPlot', data, layout);
                </script>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="intro">
            <h2>Contact</h2>
            <p>If you'd like to collaborate or learn more about my work, feel free to get in touch with me!</p>
            <p>Email: <a href="mailto:your.email@example.com">your.email@example.com</a></p>
            <p>LinkedIn: <a href="https://www.linkedin.com/in/yourlinkedinprofile" target="_blank">Connect with me</a></p>
        </section>
    </div>

    <footer>
        <p>&copy; 2024 Your Name | Data Science Portfolio</p>
    </footer>

</body>
</html>

