<template>
    <div class="portfolio-view">
        <section class="education-section">
            <h2>My Education</h2>
            <ul class="education-list">
                <li>
                    <h3>Bachelor of Information Technology</h3>
                    <p>Deakin University, Burwood</p>
                    <p>March/2023 – Current</p>
                    <p>Expected Completion: November 2025</p>
                    <p>Key Skills: C, C++, Python, Java, HTML</p>
                </li>
                <li>
                    <h3>St joseph Convent School</h3>
                    <p>Punjab, India</p>
                    <p>March/2018 – June/2022</p>
                    <p>Achievements: School leader</p>
                </li>
            </ul>
        </section>
  
        <section class="employment-section">
            <h2>Professional Experience</h2>
            <ul class="employment-list">
                <li>
                    <h3>Crew Member</h3>
                    <p>Schnitz, Cheltenham, Melbourne, Victoria</p>
                    <p>June/2023 – Current</p>
                    <p>Roles & Responsibilities:</p>
                    <ul>
                        <li>Provided a diverse range of food and beverage options.</li>
                        <li>Managed inventory and restocked display counters.</li>
                        <li>Handled both day and night shifts efficiently.</li>
                        <li>Delivered exceptional customer service at the front counter and drive-through.</li>
                        <li>Processed orders from online platforms like Uber Eats, Doordash, and Menulog.</li>
                    </ul>
                </li>
            </ul>
        </section>
    </div>
</template>

<script>
export default {
    name: 'PortfolioView',
};
</script>

<style scoped>
.portfolio-view {
    padding: 50px 10%;
    background-color: #f9f9f9;
    color: #444;
    border-radius: 12px;
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
}

h2 {
    font-size: 2.5rem;
    margin-bottom: 25px;
    border-bottom: 2px solid #007BFF;
    padding-bottom: 20px;
    text-align: center;
}

ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

li {
    margin-bottom: 35px;
    line-height: 1.6;
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
}

h3 {
    font-size: 1.8rem;
    margin-bottom: 15px;
    color: #007BFF;
}
</style>
