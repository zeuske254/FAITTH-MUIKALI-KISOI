# FAITTH-MUIKALI-KISOI
To host your HTML and CSS files in a new folder, follow these steps:

### 1. Organize Your Project Structure

Create a new folder named `my-website` and organize your files within this folder. Your project structure should look like this:

```
my-website/
├── index.html
├── css/
│   └── styles.css
├── img/
│   └── bg.jpg
└── README.md (optional)
```

### 2. Create HTML and CSS Files

Inside the `my-website` folder, create an `index.html` file and a `css` folder. Inside the `css` folder, create a `styles.css` file.

**index.html:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
    <link rel="stylesheet" href="css/styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Ubuntu&display=swap" rel="stylesheet">
</head>
<body class="background">
    <header class="navbar">
        <div class="logo">
            <img src="img/logo.png" alt="Logo">
        </div>
        <ul class="nav-list">
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
        <div class="rightNav">
            <input type="text" id="search" placeholder="Search...">
        </div>
        <div class="burger">
            <div class="line"></div>
            <div class="line"></div>
            <div class="line"></div>
        </div>
    </header>
    <section class="firstSection">
        <div class="box-main">
            <div class="firstHalf">
                <h1 class="text-big">Welcome to My Website</h1>
                <p class="text-small">Your description here.</p>
                <button class="btn">Learn More</button>
                <button class="btn btn-dark">Get Started</button>
            </div>
            <div class="secondHalf">
                <img src="img/profile.jpg" alt="Profile Picture">
            </div>
        </div>
    </section>
    <footer class="text-footer">
        &copy; 2024 My Website. All rights reserved.
    </footer>
</body>
</html>
```

**css/styles.css:**
```css
@import url('https://fonts.googleapis.com/css2?family=Ubuntu&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Ubuntu', sans-serif;
}

.logo {
    width: 20%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.logo img {
    width: 26%;
    border: 3px solid white;
    border-radius: 50px;
    margin: 5px;
}

.navbar {
    display: flex;
    align-items: center;
    justify-content: center;
    position: sticky;
    top: 0;
    background-color: rgba(0, 0, 0, 0.7);
    cursor: pointer;
    z-index: 1000;
}

.nav-list {
    width: 70%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.nav-list li {
    list-style: none;
    padding: 26px 30px;
}

.nav-list li a {
    text-decoration: none;
    color: white;
    font-size: 20px;
}

.nav-list li a:hover {
    color: rgb(197, 194, 194);
}

.rightNav {
    width: 30%;
    text-align: right;
    padding: 0 23px;
}

#search {
    padding: 5px;
    font-size: 17px;
    border: 2px solid grey;
    border-radius: 9px;
}

.background {
    background: rgba(0, 0, 0, 0.7) url('../img/bg.jpg') no-repeat center center/cover;
    background-blend-mode: darken;
}

.firstSection {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    text-align: center;
}

.box-main {
    max-width: 50%;
    margin: auto;
    padding: 20px;
    text-align: center;
}

.firstHalf {
    width: 80%;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.secondHalf {
    width: 30%;
}

.secondHalf img {
    width: 70%;
    border: 4px solid white;
    border-radius: 150px;
    display: block;
    margin: auto;
}

.text-big {
    font-size: 41px;
    margin-bottom: 20px;
}

.text-small {
    font-size: 18px;
    margin-bottom: 20px;
}

.btn {
    padding: 8px 20px;
    margin: 7px 3px;
    border: 2px solid white;
    border-radius: 8px;
    background: none;
    color: white;
    cursor: pointer;
    font-size: 20px;
    transition: background-color 0.3s, color 0.3s;
}

.btn:hover {
    background-color: white;
    color: black;
}

.btn-sm {
    padding: 6px 10px;
    vertical-align: middle;
    font-size: 16px;
}

.btn-dark {
    color: black;
    border: 2px solid grey;
}

.section {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    max-width: 80%;
    margin: auto;
    padding: 10px;
    flex-wrap: wrap;
}

.section-left {
    flex-direction: row-reverse;
}

.paras {
    padding: 0px 65px;
}

.sectionTag {
    padding: 16px 0;
}

.sectionSubTag {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.thumbnail img {
    width: 100%;
    max-width: 250px;
    border: 2px solid black;
    border-radius: 26px;
    margin-top: 19px;
}

.contact {
    background-color: #f6f5f4;
    height: auto;
    padding: 50px 0;
}

.text-center {
    text-align: center;
    padding-top: 30px;
    font-size: 35px;
}

.form {
    max-width: 62%;
    margin: 25px auto;
}

.form-input {
    margin: 14px 0;
    padding: 5px 13px;
    width: 100%;
    font-size: 19px;
    border: 2px solid grey;
    border-radius: 6px;
}

.text-footer {
    text-align: center;
    padding: 30px 0;
    display: flex;
    justify-content: center;
    color: white;
    background-color: black;
}

.burger {
    display: none;
    position: absolute;
    cursor: pointer;
    right: 5%;
    top: 15px;
}

.line {
    width: 33px;
    background-color: white;
    height: 4px;
    margin: 5px 3px;
}

@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
    }
    .nav-list {
        width: 100%;
        flex-direction: column;
    }
    .nav-list li {
        padding: 15px 0;
    }
    .rightNav {
        width: 100%;
        text-align: center;
        padding: 10px 0;
    }
    .burger {
        display: block;
    }
    .logo {
        width: 50%;
    }
}
```

### 3. Add Images

Place your images in the `img` folder. Ensure the image paths in your CSS and HTML files are correct. For example, `bg.jpg` should be placed inside the `img` folder.

### 4. Host the Website Locally

You can host your website locally using a simple HTTP server. If you have Python installed, navigate to the `my-website` directory in your terminal and run:

```sh
# For Python 3.x
python -m http.server

# For Python 2.x
python -m SimpleHTTPServer
```

Then open your browser and go to `http://localhost:8000` to see your website.

### 5. Deploy Your Website Online

You can deploy your website using a variety of services like GitHub Pages, Netlify, Vercel, or any web hosting provider.

**Deploying with GitHub Pages:**

1. **Create a GitHub Repository:**
   - Go to GitHub and create a new repository.

2. **Push Your Project to GitHub:**
   ```sh
   git init
   git remote add origin https://github.com/your-username/your-repo-name.git
   git add .
   git commit -m "Initial commit"
  

 git push -u origin master
   ```

3. **Enable GitHub Pages:**
   - Go to your repository settings.
   - Scroll down to the GitHub Pages section.
   - Select the branch (usually `main` or `master`) and the root folder (`/`) to serve your site.
   - Save the changes.

After a few minutes, your site should be available at `https://your-username.github.io/your-repo-name`.

This process sets up and hosts your website in a new folder, ensuring it's organized and accessible both locally and online.
