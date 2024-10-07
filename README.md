* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
}

.container {
    display: grid;
    grid-template-rows: auto auto auto 1fr auto;
    grid-template-columns: 1fr;
    grid-template-areas:
        "header"
        "navbar"
        "main"
        "grid-section";
    gap: 10px;
}

.header {
    grid-area: header;
    background-color: #f5f5f5;
    padding: 20px;
    text-align: center;
    font-size: 24px;
}

.navbar {
    grid-area: navbar;
    background-color: #ddd;
    padding: 10px;
    text-align: center;
}

.navbar ul {
    list-style-type: none;
}

.navbar ul li {
    display: inline;
    margin: 0 10px;
}

.navbar ul li a {
    text-decoration: none;
    color: #333;
    font-weight: bold;
}

.main {
    grid-area: main;
    text-align: center;
    padding: 20px;
}

.main .hero {
    background-color: #a9d0f5;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.main p {
    margin-top: 20px;
}

.grid-section {
    grid-area: grid-section;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    padding: 20px;
}

.grid-item {
    text-align: center;
}

.grid-item img {
    width: 100px;
    height: 100px;
    background-color: #a9d0f5;
}

.grid-item h2 {
    margin: 10px 0;
}

.grid-item p {
    font-size: 14px;
    color: #666;
}
