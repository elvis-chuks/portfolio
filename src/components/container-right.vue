<template>
    <div id="svge">
        <img src="../assets/Group 4 (2).svg" class="img-fluid">
    </div>
</template>

<script>
export default {
    name: "ContainerRight",
    data(){
        return{
            image:"../assets/peeps.svg",
            width:"450px"
        }
    }

}
</script>

<style scoped>
#svge{
    margin-top: 50px;
    margin-left: 100px;
}

@media (max-width: 576px) { 
    #svge{
    margin-top: 50px;
    margin-left: 20px;
    /* width:50%; */
        }

 }
</style>