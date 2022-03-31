<template>
    <div class="nav">
        <ul>
            <li><h1>Gerador de QRCode </h1></li>
            <li class="logo"><img alt="Vue logo" src="../assets/logo.png"></li>
        </ul>
    </div>
</template>

<script>
export default {
    name:"HeaderApp",
}
</script>
<style scoped>
h1{
    padding-top: 13px;
    font-size: 22px;
    font-family: 'Red Hat Mono', monospace;
    letter-spacing: 2px;
}
.nav{
    text-align: center;
    background-color: rgb(27, 27, 27);
    width: 100%;
    height: 52px;
    display: flex;
    position: relative;
}
ul{
    
    margin-left: auto;
    margin-right: auto;
}
li{
   float: left;
   list-style: none;
   
}
img{
    width: 30px;
    height: 30px;
}
.logo{
    margin-top: 13px;
    margin-left: 7px;
}
</style>