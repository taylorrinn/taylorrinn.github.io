<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Artist Showcase</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }

        header {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px;
        }

        h1 {
            margin: 0;
        }

        nav {
            background-color: #444;
            text-align: center;
            padding: 10px;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 10px;
        }

        .container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .tab-content {
            display: none;
        }

        .active-tab {
            display: block;
        }

        .artwork {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .artwork img {
            max-width: 100%;
            margin: 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Artist Showcase</h1>
    </header>
    <nav>
        <a href="javascript:void(0)" onclick="openTab('home')">Home</a>
        <a href="javascript:void(0)" onclick="openTab('gallery')">Gallery</a>
        <a href="javascript:void(0)" onclick="openTab('about')">About</a>
        <a href="javascript:void(0)" onclick="openTab('contact')">Contact</a>
    </nav>
    <div class="container">
        <div class="tab-content" id="home">
            <h2>Welcome to the Gallery</h2>
            <p>Explore the amazing artworks by our talented artist.</p>
        </div>
        <div class="tab-content" id="gallery">
            <h2>Art Gallery</h2>
            <div class="artwork">
                <img src="image1.jpg" alt="Artwork 1">
                <img src="image2.jpg" alt="Artwork 2">
                <img src="image3.jpg" alt="Artwork 3">
                <!-- Add more artwork images here -->
            </div>
        </div>
        <div class="tab-content" id="about">
            <h2>About the Artist</h2>
            <p>Learn more about our talented artist and their background.</p>
        </div>
        <div class="tab-content" id="contact">
            <h2>Contact Us</h2>
            <p>Get in touch with us for inquiries and more information.</p>
        </div>
    </div>
    <script>
        function openTab(tabName) {
            var tabContents = document.getElementsByClassName('tab-content');
            for (var i = 0; i < tabContents.length; i++) {
                tabContents[i].style.display = 'none';
            }
            document.getElementById(tabName).style.display = 'block';
        }
    </script>
</body>
</html>
