<template>
    <header>
        <h1>{{title}}</h1> 
    </header>
</template>

<script >
import {ref} from 'vue';
export default{
    setup(){
        const title=ref('Blog');
   
    return { title }
     }
}
</script>

<style lang="scss" scoped>
header{
    position: relative;
    height: 200px;
    background-color: #dddd;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: url('../assets/header.jpg');
    background-size: cover;
    &::before{
        opacity: 0.9;
    content:'';
    display: block;
    position: absolute;
    align-items: center;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    background:linear-gradient(to right, rgb(78, 7, 95) , rgb(133, 126, 194));
    }
}
h1{
    position: relative;
    margin: 0px;
    color: #ffffff;
    font-weight: 300;
    font-size: 60px;
}

</style>