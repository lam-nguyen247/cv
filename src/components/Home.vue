<template>
    <div>
        
        <!-- Begin loader -->
            <app-loader :arrName="arrName"/>
        <!-- End loader -->
        <!-- Begin content -->
        <div class="page" id="page">
            <b-row style="margin:1px">
                <b-col cols="1" class="site-nav">
                    <div class="avatar">
                        <img src="static/img/photo.png">
                    </div>
                    <div class="title-name">
                        <h1>LAM NGUYEN</h1>
                    </div>
                    <ul id="nav" class="main-menu">
                        <li>
                            <a href="#">
                                <i class="fa fa-home"></i>
                               
                            </a>
                        </li>
                    </ul>
                </b-col>
                <b-col cols="11">ABC</b-col>
            </b-row>
        </div>
        <!-- End content -->
       
    </div>
</template>

<script>
    import AppLoader from  "./Loader";
    export default {
        data(){
            return {
                  arrName:["L","Â","M","-","N","G","U","Y","Ễ","N"],
            }
        },
        components:{
            AppLoader
        }
    }
    setTimeout(() => {
        document.getElementById("loader").style.display="none";
        document.getElementById("page").style.display="block";
    }, 4000);
</script>

<style scoped>
   @import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css");
   
</style>