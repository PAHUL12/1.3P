<template>
    <div class="responsive-buttons">
        <button 
            v-for="(item, index) in items" 
            :key="index" 
            class="btn" 
            @click="handleItemClick(index)">
            {{ item }}
        </button>
  
        <button v-if="showElement" class="btn" @click="toggleShowElement">
            Conditional Element
        </button>
  
        <input v-model="inputValue" class="input-field" placeholder="Type something..."/>
  
        <button class="btn" @click="handleButtonClick">Submit</button>
    </div>
</template>

<script>
export default {
    name: 'ResponsiveButtonsComponent', /* Renamed for clarity */
    data() {
        return {
            items: ['Item 1', 'Item 2', 'Item 3'],
            showElement: true,
            inputValue: '',
        };
    },
    methods: {
        handleItemClick(index) {
            alert(`Item ${index + 1} clicked!`);
        },
        toggleShowElement() {
            this.showElement = !this.showElement;
        },
        handleButtonClick() {
            alert('Button clicked!');
        },
    },
};
</script>

<style scoped>
.responsive-buttons {
    display: flex;
    flex-direction: column;
    gap: 15px; /* Added gap for better spacing between items */
    padding: 20px;
}

.btn, .input-field {
    margin: 5px;
    padding: 10px 20px;
    font-size: 16px;
    background-color: #444; /* Slightly lighter shade for better contrast */
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.2s ease, transform 0.2s ease; /* Added transform for a subtle effect on hover */
}

.btn:hover {
    background-color: #666;
    transform: scale(1.05); /* Slight scale on hover for better interaction feedback */
}

.input-field {
    font-size: 16px;
    background-color: #f7f7f7; /* Slightly lighter shade for clarity */
    color: #333;
    border: 1px solid #ccc; /* Added border for clarity */
}

@media screen and (max-width: 768px) {
    .btn, .input-field {
        padding: 8px 16px;
        font-size: 14px;
    }
}

@media screen and (max-width: 480px) {
    .btn, .input-field {
        padding: 6px 12px;
        font-size: 12px;
    }
}
</style>
