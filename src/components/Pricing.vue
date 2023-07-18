<script setup>
    const headline = 'Pricing';
    const paragraph = `Pricing for everyone. Choose your plan now!`;
    const options = [
        {name: 'Free', amount: '$0'},
        {name: 'Standard', amount: '$19.99'},
        {name: 'Premium', amount: '$79.99'},
    ]

</script>

<template>
    <div class="body">
        <div class="main-section">
            <div class="headine">
                <h1>{{ headline }}</h1>
            </div>
            <div class="text">              
                <p v-html="paragraph"></p>
            </div>          
        </div>  
        <div class="pricing">
            <div class="options" v-for="(option, index) of options" :key="index">
                <div class="option">
                    <h2 class="name">{{ option.name }}</h2>
                    <h3 class="amount">{{ option.amount }}</h3>
                    <div class="services">
                        <p>1. There live the blind texts</p>
                        <p>2. Far far away behind the word</p>
                        <p>3. Far from the countries Vokalia and Consonantia</p>
                    </div>
                    <div class="buttons">
                        <button class="button-feature">Get Started</button>     
                    </div>
                </div>
            </div>         
        </div> 
         
    </div>      
</template>

<style scoped>
.main-section{
    align-items: center;
    text-align: left;
    display: flex;
    flex-direction: column;
    width: 100%;
}
.body{
    align-items: center;
    text-align: center;
    padding:  5rem 2rem 5rem 2rem;
    width: 100%;
}
.pricing{
    display: flex;
    gap: 4rem;
    justify-content: center;
}

.option{
    padding: 10px;
}
.options{
    display: flex;
    gap: 5rem;
    border: 1px solid rgb(197, 197, 197);
    border-radius: 10%;
    margin-top: 20px;
}
.name{
    font-weight: 400;
}
.amount{
    color: #ff6e6e;
}
.buttons{
    display: flex;
    gap: 1rem;
    padding: 2px;
    text-wrap: nowrap;
    height: 3rem;
    align-items: center;
    justify-content: center;
}
.button-feature {
    border: 1px solid rgb(214, 214, 214);
    border-radius: 20px;
    background: #ff6e6e;
    color: white;
    font-weight: 300;
}
</style>
