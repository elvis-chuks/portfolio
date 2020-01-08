<template>
    <div>
        

            <div class="container">
                <div class="row" id="send_p">
                    <p class="h1-responsive font-weight-bold mr-auto send_message">Send me a Message</p>  
                </div>
            <div class="row">
        
                    <div class="col-sm">
                        <mdb-input label="Your Name" />
                    </div>
                    
                    <div class="col-sm">
                        <mdb-input label="Your Email Address" />
                    </div>
                    
            </div>

            <div class="row">
                <div class="col-sm">
                        <mdb-input outline label="Your Message"/>
                </div>
            </div>

            <button class="btn"> Contact me <span>&nbsp; &nbsp; &nbsp;</span><i class="fas fa-arrow-right"></i></button>
            </div>
        </div>

</template>

<script>

import { mdbInput,mdbBtn} from "mdbvue";
export default {
    name:"Contact",
    components:{
        mdbInput,

    }
}
</script>

<style scoped>
.send_message{
    color:white;
}

#send_p{
    padding-top:80px;
}

input[type=textarea]{
    border:none;
}
.btn{
    background-color: white;
    color:#330033;
}
</style>