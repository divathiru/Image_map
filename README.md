# Ex04 Places Around Me
# Date:
10/11/2024
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
imagemap.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>South India Interactive Map</title>
    <style>
        /* Reset and global styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', Arial, sans-serif;
            background-color: #1c1c1e;
            color: #ffffff;
            text-align: center;
            line-height: 1.6;
        }

        h1 {
            margin-top: 20px;
            font-size: 2.5rem;
            color: #00ccff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.6);
        }

        p {
            font-size: 1.2rem;
            margin-bottom: 20px;
            color: #cccccc;
        }

        .map-container {
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 20px;
        }

        img {
            max-width: 90%;
            height: auto;
            border: 4px solid #444;
            border-radius: 12px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.7);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        img:hover {
            transform: scale(1.03);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.9);
        }

        /* Hover effect for clickable areas */
        area {
            cursor: pointer;
        }

        area:hover {
            outline: 3px solid #ff9900;
        }

        footer {
            margin-top: 30px;
            padding: 10px 20px;
            font-size: 0.9rem;
            color: #888;
            border-top: 1px solid #444;
        }

        footer a {
            color: #00ccff;
            text-decoration: none;
            font-weight: bold;
        }

        footer a:hover {
            color: #ff9900;
        }

        /* Add responsiveness for smaller screens */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }

            p {
                font-size: 1rem;
            }

            img {
                max-width: 95%;
            }
        }
    </style>
</head>
<body>
    <h1>South India Interactive Map</h1>
    <p>Click on the highlighted regions below to explore the respective areas.</p>
    
    <div class="map-container">
        <img src="map.png" usemap="#pcmap" alt="South India Map">
    </div>
    
    <map name="pcmap">
        <area shape="rect" coords="469,18,615,68" href="Chennai.html" alt="Chennai" target="_blank">
        <area shape="rect" coords="380,42,455,74" href="https://vkkkkellore.nic.in/about-district/" alt="Vellore" target="_blank">
        <area shape="rect" coords="175,447,328,488" href="https://trivkkkkandrum.nic.in/en/history/" alt="Thiruvananthapuram" target="_blank">
        <area shape="rect" coords="431,135,583,194" href="https://py.kkkkgov.in/about-puducherry" alt="Puducherry" target="_blank">
        <area shape="rect" coords="370,231,475,278" href="Thanjavur.html" alt="Thanjavur" target="_blank">
        <area shape="rect" coords="280,314,386,359" href="https://www.kkkkkktamilnadutourism.tn.gov.in/destinations/madurai" alt="Madurai" target="_blank">
        <area shape="rect" coords="137,87,231,137" href="https://karnakkkkktakatourism.org/tour-item/mysuru/" alt="Mysore" target="_blank">
        <area shape="rect" coords="178,212,349,264" href="Coimbatore.html" alt="Coimbatore" target="_blank">
        <area shape="rect" coords="286,169,422,198" href="tamilnadu.html" alt="Tamil Nadu" target="_blank">
        <area shape="rect" coords="62,198,177,236" href="https://kokkkkzhikode.nic.in/en/about-district/history/" alt="Kaniyakumari" target="_blank">
        <area shape="rect" coords="113,375,212,408" href="https://keralakkkkkhouse.kerala.gov.in/about-the-state-of-kerala" alt="Kerala" target="_blank">
        <area shape="rect" coords="103,311,195,368" href="https://www.kkkk.org/kochi" alt="Kochi" target="_blank">
        <area shape="rect" coords="236,26,350,74" href="Bangalore.html" alt="Bengaluru" target="_blank">
        <area shape="rect" coords="469,553,595,584" href="https://www.kkkkkk.travel/" alt="Sri Lanka" target="_blank">
        <area shape="rect" coords="439,600,554,639" href="https://www.lllllll.in/Tourism-g293962-Colombo_Western_Province-Vacations.html" alt="Colombo" target="_blank">
        <area shape="rect" coords="3,32,76,80" href="https://www.gdhd.gov.in/en/karnataka/mangalore" alt="Mangalore" target="_blank">
    </map>

    <footer>
        &copy; 2024 South India Explorer | Designed by <a href="https://example.com" target="_blank">Thirumurugan</a>
    </footer>
</body>
</html>
~~~
tamilnadu.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Explore Tamil Nadu</title>
    <style>
        /* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
    overflow-x: hidden;
}

/* Header */
header {
    position: relative;
    text-align: center;
    color: white;
    background: url('tamilnadu-header.jpg') no-repeat center center/cover;
    height: 60vh;
}

header .hero {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-image: url('1.jpg');
    background-size: cover;
}

header h1 {
    font-size: 3rem;
    margin-bottom: 10px;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
}

header p {
    font-size: 1.5rem;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
}

/* Navigation */
nav {
    background: #333;
    color: white;
    padding: 10px 0;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    gap: 20px;
}

nav a {
    text-decoration: none;
    color: white;
    font-size: 1.2rem;
    transition: color 0.3s ease;
}

nav a:hover {
    color: #ff9900;
}

/* Section Styles */
.content-section {
    padding: 40px 20px;
    text-align: center;
    background-color: #fff;
    margin: 20px auto;
    max-width: 900px;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}

.content-section h2 {
    font-size: 2.5rem;
    margin-bottom: 20px;
    color: #555;
}

.content-section p {
    font-size: 1.2rem;
    margin-bottom: 20px;
    color: #666;
}

.content-section img {
    max-width: 50%;
    height: auto;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.content-section img:hover {
    transform: scale(1.05);
}

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
    padding: 20px;
}

.gallery-grid img {
    height: 100%;
    width: 100%;
    height: auto;
    aspect-ratio: 4/3; /* Ensures uniform aspect ratio */
    object-fit: cover; /* Ensures images fit well within their container */
    border-radius: 8px;
    box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.gallery-grid img:hover {
    transform: scale(1.1);
}

.i1{
    height: 10vh;
    width: 10vw;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background: #333;
    color: white;
    font-size: 1rem;
}

footer a {
    color: #ff9900;
    text-decoration: none;
}

footer a:hover {
    color: #00ccff;


}

    </style>
</head>
<body>
    <header>
        <div class="hero">
            <h1>Welcome to Tamil Nadu</h1>
            <p>The Land of Temples, Culture, and Heritage</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#culture">Culture</a></li>
            <li><a href="#tourism">Tourism</a></li>
            <li><a href="#cuisine">Cuisine</a></li>
        </ul>
    </nav>

    <section id="culture" class="content-section">
        <h2>Culture</h2>
        <p>Tamil Nadu is known for its rich cultural heritage. From Bharatanatyam, a classical dance form, to Carnatic music, Tamil Nadu boasts a vibrant artistic tradition. The Tamil language, one of the world's oldest languages, is a cornerstone of the state's identity.</p>
        <img src="1.jpg" alt="Tamil Nadu Culture">
    </section>

    <section id="tourism" class="content-section">
        <h2>Tourism</h2>
        <p>Explore iconic destinations like Meenakshi Amman Temple in Madurai, Marina Beach in Chennai, and the Nilgiris in Ooty. Tamil Nadu is also home to UNESCO World Heritage sites like the Group of Monuments at Mahabalipuram and the Brihadisvara Temple.</p>
        <img src="1.jpg" style="height: 30vh; width: 100%;" alt="Tamil Nadu Tourism" class="i1">
    </section>

    <section id="cuisine" class="content-section">
        <h2>Cuisine</h2>
        <p>Experience the authentic flavors of Tamil Nadu with dishes like idli, dosa, sambar, filter coffee, and Chettinad chicken curry. The state’s cuisine is a mix of vegetarian and non-vegetarian delicacies.</p>
        <img src="1.jpg" alt="Tamil Nadu Cuisine">
    </section>



    <footer>
        <p>&copy; 2024 Explore Tamil Nadu. Designed by Thirumurugan.</p>
    </footer>
</body>
</html>
~~~
~~~
chennai.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Discover Chennai - the vibrant capital of Tamil Nadu, India. Explore its culture, cuisine, and iconic landmarks.">
    <meta name="keywords" content="Chennai, Tamil Nadu, India, Marina Beach, Culture, Cuisine, Tourism">
    <meta name="author" content="Your Name">
    <title>Discover Chennai</title>
    <style>
        /* General styles */
        body {
            margin: 0;
            font-family: 'Lato', Arial, sans-serif;
            line-height: 1.6;
            background: #f8f9fa;
            color: #333;
        }

        /* Header styling */
        header {
            background-image: url("1.jpg");
            background-size: cover;
            color: white;
            text-align: center;
            padding: 2rem 1rem;
        }
        header h1 {
            font-size: 2.5rem;
            margin: 0;
        }
        header p {
            font-size: 1.2rem;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: center;
            background: #333;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        nav a {
            color: white;
            padding: 0.8rem 1.5rem;
            text-decoration: none;
            text-transform: uppercase;
            font-size: 1rem;
            transition: background 0.3s;
        }
        nav a:hover {
            background: #ff7e5f;
        }

        /* Section styling */
        section {
            padding: 2rem 10%;
        }
        section h2 {
            font-size: 2rem;
            color: #ff7e5f;
            margin-bottom: 1rem;
        }
        section p {
            font-size: 1.1rem;
            margin-bottom: 1rem;
        }

        /* Image container */
        .image {
            display: flex;
            justify-content: center;
            margin: 2rem 0;
        }
        .image img {
            max-width: 100%;
            height: 500px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        /* List styles */
        ul, ol {
            margin: 1rem 0;
            padding: 0 1.5rem;
        }
        ul li, ol li {
            margin-bottom: 0.5rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 1rem;
            background: #333;
            color: white;
            font-size: 0.9rem;
        }

        /* Media Queries */
        @media (max-width: 768px) {
            section {
                padding: 2rem 5%;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Discover Chennai</h1>
        <p>The Gateway to South India's Rich Heritage</p>
    </header>
    <nav>
        <a href="#about">About</a>
        <a href="#landmarks">Landmarks</a>
        <a href="#cuisine">Cuisine</a>
        <a href="#culture">Culture</a>
    </nav>
    <section id="about">
        <h2>About Chennai</h2>
        <p>Chennai, formerly known as Madras, is the capital of Tamil Nadu and one of India’s most vibrant cities. It is renowned for its cultural heritage, modern infrastructure, and thriving economy.</p>
        <div class="image">
            <img src="1.jpg" alt="Chennai City Skyline">
        </div>
    </section>
    <section id="landmarks">
        <h2>Famous Landmarks</h2>
        <p>Chennai is home to numerous iconic landmarks that blend history and modernity:</p>
        <ul>
            <li><strong>Marina Beach:</strong> The second-longest urban beach in the world.</li>
            <li><strong>Kapaleeshwarar Temple:</strong> A masterpiece of Dravidian architecture.</li>
            <li><strong>Fort St. George:</strong> A historical site reflecting British colonial influence.</li>
        </ul>
        <div class="image">
            <img src="1.jpg" alt="Kapaleeshwarar Temple">
        </div>
    </section>
    <section id="cuisine">
        <h2>Cuisine</h2>
        <p>Chennai’s cuisine offers an irresistible combination of tradition and flavor. Here are some must-try dishes:</p>
        <ol>
            <li><strong>Idli and Dosa:</strong> Staple breakfast items served with chutneys and sambar.</li>
            <li><strong>Chettinad Chicken:</strong> A spicy dish from the Chettinad region.</li>
            <li><strong>Filter Coffee:</strong> A quintessential South Indian beverage.</li>
        </ol>
        <div class="image">
            <img src="1.jpg" alt="South Indian Cuisine">
        </div>
    </section>
    <section id="culture">
        <h2>Culture and Festivals</h2>
        <p>Chennai is the cultural heart of Tamil Nadu. It celebrates art, music, and dance through grand festivals like:</p>
        <ul>
            <li><strong>Margazhi Music Festival:</strong> A showcase of Carnatic music and traditional performances.</li>
            <li><strong>Pongal:</strong> A harvest festival marking Tamil Nadu’s cultural pride.</li>
            <li><strong>Deepavali:</strong> The festival of lights celebrated with grandeur.</li>
        </ul>
        <div class="image">
            <img src="1.jpg" alt="Carnatic Music Performance">
        </div>
    </section>
    <footer>
        <p>&copy; 2024 Discover Chennai. Designed with passion for culture and heritage.</p>
    </footer>
</body>
</html>
~~~
~~~
Coimbatore.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome to Coimbatore</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-image: url("1.jpg");
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 50px 20px;
        }
        header h1 {
            font-size: 2.5rem;
            margin: 0;
        }
        header p {
            font-size: 1.2rem;
            margin-top: 10px;
        }
        nav {
            background-color: #333;
            overflow: hidden;
        }
        nav a {
            float: left;
            color: white;
            text-decoration: none;
            padding: 14px 20px;
            text-align: center;
            font-weight: 600;
        }
        nav a:hover {
            background-color: #4CAF50;
            color: white;
        }
        section {
            padding: 20px;
            max-width: 900px;
            margin: 20px auto;
            background: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        section h2 {
            color: #4CAF50;
            margin-top: 0;
        }
        section ul {
            padding-left: 20px;
        }
        section ul li {
            margin-bottom: 10px;
        }
        footer {
            text-align: center;
            padding: 10px 0;
            background: #4CAF50;
            color: white;
            margin-top: 20px;
        }
        img {
            max-width: 100%;
            border-radius: 8px;
            margin-top: 10px;
        }
        a {
            color: #4CAF50;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Coimbatore</h1>
        <p>The Manchester of South India</p>
    </header>
    <nav>
        <a href="#about">About</a>
        <a href="#attractions">Attractions</a>
        <a href="#culture">Culture</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="about">
        <h2>About Coimbatore</h2>
        <p>Coimbatore, also known as Kovai, is a dynamic city in Tamil Nadu, India. Nestled by the Western Ghats and known for its textile industry, it is often referred to as the "Manchester of South India."</p>
        <img src="1.jpg" alt="Aerial view of Coimbatore">
    </section>
    <section id="attractions">
        <h2>Top Attractions</h2>
        <ul>
            <li><strong>Marudamalai Temple:</strong> A serene hilltop temple dedicated to Lord Murugan.</li>
            <li><strong>Isha Yoga Center:</strong> Home to the iconic 112-foot Adiyogi statue.</li>
            <li><strong>VOC Park and Zoo:</strong> A delightful spot for families and kids.</li>
            <li><strong>Siruvani Waterfalls:</strong> Known for its crystal-clear and sweet-tasting water.</li>
        </ul>
        <img src="1.jpg" alt="Adiyogi statue at Isha Yoga Center">
    </section>
    <section id="culture">
        <h2>Culture and Lifestyle</h2>
        <p>Coimbatore boasts a rich cultural heritage, vibrant festivals like Pongal and Diwali, and a delightful cuisine. From aromatic filter coffee to crispy dosas, the city's culinary offerings are a treat for food enthusiasts.</p>
    </section>
    <section id="contact">
        <h2>Contact Us</h2>
        <p>For inquiries and information, email us at <a href="mailto:info@coimbatore.com">info@coimbatore.com</a>.</p>
    </section>
    <footer>
        <p>&copy; 2024 Explore Coimbatore. All rights reserved.</p>
    </footer>
</body>
</html>
~~~
~~~
Thanjavur.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thanjavur - The Land of Art and Culture</title>
    <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@300;600&family=Playfair+Display:ital,wght@1,500&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* General Styling */
        body {
            font-family: 'Raleway', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #f9f9f9, #eaf2f8);
            color: #333;
        }
        header {
            background-image: url("https://media.istockphoto.com/id/1198023306/photo/thanjavur-brihadeeswara-temple-image.jpg?s=612x612&w=0&k=20&c=JqGIQfzFlOLI5wcHEuE2G2sdv208C96aUTZKx2a0QX4=");
            background-size: cover;
            color: white;
            padding: 30px 10px;
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: 3em;
            font-style: italic;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #555;
            font-size: 1.2em;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 15px 25px;
            font-family: 'Roboto', sans-serif;
            font-weight: bold;
            transition: background 0.3s, color 0.3s;
        }
        nav a:hover {
            background-color: #81c784;
            color: black;
        }
        main {
            padding: 20px;
        }
        section {
            margin: 30px 0;
            padding: 20px;
            border-radius: 10px;
            background: white;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5em;
            margin-bottom: 10px;
            color: #4caf50;
        }
        p, ul {
            font-size: 1.1em;
            line-height: 1.8;
        }
        ul {
            padding-left: 20px;
        }
        .content {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .card {
            background: #fff;
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            max-width: 300px;
            overflow: hidden;
            text-align: left;
            transition: transform 0.3s;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .card img {
            width: 100%;
            border-bottom: 3px solid #4caf50;
            height: 300px;
        }
        .card h3 {
            font-family: 'Raleway', sans-serif;
            font-size: 1.5em;
            color: #4caf50;
            padding: 10px 15px;
        }
        .card p {
            padding: 0 15px 15px;
        }
        footer {
            background: #4caf50;
            color: white;
            text-align: center;
            padding: 10px 0;
            font-size: 1em;
            font-family: 'Roboto', sans-serif;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        .highlight {
            color: #e57373;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <header>Welcome to Vibrant Thanjavur</header>
    <nav>
        <a href="#history">History</a>
        <a href="#culture">Culture</a>
        <a href="#landmarks">Landmarks</a>
        <a href="#gallery">Gallery</a>
    </nav>
    <main>
        <section id="history">
            <h2>History of Thanjavur</h2>
            <p>
                Thanjavur, a city of historical grandeur, served as the heart of the Chola dynasty. Known for its rich 
                cultural heritage, it boasts the <span class="highlight">Brihadeeswarar Temple</span>, a UNESCO World Heritage Site.
            </p>
        </section>
        <section id="culture">
            <h2>Culture and Traditions</h2>
            <div class="content">
                <div class="card">
                    <img src="1.jpg" alt="Brihadeeswarar Temple">
                    <h3>Brihadeeswarar Temple</h3>
                    <p>A magnificent example of Chola architecture, known for its towering vimana.</p>
                </div>
                <div class="card">
                    <img src="1.jpg" alt="Thanjavur Paintings">
                    <h3>Thanjavur Paintings</h3>
                    <p>Famous for their intricate details and gold foiling, these artworks are a visual treat.</p>
                </div>
            </div>
        </section>
        <section id="landmarks">
            <h2>Must-Visit Landmarks</h2>
            <ul>
                <li>The Great Living Chola Temples</li>
                <li>Thanjavur Royal Palace</li>
                <li>Saraswathi Mahal Library</li>
                <li>Punnai Nallur Mariamman Temple</li>
            </ul>
        </section>
        <section id="gallery">
            <h2>Gallery</h2>
            <div class="content">
                <div class="card">
                    <img src="1.jpg" alt="Saraswathi Mahal Library">
                    <h3>Saraswathi Mahal Library</h3>
                    <p>One of the oldest libraries in Asia, holding ancient manuscripts and rare texts.</p>
                </div>
                <div class="card">
                    <img src="1.jpg" alt="Thanjavur Landscape">
                    <h3>Thanjavur Landscape</h3>
                    <p>The vibrant blend of culture and natural beauty makes this city a true gem.</p>
                </div>
            </div>
        </section>
    </main>
    <footer>&copy; 2024 Explore Thanjavur. All Rights Reserved.</footer>
</body>
</html>
~~~
~~~
Bangalore.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Discover Bangalore</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            background-color: #f4f8fb;
            line-height: 1.6;
        }

        h1, h2 {
            margin: 0;
        }

        a {
            text-decoration: none;
        }

        /* Hero Section */
        .hero {
            background: url('1.jpg') no-repeat center center/cover;
            color: white;
            text-align: center;
            padding: 60px 20px;
            box-shadow: inset 0 0 0 2000px rgba(0, 0, 0, 0.4);
        }

        .hero h1 {
            font-size: 3rem;
            font-family: 'Playfair Display', serif;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.4rem;
            font-family: 'Lobster', cursive;
            color: #f7d794;
        }

        /* Content Section */
        .content {
            padding: 20px;
        }

        .content article {
            margin-bottom: 30px;
        }

        .content h2 {
            font-family: 'Roboto Slab', serif;
            font-size: 2rem;
            color: #34495e;
            margin-bottom: 10px;
        }

        .content p {
            font-size: 1.2rem;
            color: #2c3e50;
        }

        /* Image Grid */
        .image-grid {
            display: flex;
            gap: 20px;
            margin: 20px 0;
        }

        .image-grid div {
            flex: 1;
            text-align: center;
        }

        .image-grid img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease-in-out;
            height: 300px;
        }

        .image-grid img:hover {
            transform: scale(1.05);
        }

        .image-grid p {
            margin-top: 10px;
            font-family: 'Poppins', sans-serif;
            font-size: 1rem;
            color: #555;
        }

        /* Footer Section */
        footer {
            text-align: center;
            padding: 15px;
            background-color: #2c3e50;
            color: white;
            font-size: 0.9rem;
        }

        footer a {
            color: #f7d794;
        }
    </style>
</head>
<body>
    <header class="hero">
        <h1>Welcome to Bangalore</h1>
        <p>Your Gateway to Endless Opportunities</p>
    </header>

    <section class="content">
        <article>
            <h2>About Bangalore</h2>
            <p>
                Known as the "Garden City" and "Silicon Valley of India," Bangalore is a bustling metropolis 
                full of opportunities, culture, and greenery. Whether you're here for the thriving tech scene 
                or the vibrant lifestyle, Bangalore welcomes you with open arms.
            </p>
        </article>

        <div class="image-grid">
            <div>
                <img src="1.jpg" alt="Bangalore Palace">
                <p>The Majestic Bangalore Palace</p>
            </div>
            <div>
                <img src="1.jpg" alt="Cubbon Park">
                <p>Relax at Cubbon Park</p>
            </div>
            <div>
                <img src="1.jpg" alt="Tech Parks">
                <p>Innovative Tech Parks</p>
            </div>
        </div>

        <article>
            <h2>Why Bangalore?</h2>
            <p>
                Bangalore is more than just a city—it's a lifestyle. Enjoy pleasant weather year-round, 
                explore world-class dining, and witness a melting pot of cultures. It's no surprise that 
                millions call it home.
            </p>
        </article>
    </section>

    <footer>
        <p>&copy; 2024 Discover Bangalore | Designed by <a href="#">Thirumurugan</a></p>
    </footer>
</body>
</html>
~~~
# OUTPUT
![Screenshot 2024-12-06 211218](https://github.com/user-attachments/assets/fd4e2507-73c1-4c90-8f7e-737bfedfbe98)

![Screenshot 2024-12-06 211310](https://github.com/user-attachments/assets/05c47e4e-a560-4db6-ba7e-a05136c43572)

![Screenshot 2024-12-06 211329](https://github.com/user-attachments/assets/0f6d6c4a-a526-48a7-9815-fa5797b2644d)

![Screenshot 2024-12-06 211346](https://github.com/user-attachments/assets/46d4eec7-728f-4b08-a232-4cfc436965c2)

![Screenshot 2024-12-06 211456](https://github.com/user-attachments/assets/7ffc02cf-a91e-490c-98fb-e87c9b28ca61)

![Screenshot 2024-12-06 211520](https://github.com/user-attachments/assets/09cd991d-d311-46cb-9de9-c258fe1d69be)

![Screenshot 2024-12-06 211533](https://github.com/user-attachments/assets/8d9cc30b-0e36-4f96-9c22-9c45688837c5)

![Screenshot 2024-12-06 211547](https://github.com/user-attachments/assets/9a18886f-f41a-492d-8650-c5cbc503d4a4)

![Screenshot 2024-12-06 211559](https://github.com/user-attachments/assets/d3269e41-88c9-46d1-be33-79ae2df52b83)

![Screenshot 2024-12-06 211610](https://github.com/user-attachments/assets/25745c62-e393-4782-a37e-f14ff5ff16ce)

![Screenshot 2024-12-06 211636](https://github.com/user-attachments/assets/3446305f-ad73-44cc-aeb2-75f67b40859b)

![Screenshot 2024-12-06 211726](https://github.com/user-attachments/assets/d97b2ebd-9083-4e13-bc67-acf8d224c049)

![Screenshot 2024-12-06 211755](https://github.com/user-attachments/assets/aeffa5d3-1d31-4eef-ab9c-f335f5635da1)

![Screenshot 2024-12-06 211809](https://github.com/user-attachments/assets/f71fb3b3-f279-4422-a1d0-b67eb1c841e9)

![Screenshot 2024-12-06 211826](https://github.com/user-attachments/assets/91dfeeb7-a862-45f1-9e96-dc98227515e4)

![Screenshot 2024-12-06 211840](https://github.com/user-attachments/assets/80c0f816-4860-4f74-9771-059f41527dfa)

![Screenshot 2024-12-06 212010](https://github.com/user-attachments/assets/ccc82547-0ad7-49e0-9a5c-2fbfcfb61095)

![Screenshot 2024-12-06 212027](https://github.com/user-attachments/assets/bc6d87eb-24af-4417-bbe2-da30569e51db)

![Screenshot 2024-12-06 212049](https://github.com/user-attachments/assets/9d59cae8-894c-4c1e-80e9-9a3147b92615)

![Screenshot 2024-12-06 212100](https://github.com/user-attachments/assets/d11f1db1-41c8-4158-919a-66cd86f7f046)



# RESULT
The program for implementing image maps using HTML is executed successfully.
