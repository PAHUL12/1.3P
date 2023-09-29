<template>
    <section id="contact">
        <h2>Get in Touch</h2>
        <form @submit.prevent="handleSubmit"> <!-- Added submit handler for future functionality -->
            <div class="form-group">
                <label for="name">Your Name</label>
                <input type="text" id="name" name="name" placeholder="John Doe" required>
            </div>
            <div class="form-group">
                <label for="email">Your Email</label>
                <input type="email" id="email" name="email" placeholder="john@example.com" required>
            </div>
            <div class="form-group">
                <label for="message">Your Message</label>
                <textarea id="message" name="message" rows="4" placeholder="Hello! I'd like to connect..." required></textarea>
            </div>
            <button type="submit" class="submit-btn">Send Message</button>
        </form>
    </section>
</template>

<script>
export default {
    name: 'ContactComponent',
    methods: {
        handleSubmit() {
            // TODO: Handle the form submission logic here.
            alert('Form submitted! This can be replaced with actual form processing logic.');
        }
    }
};
</script>

<style scoped>
#contact {
    padding: 50px 10%; /* Enhanced padding for better spacing */
    background-color: #f5f5f5; /* Slightly darker gray for subtle depth */
    border-radius: 10px;
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08); /* Enhanced shadow for better depth */
    margin: 30px 0;
    text-align: center; /* Centered text for form */
}

#contact h2 {
    font-family: 'Arial', sans-serif;
    font-size: 2.5rem; /* Enhanced font size */
    border-bottom: 2px solid #555; 
    padding-bottom: 20px; /* Enhanced padding */
    margin-bottom: 40px;
    color: #444; /* Darker text color */
}

.form-group {
    margin-bottom: 25px;
    text-align: left; /* Left aligned labels and input fields */
}

.form-group label {
    display: block;
    margin-bottom: 12px;
    font-size: 1.1rem; /* Slightly larger font size */
    font-weight: 500; /* Slightly bold */
}

.form-group input, .form-group textarea {
    width: 100%;
    padding: 12px 15px; /* Enhanced padding for better typing experience */
    border: 1px solid #ccc;
    border-radius: 6px; /* Rounded edges for inputs */
    font-size: 1rem; /* Standard font size */
    transition: border-color 0.2s ease; /* Transition for focus effect */
}

.form-group input:focus, .form-group textarea:focus {
    border-color: #6B73FF; /* Blue focus color */
    outline: none; /* Removing browser default outline */
}

.submit-btn {
    background-color: #6B73FF; /* Blue background color */
    color: white;
    padding: 12px 30px; /* Enhanced padding */
    border: none;
    border-radius: 6px;
    cursor: pointer;
    transition: background-color 0.3s ease;
    font-weight: 600; /* Bold text */
}

.submit-btn:hover {
    background-color: #5555FF; /* Slightly darker blue on hover */
}
</style>
