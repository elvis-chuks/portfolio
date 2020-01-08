<template>
    <div id="wrapper">
        <div class="row">
    <div id="description">
                <p id ="desc" class="h1-responsive font-weight-bold">Back end <br>Developer.</p>
                <p id="detail">
                    <a href="" class="typewrite" data-period="2000" data-type='[ "Hi, Im Elvis.", "I love making things that might <br> possibly work using Python &#128013; / Golang &#128059;" ]'>
                        <span class="wrap"></span>
                    </a>
                </p>
                <!-- <p id="detail">I love making things that might <br>possibly work using Python&#128013;/Golang&#128059; .</p> -->
            </div>
        </div>
    <div class="row">
    <div id="narration">

            <div stuff>
                <!-- my stuff -->
                
                <p>
                    Highly skilled at designing efficient backend systems, REST APIs’ & and have a bit of flair for robotics &#128126;.
                </p>
            </div>
            <div experience>
                
                <p>
                    Over 3+ years of experience. 
                </p>
            </div>

            <div>
                <a class="btn aboutme" href="#aboutme">About Me</a>
                <a class="btn aboutme" href="#">My Work</a>
            </div>

    </div>
    </div>
    </div>
<!-- 127757 world 127925 music &#128521; wink-->
</template>

<script>

var TxtType = function(el, toRotate, period) {
        this.toRotate = toRotate;
        this.el = el;
        this.loopNum = 0;
        this.period = parseInt(period, 10) || 2000;
        this.txt = '';
        this.tick();
        this.isDeleting = false;
    };

    TxtType.prototype.tick = function() {
        var i = this.loopNum % this.toRotate.length;
        var fullTxt = this.toRotate[i];

        if (this.isDeleting) {
        this.txt = fullTxt.substring(0, this.txt.length - 1);
        } else {
        this.txt = fullTxt.substring(0, this.txt.length + 1);
        }

        this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

        var that = this;
        var delta = 200 - Math.random() * 100;

        if (this.isDeleting) { delta /= 2; }

        if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
        } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
        }

        setTimeout(function() {
        that.tick();
        }, delta);
    };

    window.onload = function() {
        var elements = document.getElementsByClassName('typewrite');
        for (var i=0; i<elements.length; i++) {
            var toRotate = elements[i].getAttribute('data-type');
            var period = elements[i].getAttribute('data-period');
            if (toRotate) {
              new TxtType(elements[i], JSON.parse(toRotate), period);
            }
        }
        // INJECT CSS
        var css = document.createElement("style");
        css.type = "text/css";
        css.innerHTML = ".typewrite > .wrap { border-right: 0.08em solid #fff}";
        document.body.appendChild(css);
    };

export default {
    name : "ContainerLeft"
}
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css?family=Arimo|Poppins&display=swap');
    @media (max-width: 576px) { 
    #desc{
        font-size:5em;
    }

    }

    #wrapper{
    margin: 0px 40px;
    margin-top:40px;
    
    }
    #desc{
    margin-top:70px;
    font-size: 70px;
    /* font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; */
    font-style: normal;
    font-weight: bold;
    line-height: 80px;

    font-family: 'Poppins', sans-serif;

    }

    #detail{
    font-size: 20px;
    font-family: 'Courier New', Courier, monospace;
    line-height: 25px;
    }



    [stuff],[experience]{
        /* font-weight: bold; */
        font-size: 20px;
        font-family: 'Courier New', Courier, monospace;
        line-height: 25px;
        
    }

    #narration{
        margin-top:70px;
        padding-bottom: 80px;
    }

    
    .aboutme{
        border:1px solid #330033;
        color:#330033;
    }


    /* .typewrite{
        font-family: 'Arimo', sans-serif;
    } */
    @media (max-width: 576px) { 
    #description{
        margin-left:-35px;
    }

    }
</style>