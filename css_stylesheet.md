/* CSS Basics: Comments, Backgrounds, and Borders */
/* This is a single-line CSS comment */
/*
   Multi-line CSS comment block:
   Styling rules for JALA Academy assignments.
*/

body {
    background-color: #f4f6f9;
    background-image: url('https://via.placeholder.com/800');
    background-repeat: no-repeat;
    background-attachment: fixed; /* Background should not scroll */
    background-size: cover;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    padding: 20px;
    scroll-behavior: smooth; /* Smooth scrolling for top/bottom links */
}

/* Different borders on each side with different patterns */
.div-box {
    width: 60%;
    height: 100px;
    border-top: 3px solid red;
    border-right: 5px dashed green;
    border-bottom: 4px dotted blue;
    border-left: 6px double orange;
    padding: 15px;
    margin: 20px 0;
    font-size: 16px;
    font-style: italic;
    text-align: center;
}

/* CSS Page Adjustments: Tables, Visibility, Display, Padding & Margin */
table {
    width: 100%;
    border: 2px solid black;
    border-collapse: collapse;
    table-layout: fixed; /* Fixed table layout compatibility */
    margin-bottom: 20px;
}

table:hover {
    background-color: #fff3cd; /* Page/Table color changes on hover */
}

th, td {
    border: 1px solid black;
    padding: 10px;
}

.hidden-element { visibility: hidden; }
.visible-element { visibility: visible; }
.display-none { display: none; }
.display-inline { display: inline; }
.display-block { display: block; }

/* CSS Effects: Shadows, Positions, Overflow, and Animations */
section {
    background: rgba(255, 255, 255, 0.9);
    padding: 25px;
    margin-bottom: 30px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Shadow effect */
}

section img:hover {
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3); /* Hover cursor shadow */
    opacity: 0.9;
}

.sticky-nav {
    position: sticky;
    top: 0;
    background: #333;
    color: white;
    padding: 10px;
}

.scroll-box {
    height: 80px;
    overflow: scroll;
    border: 1px solid #ccc;
    padding: 5px;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

.animated-element {
    animation-name: fadeIn;
    animation-duration: 2s;
    animation-iteration-count: infinite;
    animation-delay: 1s;
}

.grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 15px;
}

@media (max-width: 768px) {
    body {
        padding: 10px;
    }
    .div-box {
        width: 100%;
    }
}