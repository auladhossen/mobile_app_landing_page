<script setup>
import { ref } from 'vue';

const headline = 'Promote Your Products by AppCo';
const paragraph = 'Another cool free html css template by AppCo Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast';
const imageLink = ref('../public/photo2.svg');
</script>

<template>
    <div class="card">
        <div class="first-section">
            <div class="headine">
                <h1>{{headline}}</h1>
            </div>
            <div class="text">
                <div>
                    <p>{{ paragraph}}</p>
                </div>
            </div>
            <div class="buttons">
                <button class="button-feature">See Features</button>
                <button class="button-pricing">Pricing</button>          
            </div>
        </div>
        <div class="second-section">
            <img :src="imageLink" alt="Image"/>
        </div>
    </div>
           
</template>

<style scoped>
.first-section{
    align-items: left;
    text-align: left;
    display: flex;
    flex-direction: column;
    width: 45%;
}
.second-section{
    width: 45%;
}
.card{
    display: flex;
    padding: 10px;
    margin-top: 30px;
    margin-bottom: 50px;
}
.buttons{
    display: flex;
    gap: 1rem;
    padding: 2px;
    text-wrap: nowrap;
    height: 3rem;
    align-items: center;
}
.button-feature {
    border: 1px solid rgb(155, 155, 155);
    border-radius: 30px;
    background: #ff6e6e;
    color: white;
    font-weight: 300;
}
.button-pricing {
    border: 1px solid rgb(198, 198, 198);
    border-radius: 30px;
    background: #fcfcfc;
    font-weight: 300;
}
</style>
