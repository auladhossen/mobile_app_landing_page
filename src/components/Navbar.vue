<script setup>

    let navOptions = [
        {name:'Home', id: 'home'}, 
        {name:'Features', id: 'feature'}, 
        {name:'Team', id: 'team'}, 
        {name:'Pricing', id: 'pricing'}, 
        {name:'Contact', id: 'contact'}, 
    ]

</script>

<template>
  <div class="card">
    <div class="nav-logo">
        <h2>AppCo</h2>
    </div>
    <div class="nav-options">
        <div  v-for="(option, index) of navOptions">
            <div>{{ option.name}}</div>
        </div>
    </div>

    <div class="nav-buttons">
        <button class="nav-button-signin">Sign in</button>
        <button class="nav-button-register">Register</button>          
    </div>
  </div>
</template>

<style scoped>
.nav-options{
    display: flex;
    gap: 2rem;
    color: #7a7a7a;
    font-weight: 400;
    font-size: medium;
    cursor: pointer;
    padding: 2rem;
}
.card{
    display: flex;
    padding: 1px 10px 1px 10px;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid #ebebeb;
    position: sticky;
    top: 0;
    background: white;
}
.nav-buttons{
    display: flex;
    gap: 1rem;
    padding: 2px;
    text-wrap: nowrap;
    height: 3rem;
    align-items: center;
}
.nav-button-register {
    border: 1px solid rgb(155, 155, 155);
    border-radius: 30px;
    background: #ff6e6e;
    color: white;
    font-weight: 300;
}
.nav-button-signin {
    border: 1px solid rgb(198, 198, 198);
    border-radius: 30px;
    background: #fcfcfc;
    font-weight: 300;
}
.nav-button-signin:hover {
    border: 1px solid black;
    color: black;

}
</style>
