<template>
    <footer class="footer-component">
        <p>&copy; 2023 Pahul Johal</p>
    </footer>
</template>

<script>
export default {
    name: 'FooterComponent',  /* Renamed to more general 'FooterComponent' */
};
</script>

<style scoped>
.footer-component {
    background-color: #323232; /* Slightly lighter shade for better contrast */
    color: #F5F5F5;
    text-align: center;
    padding: 25px 0; /* Increased padding for better spacing */
    font-size: 0.95rem; /* Slightly bigger font for better readability */
    box-shadow: 0 -3px 5px rgba(0, 0, 0, 0.1);
    position: relative;
    bottom: 0;
    width: 100%;
    border-top: 2px solid rgba(255, 255, 255, 0.1); /* Made border slightly thicker */
}
</style>
