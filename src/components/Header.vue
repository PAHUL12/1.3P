<template>
    <header class="header-component">
        <nav>
            <router-link class="nav-link" to="/">Home</router-link>
            <router-link class="nav-link" to="/about">About</router-link>
            <router-link class="nav-link" to="/portfolio">Portfolio</router-link>
            <router-link class="nav-link" to="/contact">Contact</router-link>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent',  /* Renamed to more general 'HeaderComponent' */
};
</script>

<style scoped>
.header-component {
    background-color: #333; /* Slightly lighter shade for better contrast */
    color: #F5F5F5;
    padding: 20px 0; /* Increased padding for better spacing */
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.1);
}

nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    gap: 20px; /* Added gap for better spacing between links */
}

.nav-link {
    color: #F5F5F5;
    text-decoration: none;
    font-weight: 600;
    padding: 8px 20px; /* Increased padding for a better touch target */
    border-radius: 5px;
    transition: background-color 0.3s ease, transform 0.3s ease; /* Added transform for a subtle effect on hover */
}

.nav-link:hover {
    background-color: rgba(255, 255, 255, 0.1);
    transform: scale(1.05); /* Slight scale on hover for better interaction feedback */
}
</style>
