<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JALA Academy - Comprehensive HTML5 Assignments</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Semantic Elements: Header & Nav -->
    <header>
        <h1>JALA Academy Front-End Masterclass</h1>
        <nav>
            <ul>
                <li><a href="#basics">HTML Basics</a></li>
                <li><a href="#inputs">Inputs & Attributes</a></li>
                <li><a href="#semantics">Semantics & Layout</a></li>
            </ul>
        </nav>
    </header>

    <!-- HTML5 Basics Section -->
    <section id="basics">
        <h2>1. HTML Basics & Text Formatting</h2>
        <p>This is a standard paragraph with <b>Bold text</b>, <i>Italic text</i>, and a <span>span element</span>.</p>
        <blockquote>
            "Practice consistently to master web development." - JALA Academy
        </blockquote>
        <hr>
        <h3>Unordered List</h3>
        <ul>
            <li>List Item 1: HTML5</li>
            <li>List Item 2: CSS3</li>
            <li>List Item 3: JavaScript</li>
        </ul>
        <div class="div-box">
            This is inside a &lt;div&gt; block-level element.
        </div>
        <img src="https://via.placeholder.com/200" alt="Sample Hero Image">
    </section>

    <!-- HTML5 Input Attributes & Restrictions Section -->
    <section id="inputs">
        <h2>2. HTML5 Input Attributes, Types, and Restrictions</h2>
        <form>
            <label>Text: <input type="text" name="txt" required placeholder="Required field" maxlength="15"></label><br><br>
            <label>Password: <input type="password" name="pwd" readonly value="Secret123"></label><br><br>
            <label>Disabled Input: <input type="text" disabled value="Cannot edit"></label><br><br>
            
            <label>Number (Min 1, Max 10): <input type="number" min="1" max="10" size="5"></label><br><br>
            <label>Range: <input type="range" min="0" max="100"></label><br><br>
            <label>Color Picker: <input type="color"></label><br><br>
            <label>Date: <input type="date"></label><br><br>
            <label>File Upload: <input type="file"></label><br><br>
            <label>Email: <input type="email" placeholder="test@jala.com"></label><br><br>

            <p>Gender:</p>
            <label><input type="radio" name="gender" value="male"> Male</label>
            <label><input type="radio" name="gender" value="female"> Female</label><br><br>
            
            <label><input type="checkbox" name="subscribe"> Subscribe to newsletter</label><br><br>

            <input type="submit" value="Submit Form">
            <input type="reset" value="Reset Form">
            <button type="button">Custom Button</button>
        </form>

        <hr>
        <h3>Target Attribute & Iframe & Marquee</h3>
        <p><a href="https://jala-academy.github.io" target="_blank">Open JALA in New Tab (_blank)</a></p>
        <p><a href="#basics" target="_self">Navigate within same page (_self)</a></p>

        <iframe src="https://example.com" width="300" height="150" title="Iframe Example"></iframe>
        
        <marquee behavior="scroll" direction="left">Welcome to JALA Academy Live Projects Training!</marquee>
    </section>

    <!-- Semantic Elements Section -->
    <section id="semantics">
        <h2>3. Semantic Elements</h2>
        <article>
            <h3>Article Heading</h3>
            <p>Articles represent independent content structures.</p>
            <figure>
                <img src="https://via.placeholder.com/100" alt="Figure Sample">
                <figcaption>Fig 1.0 - Sample caption for figure.</figcaption>
            </figure>
        </article>
        
        <aside>
            <h4>Related Links</h4>
            <p>Check out <mark>brightitcareer.com</mark> for job support.</p>
        </aside>
    </section>

    <footer>
        <p><time datetime="2026-06-07">Published on June 7, 2026</time></p>
        <p>&copy; 2026 JALA Academy Student Portal</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>