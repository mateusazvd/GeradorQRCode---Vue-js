<template>
<div>
    <h1>Crie seu QRCode</h1>
    <textarea maxlength="800" rows="6" v-model="inputUsuario"></textarea><br/>
    <button @click="gerarQrcode()">Gerar QRCode</button><br/>
    <img id="QrcodeIMG" :src="conteudoQrcode">  
</div>
    
</template>
<script>
export default {
    nome:'AreaConteudo',
    data() {
        return{
            inputUsuario:"",
            conteudoQrcode:""
        }
    },
    methods: {
        gerarQrcode(){
             var inputUsuario2 = this.inputUsuario
             var googleApi = "https://chart.googleapis.com/chart?cht=qr&chs=250x250&chl="
             var cont = googleApi + encodeURIComponent(inputUsuario2)
             this.conteudoQrcode = cont
        }
    }

}
</script>
<style scoped>
   h1{
       margin-bottom: 15px;
   }
   div{
       text-align: center;
    
       margin-top: 7vh;
       
   }
   textarea{
       width: 250px;
       background-color: #232323;
       color: white;
   }
   img{
       margin-top: 30px;
   }
   button{
       padding: 20px 63px;
       font-size: 18px;
       margin-top: 30px;
       border: none;
       border-radius: 7px;
       cursor: pointer;
   }
   
</style>