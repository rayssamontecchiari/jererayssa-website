<template>
    <div class="content">
        <h3>Jere e Rayssa</h3>      
        <b-img 
            src="../css/images/casal.jpeg" 
            fluid 
            alt="Responsive image" 
            rounded="circle"
            class="image-casal"
        /> <br>
        <b-img
            src="../css/images/line.png"
            class="image-divisor"
        />
        <br>
        <br>
        <div class="divisor">
            <h5>Confirme sua Presença</h5>
        </div>
        
        <div class="divisor">
            <Form />
        </div>

        <!-- <div class="divisor">
            <p class="text">
                Neste dia especial queremos convidar você para
                nossa celebração!
            </p>
            <p class="text">
                <b>31/07/2022</b>
            </p>
        </div> -->
    </div>
</template>


<script>
export default {
    
}
</script>

<style lang="css">
    @font-face {
        font-family: josefin;
        src: url("../css/font/josefin-sans-thin.ttf");
    }
    .content {
        margin: 0 auto;
        margin-top: 5%;
        text-align: center;
        max-width: 600px;
        font-family: 'josefin', sans-serif;
    }
    .divisor {
        margin-top: 3%;
    }
    .image-divisor {
        width: 120px;
    }
    .text {
        max-width: 50%;
        margin: 0 auto;
        text-align: center;
    }
    .image-casal {
        width: 120px;
    }
</style>