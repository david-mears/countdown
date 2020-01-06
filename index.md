<h1>DAYS UNTIL CHRISTMAS</h1>

<h1 id="countdown" style="font-size:8vw;">Something went wrong</h1>

<script>
    // var daysRemaining = "4"
    // document.getElementById("countdown").innerHTML = daysRemaining;

    // Set the date we're counting down to
    var countDownDate = new Date("December 25, 2020 00:00:00").getTime();


    var now = new Date().getTime();

    // Find the distance between now and the count down date
    var distance = countDownDate - now;

    // Time calculations for days, hours, minutes and seconds
    var days = Math.floor(distance / (1000 * 60 * 60 * 24));

    // Display the result in the element with id="demo"
    document.getElementById("countdown").innerHTML = days;

    // If the count down is finished, write some text
    if (distance < 0) {
        document.getElementById("countdown").innerHTML = "EXPIRED";
    }
</script>
