<template>
    <div>
        <div class="row" id="deets">
        <div class="col-sm deets">
            <p class="h1-responsive font-weight-bold">I Design & <br> Build stuff.</p>

            <p class="h4-responsive">Open source <br> projects, web apps <br>  and experimentals.</p>

            <button class="btn btn_btn">See My Work <span>&nbsp; &nbsp; &nbsp;</span><i class="fas fa-arrow-right"></i></button>
        </div>

        <div class="col-sm deets thoughts">
            <p class="h1-responsive font-weight-bold">I Like to share my thoughts, sometimes.</p>

            <p class="h4-responsive">About Architecture, <br>back end dev, <br>learning and life.</p>

            <button class="btn btn_btn">View My Thoughts <span>&nbsp; &nbsp; &nbsp;</span><i class="fas fa-arrow-right"></i></button>
        </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Details",
}
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css?family=Poppins&display=swap');
#deets{
    margin-top:60px;
    /* padding:20px; */
    background-color: #fff;
    color:#330033;
    /* -webkit-box-shadow: 3px 3px 5px 6px #ccc;  Safari 3-4, iOS 4.0.2 - 4.2, Android 2.3+ */
    /* -moz-box-shadow:    3px 3px 5px 6px #ccc;  Firefox 3.5 - 3.6 */
    /* box-shadow:         2px 2px 3px 3px #ccc;  */
}
.deets{
    padding:130px 60px;
    font-family: 'Poppins', sans-serif;
}
.thoughts{
    border-left:1px solid #330033;
}

.btn_btn{
    border:1px solid #330033;
    color:#330033;
}

@media (max-width: 576px) { 
    .thoughts{
        border-left: none;
        border-top: 1px solid #330033;
    }

    .deets{
        padding:60px 40px;
    }

    }
</style>