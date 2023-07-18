<script setup>
import { ref } from 'vue';

const headline = 'Selling Digital Services';
const paragraph = 'Another cool free html css template by AppCo Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast.far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast';
const imageLink = ref('../public/photo1.svg');

</script>

<template>
    <div class="body">
        <div class="second-section">
            <img :src="imageLink" alt="Image"/>
        </div>
        <div class="first-section">
            <div class="headine">
                <h1>{{headline}}</h1>
            </div>
            <div class="text">
                <div>
                    <p>{{ paragraph}}</p>
                </div>
            </div>
        </div>      
    </div>      
</template>

<style scoped>
.first-section{
    align-items: center;
    text-align: center;
    display: flex;
    flex-direction: column;
    width: 45%;
}
.second-section{
    width: 45%;
}
.body{
    display: flex;
    padding: 10px;
    background-color: rgb(233, 233, 233);
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
    background: #6068ff;
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
