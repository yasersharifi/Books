<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Book Library Navigation</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            text-align: center;
            margin-bottom: 30px;
            padding: 20px;
            background-color: #2c3e50;
            color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .categories {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 20px;
        }
        
        .category {
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .category:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }
        
        .category h2 {
            color: #2c3e50;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 2px solid #e8e8e8;
        }
        
        .books {
            list-style-type: none;
        }
        
        .books li {
            margin-bottom: 10px;
            padding: 8px;
            background-color: #f8f9fa;
            border-radius: 4px;
            transition: background-color 0.2s ease;
        }
        
        .books li:hover {
            background-color: #e9ecef;
        }
        
        .books a {
            color: #3498db;
            text-decoration: none;
            display: block;
        }
        
        .books a:hover {
            color: #2980b9;
            text-decoration: underline;
        }
        
        @media (max-width: 768px) {
            .categories {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Technical Book Library</h1>
            <p>Navigate through various programming and technical resources</p>
        </header>
        
        <div class="categories">
            <!-- Common Category -->
            <div class="category">
                <h2>Common</h2>
                <ul class="books">
                    <li><a href="./Common/Clean Code.pdf">Clean Code.pdf</a></li>
                    <li><a href="./Common/Uncle Bob Clean Architecture.pdf">Uncle Bob Clean Architecture.pdf</a></li>
                    <li><a href="./Common/Pragmatic The Pragmatic Programmer.pdf">Pragmatic The Pragmatic Programmer.pdf</a></li>
                </ul>
            </div>
            
            <!-- DDD Category -->
            <div class="category">
                <h2>DDD</h2>
                <ul class="books">
                    <li><a href="./DDD/Domain-Driven Design Tackling Complexity in the Heart of Software.pdf">Domain-Driven Design Tackling Complexity in the Heart of Software.pdf</a></li>
                </ul>
            </div>
            
            <!-- Docker Category -->
            <div class="category">
                <h2>Docker</h2>
                <ul class="books">
                    <li><a href="./Docker/01.Docker Cookbook.pdf">01.Docker Cookbook.pdf</a></li>
                </ul>
            </div>
            
            <!-- Get Senior Category -->
            <div class="category">
                <h2>Get Senior</h2>
                <ul class="books">
                    <li><a href="./Get Senior/The-managers-path-a-guide-for-tech-leaders-camille-fournier.pdf">The Manager's Path: A Guide for Tech Leaders</a></li>
                </ul>
            </div>
            
            <!-- Git And Github Category -->
            <div class="category">
                <h2>Git And Github</h2>
                <ul class="books">
                    <li><a href="./Git And Github/01.Beginning Git and GitHub.pdf">Beginning Git and GitHub.pdf</a></li>
                </ul>
            </div>
            
            <!-- javascript Category -->
            <div class="category">
                <h2>JavaScript</h2>
                <ul class="books">
                    <li><a href="./javascript/01.JavaScript The Good Parts.pdf">JavaScript The Good Parts.pdf</a></li>
                    <li><a href="./javascript/02.Eloquent JavaScript.pdf">Eloquent JavaScript.pdf</a></li>
                    <li><a href="./javascript/03.You Dont Know Js.pdf">You Don't Know JS.pdf</a></li>
                    <li><a href="./javascript/04.Learning Javascript Design Patterns A Javascript and React Developer's Guide.pdf">Learning JavaScript Design Patterns</a></li>
                    <li><a href="./javascript/05.Learning Javascript Data Structures and Algorithms.pdf">Learning JavaScript Data Structures and Algorithms.pdf</a></li>
                </ul>
            </div>
            
            <!-- Microservice Category -->
            <div class="category">
                <h2>Microservice</h2>
                <ul class="books">
                    <li><a href="./Microservice/Building Microservices, 2nd Edition-Sam Newman-O'Reilly.pdf">Building Microservices, 2nd Edition</a></li>
                    <li><a href="./Microservice/Designing Data-Intensive Applications The Big Ideas Behind Reliable, Scalable, and Maintainable Systems.pdf">Designing Data-Intensive Applications</a></li>
                </ul>
            </div>
            
            <!-- React Category -->
            <div class="category">
                <h2>React</h2>
                <ul class="books">
                    <li><a href="./React/React Cookbook-David Griffiths, Dawn Griffiths-O'Reilly.pdf">React Cookbook</a></li>
                    <li><a href="./React/React Hooks In Actions.pdf">React Hooks In Actions.pdf</a></li>
                </ul>
            </div>
            
            <!-- Sql Category -->
            <div class="category">
                <h2>SQL</h2>
                <ul class="books">
                    <li><a href="./Sql/01.OReilly Designing Data Intensive Applications.pdf">O'Reilly Designing Data Intensive Applications.pdf</a></li>
                    <li><a href="./Sql/02.The Art Of Postgresql.pdf">The Art Of PostgreSQL.pdf</a></li>
                    <li><a href="./Sql/03.SQL Cookbook, 2nd Edition-Anthony Molinaro, Robert de Graaf-O'Reilly.pdf">SQL Cookbook, 2nd Edition</a></li>
                </ul>
            </div>
            
            <!-- System Design Category -->
            <div class="category">
                <h2>System Design</h2>
                <ul class="books">
                    <li><a href="./System Design/Linkedin_Posts_2024_Blue.pdf">LinkedIn Posts 2024 Blue.pdf</a></li>
                    <li><a href="./System Design/Mark_Richards_Neal_Ford_Fundamentals_of_Software_Architecture_An.pdf">Fundamentals of Software Architecture</a></li>
                    <li><a href="./System Design/modern_software_V1_1_2.pdf">Modern Software V1.1.2.pdf</a></li>
                    <li><a href="./System Design/SystemDesignInterview.pdf">System Design Interview.pdf</a></li>
                </ul>
            </div>
        </div>
    </div>
</body>
</html>