<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio - Motion & Visuals</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            overflow-x: hidden;
        }
        header {
            text-align: center;
            background-color: #333;
            color: white;
            padding: 20px;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        header h1 {
            margin: 0;
            font-size: 3rem;
            letter-spacing: 2px;
        }
        section {
            padding: 50px 20px;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 10px;
            transition: transform 0.4s ease;
        }
        .gallery img:hover {
            transform: scale(1.1);
        }
        .large-images img {
            grid-column: span 2;
        }
        .small-images img {
            grid-column: span 1;
        }

        /* Motion and Animation */
        .fade-in {
            animation: fadeIn 2s ease forwards;
            opacity: 0;
        }
        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }
        .slide-up {
            animation: slideUp 2s ease forwards;
            transform: translateY(100%);
            opacity: 0;
        }
        @keyframes slideUp {
            0% {
                transform: translateY(100%);
                opacity: 0;
            }
            100% {
                transform: translateY(0);
                opacity: 1;
            }
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
    </header>

    <section class="large-images fade-in">
        <div class="gallery">
            <img src="images/large-image1.jpg" alt="Large Image 1">
            <img src="images/large-image2.jpg" alt="Large Image 2">
        </div>
    </section>

    <section class="small-images slide-up">
        <div class="gallery">
            <img src="images/small-image1.jpg" alt="Small Image 1">
            <img src="images/small-image2.jpg" alt="Small Image 2">
            <img src="images/small-image3.jpg" alt="Small Image 3">
            <img src="images/small-image4.jpg" alt="Small Image 4">
        </div>
    </section>

    <footer>
        <p>&copy; 2024 My Portfolio. All Rights Reserved.</p>
    </footer>
</body>
</html>

