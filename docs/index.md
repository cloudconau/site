---
hide:
  - toc
  - navigation
---

<style>
  #countdown_container {
    border: 1px solid blue;
    font-align: center;
    padding-left: 2em;
  }
  #demo {
    background-color: palegreen;
  }
</style>

# CloudCon Sydney 2025

<div id="countdown_container">
    <!-- Display the countdown timer in an element -->
    <h3 id="demo"></h3>
    <h3>Tickets are selling fast! <a href="https://regonsite.eventsair.com/cloudcon-2025/registration/Site/Register" target="_blank">Purchase your ticket.</a></h3>
</div>

<script>
// Set the date we're counting down to
var countDownDate = new Date("Sep 9, 2025 09:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();

  // Find the distance between now and the count down date
  var distance = countDownDate - now;

  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  // Display the result in the element with id="demo"
  document.getElementById("demo").innerHTML = "Countdown to CloudCon: " + days + "days " + hours + "hours "
  + minutes + "mins " + seconds + "seconds ";

  // If the count down is finished, write some text
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "EXPIRED";
  }
}, 1000);
</script>

Don’t miss CloudCon Sydney – happening 9–10 September 2025!

This premier cloud native event brings together global visionaries and local innovators for two days of hands-on learning, collaboration, and insight.

Connect directly with leaders from Kubernetes and other cutting-edge projects, and help shape the future of cloud native in Australia.

!!! success "Speaker Lineup"
    Half international speakers, half local experts – 100% unmissable.

    [View the lineup here!](agenda.md)

![KCD 2024](images/lobby.png)

## Questions?

Please contact the organisers via email: `organizers@kcdaustralia.onmicrosoft.com`