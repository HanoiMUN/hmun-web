+++
title = "home"
template = "index.html"
page_template = "page.html"
+++

<style>
div img {
  margin: 0 auto;
  width: 200px;
  height: auto;
}

table {
  margin: 0 auto;
}

div p{
  font-size:60px;
  margin-bottom:-20px;
  padding:20px ;
}

</style>

# EARLY BIRD DEADLINE COUNTDOWN
<div class="text-center place-content-center flex ">
  <div>
    <p id="days" >00</p><span>Days</span>
  </div>
  <div>
    <p id="Hours">00</p><span>Hours</span>
  </div>
  <div>
    <p id="Minutes">00</p><span>Minutes</span>
  </div>
  <div>
    <p id="Seconds">00</p><span>Seconds</span>
  </div>
</div>

<div>
    <script>
        var deadline = new Date("April 3, 2024 23:59:00 UTC").getTime();
        var x = setInterval(function() {
            var now = new Date().getTime();
            var t = deadline - now;
            var days = Math.floor(t / (1000 * 60 * 60 * 24));
            var hours = Math.floor((t%(1000 * 60 * 60 * 24))/(1000 * 60 * 60));
            var minutes = Math.floor((t % (1000 * 60 * 60)) / (1000 * 60));
            var seconds = Math.floor((t % (1000 * 60)) / 1000);
            document.getElementById("days").innerHTML =days ;
            document.getElementById("Hours").innerHTML =hours;
            document.getElementById("Minutes").innerHTML = minutes;
            document.getElementById("Seconds").innerHTML =seconds;
            if (t < 0) {
                clearInterval(x);
                document.getElementById("days").innerHTML ='00';
                document.getElementById("Hours").innerHTML ='00';
                document.getElementById("Minutes").innerHTML ='00';
                document.getElementById("Seconds").innerHTML = '00';
            }
        }, 1000);
    </script>
</div>

<br />

# Committees

||||
|---|---|---|
|[![ilo](/ilo.png)](/reg-for-delegate)|[![imo](/imo.png)](/reg-for-delegate)|[![ec](/ec.png)](/reg-for-delegate)|

|||
|---|---|
|[![jhcc](/jhcc.png)](/reg-for-delegate)|[![ad-hoc](/adhoc.png)](/reg-for-delegate)|

<br />

[![register for delegate](/reg-btn.png)](/reg-for-delegate)

<br />

[![register for delegation](/reg-delegations.png)](/reg-for-delegation)

<br />

[![register for observer](/nut-ob.png)](/reg-for-observer)

