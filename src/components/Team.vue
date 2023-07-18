<script setup>
    const headline = 'Our Team Members';
    const paragraph = 'Following reasons show advantages of adding AppCo to your lead pages, demos and checkouts evisculate interoperable imperatives rather.';
    
    const teamMembers = [
        {name: 'John Lee', link: '../public/member1.svg'},
        {name: 'Faizal Yakub', link: '../public/member2.svg'},
        {name: 'Jae Lim', link: '../public/member3.svg'},
        {name: 'Kian Ho', link: '../public/member4.svg'},
    ];
</script>

<template>
    <div class="body">
        <div class="main-section">
            <div class="headine">
                <h1>{{ headline }}</h1>
            </div>
            <div class="text">              
                <p>{{ paragraph }}</p>
            </div>
            <div class="members">
                <div class="member" v-for="(member, index) in teamMembers" :key="index">
                    <img class="image" :src="member.link"/>
                    <p class="name">{{ member.name}}</p>
                </div>
            </div>
        </div>      
    </div>      
</template>

<style scoped>
.main-section{
    align-items: center;
    text-align: right;
    display: flex;
    flex-direction: column;
    width: 100%;
}
.second-section{
    width: 45%;
}
.body{
    align-items: center;
    text-align: center;
    display: flex;
    padding: 10px;
    width: 100%;
}
.members{
    display: flex;
    gap: 5rem;
    margin-top: 10px;
    margin-bottom: 10px;
    padding: 20px;
    width: 100%;
    align-items: center;
    justify-content: space-around;
}
.member{
    text-align: center;
}
.text{
    width: 60%;
    text-align: center;
}
.image{
    width: 12rem;
    border: 1px solid #cfcfcf;
    border-radius: 50%;
    padding: 10px;
}
.name{
    font-weight: 500;
}
</style>
