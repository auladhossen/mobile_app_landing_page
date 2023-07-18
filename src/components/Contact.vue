<script setup>
    const headline = 'Contact with Us';
    const paragraph = `It's very easy to get in touch with us. Just use the contact form or pay us a visit for a coffee at the office. Dynamically innovate competitive technology after an expanded array of leadership.
                It's very easy to get in touch with us. Just use the contact form or pay us a visit for a coffee at the office. Dynamically innovate competitive technology after an expanded array of leadership.
                </br>Head Office:
                121 King St, Virginia VIC 3000, USA
                </br>Phone: +61 56757658
                </br> Email : test@yourdomain.com`

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
        <div class="form">
            <p class="text">Get us quickly</p>
            <div class="top-section">
                <input class="input" type="text" placeholder="Enter Name"> 
                <input class="input" type="email" placeholder="Enter Email"> 
            </div>      
            <div class="bottom-section">
                <input class="input" type="text" placeholder="Enter Phone"> 
                <input class="input" type="text" placeholder="Enter Company"> 
            </div>    
            <div class="message">
                <textarea class="text-area" rows="4" cols="48" name="comment" form="usrform">Enter text here</textarea>               
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
    display: flex;
    gap: 5rem;
    padding:  5rem 2rem 5rem 2rem;
    width: 100%;
    background-color: #eaeaea;
}

.top-section, .bottom-section{
    display: flex;
    gap: 1rem;
}

.input{
    padding: 5px;
    margin: 5px;
    border: 1px solid rgb(217, 217, 217);
}

.message{
    margin-top: 5px;
}
.text-area{
    border: 1px solid rgb(217, 217, 217);
    color: rgb(120, 120, 120);
}

</style>
