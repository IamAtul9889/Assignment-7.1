## Assignment 7.1 — Responsive Navigation Bar

### `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Navigation</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="navbar">
        <h2 class="logo">MyWebsite</h2>

        <nav class="nav-links">
            <a href="#">Home</a>
            <a href="#">About</a>
            <a href="#">Services</a>
            <a href="#">Contact</a>
        </nav>

        <button>Login</button>
    </header>
</body>
</html>
```

### `style.css`

```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: navy;
    padding: 15px 30px;
}

.logo {
    color: white;
}

.nav-links {
    display: flex;
    gap: 25px;
}

.nav-links a {
    color: white;
    text-decoration: none;
}

.nav-links a:hover {
    color: yellow;
}

button {
    background: orange;
    border: none;
    padding: 10px 18px;
    border-radius: 5px;
    cursor: pointer;
}

@media (max-width: 600px) {
    .navbar {
        flex-direction: column;
        gap: 15px;
    }

    .nav-links {
        flex-wrap: wrap;
        justify-content: center;
    }
}
```

**Submission:** Save both files in the same folder, open `index.html` with Live Server, and resize the browser to test responsiveness.