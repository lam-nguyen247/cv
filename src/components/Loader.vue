<template>
    <div>
        <div class="loader" id="loader">
            <div class="container">
                <img src="../assets/logo.png">
                <div class="name">
                    <span 
                        v-for="(char,index) in arrName"
                        :key="index"
                    >{{char=="-"?'&nbsp;':char}}</span>
                </div>
                <div class="line"></div>
                <div class="sub">
                    <p> Web developer </p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props:['arrName'],
    }
</script>

<style scoped>

</style>