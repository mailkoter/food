<script>
import HeaderMain from './components/HeaderMain.vue'
import MainInfo from "./components/Maininfo.vue";
import FormSection1 from "./components/Form1.vue";
import SliderBlock from "./components/SliderBlock.vue"

export default {
  name: 'App',
  components: {
    HeaderMain,
    MainInfo,
    FormSection1,
    SliderBlock
  }
}
</script>

<template>
  <div id="app">
    <HeaderMain />
    <MainInfo />
    <FormSection1 />
    <SliderBlock />
    <router-view />
  </div>
</template>

<style>
body{
    font-family: "Unbounded", sans-serif;
    font-optical-sizing: auto;
    font-style: normal;
}
input{
    border: none;
    border-radius: 500px;
    height: 62px;
    font-size: 18px;
    font-weight: 400;
}
input:focus{
    outline: none;
}
form{
    display: flex;
    gap: 20px;
}
input::placeholder{
    color: #7E7E7F;
    font-size: 18px;
    font-weight: 400;
}
input[name="first_name"]{
    max-width: 187px;
    text-align: center;
}
input[type="tel"]{
    padding-left: 117px;
    padding-right: 0;
    position: relative;
}
.tel{
    position: relative;
}
.tel:before{
    content: url("assets/image/rus.svg");
    position: absolute;
    top: -2px;
    left: 20px;
    width: 35px;
    height: 23px;
    z-index: 999999;
}
.tel:after{
    content: "+7";
    font-family: 'Inter';
    font-size: 18px;
    font-weight: 400;
    position: absolute;
    top: 20px;
    left: 92px;
    width: 35px;
    height: 23px;
    z-index: 999999;
}
.container{
    max-width: 1545px;
    margin: 0 auto;
}
a{
    text-decoration: none;
    color: black;
}
p, a{
    font-family: "Inter", sans-serif;
    font-size: 18px;
}
h2{
    font-weight: 600;
    font-size: 28px;
    color: black;
}
h1{
    font-family: "Unbounded", sans-serif;
    font-optical-sizing: auto;
    font-style: normal;
    font-size: 42px;
    font-weight: 700;
    color: #000;
}
.orange{
    color: #FFA333;
}
.defult_btn{
    background: #FFA333;
    padding: 25px 67px;
    font-weight: 600;
    color: #fff;
    border-radius: 500px;
}
</style>
