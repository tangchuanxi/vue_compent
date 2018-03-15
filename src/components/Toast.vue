<template>  
    <div class="toast"  v-if="isShow">  
        <div class="toast-div">{{ text }}</div>  
    </div>  
</template>  
  
<script>  
export default{  
    data(){
        return {  
            text:'内容',  
            isShow:true,  
            duration:1500  
        }  
    },
    methods:{

    }
}  
</script>  
  
<style>  
*{  
    margin: 0;  
    padding: 0;  
}  
.toast{  
    position: fixed;  
    left: 50%;  
    transform: translate(-50%, 0);  
    margin-top: 5rem;  
    background: #000000;  
    line-height: 0.7rem;  
    color: #FFFFFF;  
    padding: 0 0.2rem;  
    border-radius: 0.2rem;  
    width: 100px;
    height: 30px;
    line-height: 30px;
    text-align: center;
}  


</style> 