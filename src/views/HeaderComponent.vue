<template>
    <header>
        <div class="header-container">
            <h1>Pahul Johal's Portfolio</h1>
            <nav>
                <ul>
                    <li><router-link to="/about">About Me</router-link></li>
                    <li><router-link to="/experience">Experience</router-link></li>
                    <li><router-link to="/contact">Contact</router-link></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent'
};
</script>

<style scoped>
header {
    background-color: #333;
    color: white;
    box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.15); /* Enhanced shadow for depth */
}

.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 25px 10%; /* Enhanced padding for better spacing */
    max-width: 1200px; /* Limiting the maximum width for large screens */
    margin: 0 auto; /* Centering on large screens */
}

header h1 {
    font-size: 26px; /* Slightly enhanced font size */
    margin: 0;
    letter-spacing: 1px; /* Adding letter spacing for better readability */
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    gap: 25px; /* Slightly enhanced gap between nav items */
}

nav li {
    display: inline;
}

nav a {
    text-decoration: none;
    color: white;
    font-size: 1.1rem; /* Using rem for scalability */
    padding: 5px 10px; /* Padding for better hover effect */
    border-radius: 4px; /* Rounded edges for hover background effect */
    transition: color 0.3s ease, background-color 0.3s ease;
}

nav a:hover {
    color: #333; /* Text color on hover */
    background-color: #f5f5f5; /* Background color on hover */
}

@media screen and (max-width: 768px) {
    .header-container {
        flex-direction: column; /* Align vertically on mobile */
        align-items: start; /* Align to start on mobile */
    }

    nav ul {
        display: flex; /* Show navigation on mobile */
        flex-direction: column; /* Vertical navigation on mobile */
        gap: 15px; /* Gap between vertical nav items */
    }
}
</style>
