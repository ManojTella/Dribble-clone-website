# Create-a-simplified-clone-of-Dribbble-landing-page
## AIM:To create a simplified clone of Dribble Landing Page
### program:
### index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">Dribbble</div>
            <ul class="nav-links">
                <li><a href="#">Inspiration</a></li>
                <li><a href="#">Find Work</a></li>
                <li><a href="#">Learn Design</a></li>
                <li><a href="#">Go Pro</a></li>
                <li><a href="#">Hire Designers</a></li>
            </ul>
            <div class="auth-buttons">
                <button class="login">Log in</button>
                <button class="sign-up">Sign up</button>
            </div>
        </nav>
    </header>
    <main>
        <section class="hero">
            <h1>Discover the world’s top designers & creatives</h1>
            <p>Dribbble is the leading destination to find & showcase creative work and home to the world's best design professionals.</p>
            <button class="cta-button">Explore Now</button>
        </section>
        <section class="gallery-container">
            <div class="gallery">
                <div class="gallery-item"><img src="img1.png" alt="Image 1"></div>
                <div class="gallery-item"><img src="img2.png" alt="Image 2"></div>
                <div class="gallery-item"><img src="img3.png" alt="Image 3"></div>
                <div class="gallery-item"><img src="img4.png" alt="Image 4"></div>
                <div class="gallery-item"><img src="img5.png" alt="Image 5"></div>
                <div class="gallery-item"><img src="img6.png" alt="Image 6"></div>
            </div>
        </section>
    </main>
    <footer>
        <p>© 2024 Dribbble. All rights reserved.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>

```
## Styles.css
```
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    overflow-x: hidden;
}

header {
    background-color: transparent;
    border-bottom: 1px solid #ddd;
    padding: 20px 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    transition: background-color 0.3s;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
}

.nav-links li {
    display: inline;
}

.nav-links a {
    text-decoration: none;
    color: #333;
    transition: color 0.3s;
}

.nav-links a:hover {
    color: #ea4c89;
}

.auth-buttons button {
    margin-left: 10px;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s, color 0.3s;
}

.auth-buttons .login {
    background-color: #f3f3f3;
}

.auth-buttons .sign-up {
    background-color: #ea4c89;
    color: #fff;
}

.auth-buttons .login:hover {
    background-color: #ddd;
}

.auth-buttons .sign-up:hover {
    background-color: #d13b6f;
}

.hero {
    text-align: center;
    padding: 150px 20px;
    background-color: #f5f5f5;
    transition: background-color 0.5s;
}

.hero h1 {
    font-size: 36px;
    margin-bottom: 20px;
    animation: fadeIn 2s ease-in-out;
}

.hero p {
    font-size: 18px;
    color: #666;
    animation: fadeIn 2s ease-in-out 0.5s;
}

.cta-button {
    padding: 15px 30px;
    background-color: #ea4c89;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
    margin-top: 20px;
    transition: background-color 0.3s, transform 0.3s;
}

.cta-button:hover {
    background-color: #d13b6f;
    transform: scale(1.05);
}

.gallery-container {
    overflow: hidden;
    white-space: nowrap;
}

.gallery {
    display: flex;
    animation: scroll 20s linear infinite;
}

.gallery-item {
    display: inline-block;
    padding: 0 1
    
    
    0px;
}

.gallery-item img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: 10px;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #fff;
    border-top: 1px solid #ddd;
    transition: background-color 0.5s;
}

footer p {
    margin: 0;
    color: #666;
}

@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

@keyframes scroll {
    from {
        transform: translateX(0);
    }
    to {
        transform: translateX(-50%);
    }
}

```
## Script.js
```
document.addEventListener('DOMContentLoaded', function () {
    const header = document.querySelector('header');
    const hero = document.querySelector('.hero');

    // Change header background on scroll
    window.addEventListener('scroll', function () {
        if (window.scrollY > 50) {
            header.style.backgroundColor = '#fff';
        } else {
            header.style.backgroundColor = 'transparent';
        }
    });

    // Change hero and footer background color periodically
    setInterval(() => {
        hero.style.backgroundColor = hero.style.backgroundColor === 'rgb(245, 245, 245)' ? '#e5e5e5' : '#f5f5f5';
        document.querySelector('footer').style.backgroundColor = document.querySelector('footer').style.backgroundColor === 'rgb(255, 255, 255)' ? '#f9f9f9' : '#fff';
    }, 3000);
});
```

## Output:
![image](https://github.com/21003698/Create-a-simplified-clone-of-Dribbble-landing-page./assets/93427522/c3e4975a-7511-4dd1-9b15-827c6794cc2c)

## Result:
Thus,Creating a simplified clone of Dribbble landing-page was done successfully.
