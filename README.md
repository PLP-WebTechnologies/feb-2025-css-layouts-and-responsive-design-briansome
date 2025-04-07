# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Layout</title>
    <style>
        body {
            font-family: sans-serif;
            margin: 0;
            padding: 0;
        }

        nav {
            background-color: #333;
            color: white;
            padding: 10px 0;
        }

        nav ul {
            list-style: none;
            display: flex; /* Using Flexbox for navigation */
            justify-content: center;
            margin: 0;
            padding: 0;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav a {
            color: white;
            text-decoration: none;
        }

        .container {
            display: grid; /* Using Grid for main content */
            grid-template-columns: 1fr; /* Single column by default (mobile) */
            gap: 20px;
            padding: 20px;
        }

        .item {
            background-color: #f0f0f0;
            padding: 20px;
            border-radius: 5px;
        }

        /* Media Queries for responsiveness */
        @media (min-width: 600px) { /* Tablet */
            .container {
                grid-template-columns: 1fr 1fr; /* Two columns on tablet */
            }
        }

        @media (min-width: 992px) { /* Desktop */
            .container {
                grid-template-columns: 1fr 1fr 1fr; /* Three columns on desktop */
            }
        }

    </style>
</head>
<body>

    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <div class="container">
        <div class="item">
            <h2>Item 1</h2>
            <p>This is the content of item 1.</p>
        </div>
        <div class="item">
            <h2>Item 2</h2>
            <p>This is the content of item 2.</p>
        </div>
        <div class="item">
            <h2>Item 3</h2>
            <p>This is the content of item 3.</p>
        </div>
        <div class="item">
          <h2>Item 4</h2>
          <p>This is item 4</p>
        </div>
        <div class="item">
          <h2>Item 5</h2>
          <p>This is item 5</p>
        </div>
        <div class="item">
          <h2>Item 6</h2>
          <p>This is item 6</p>
        </div>
    </div>

</body>
</html>
