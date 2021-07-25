<template>
  <div class="hello">
<!-- <!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width,initial-scale=1.0" />
    <link rel="icon" href="/favicon.png" />
    <title>Anthony Quits</title>
    <meta
      name="description"
      content="Anthony Gilbert quit nicotine. this is helping him along the way."
    />
    <meta itemprop="name" content="Anthony Quits" />
    <meta
      itemprop="description"
      content="Anthony Gilbert quit nicotine. this is helping him along the way."
    />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Anthony Quits" />
    <meta
      name="twitter:description"
      content="Anthony Gilbert quit nicotine. this is helping him along the way."
    />
    <meta name="twitter:site" content="@anthony_codes" />
    <meta name="twitter:creator" content="@anthony_codes" />
    <meta name="og:title" content="Anthony Quits" />
    <meta
      name="og:description"
      content="Anthony Gilbert quit nicotine. this is helping him along the way."
    />
    <meta name="og:type" content="website" />
    <link rel="stylesheet" href="app.css" />
  </head>
  <body> -->
    <div id="app">
      <header class="container">
        <h1>Anthony quits 🚬</h1>
        <p>
          <a href="https://twitter.com/anthony_codes" target="blank"
            >Anthony Gilbert</a
          >
          quit nicotine. this is helping him along the way.
        </p>
      </header>
      <div class="container flex">
        <div class="progress" fraction="seconds">
          <div class="left"></div>
          <div class="right">
            <h2></h2>
            <h3>Seconds</h3>
          </div>
        </div>
        <div class="progress" fraction="minutes">
          <div class="left"></div>
          <div class="right">
            <h2></h2>
            <h3>Minutes</h3>
          </div>
        </div>
        <div class="progress" fraction="hours">
          <div class="left"></div>
          <div class="right">
            <h2></h2>
            <h3>Hours</h3>
          </div>
        </div>
        <div class="progress" fraction="days">
          <div class="left"></div>
          <div class="right">
            <h2></h2>
            <h3>Days</h3>
          </div>
        </div>
      </div>
      <div class="container flex">
        <div class="progress" fraction="weeks">
          <div class="left"></div>
          <div class="right">
            <h2></h2>
            <h3>Weeks</h3>
          </div>
        </div>
        <div class="progress" fraction="months">
          <div class="left"></div>
          <div class="right">
            <h2></h2>
            <h3>Months</h3>
          </div>
        </div>
        <div class="progress" fraction="years">
          <div class="left"></div>
          <div class="right">
            <h2></h2>
            <h3>Years</h3>
          </div>
        </div>
        <div class="progress dark">
          <div class="right">
            <h2>
              <span>$<span id="dollars"></span></span
              ><small>.<span id="cents"></span></small>
            </h2>
            <h3>Saved</h3>
          </div>
        </div>
      </div>
      <div class="container">
        <div class="timeline">
          <div>
            <h3>1 Hour</h3>
            <p>Heart rate drops.</p>
          </div>
          <div>
            <h3>12 Hours</h3>
            <p>The carbon monoxide level in your blood drops to normal.</p>
          </div>
          <div>
            <h3>2 Weeks to 3 Months</h3>
            <p>
              Heart attack risk begins to drop. Lung function begins to improve.
            </p>
          </div>
          <div>
            <h3>1 to 9 Months</h3>
            <p>Coughing and shortness of breath decrease.</p>
          </div>
          <div>
            <h3>1 Year</h3>
            <p>
              Added risk of coronary heart disease is half that of a smoker's.
            </p>
          </div>
          <div>
            <h3>5 Years</h3>
            <p>Stroke risk is reduced to that of a nonsmoker’s.</p>
          </div>
          <div>
            <h3>10 Years</h3>
            <p>
              Lung cancer death rate is about half that of a smoker’s. Related
              cancer risks decrease.
            </p>
          </div>
          <div>
            <h3>15 Years</h3>
            <p>
              Risk of coronary heart disease is back to that of a nonsmoker’s.
            </p>
          </div>
          <p style="text-align: center;">
            <small
              ><a
                href="https://www.cdc.gov/tobacco/data_statistics/sgr/2004/posters/20mins/index.htm"
                target="blank"
                >cdc.gov</a
              >
              |
              <a href="https://github.com/anthonygilbertt" target="blank"
                >GitHub</a
              ></small
            >
          </p>
        </div>
      </div>
    </div>
    <!-- <script src="app.js"></script> -->

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
  
}

// const data = {
//   years: null,
//   months: null,
//   weeks: null,
//   days: null,
//   hours: null,
//   minutes: null,
//   seconds: null,
//   savings: null,
//   dollars: null,
//   cents: null,
//   dailyCost: 6.375466667,
//   time: 1569369600000 // new Date(2019, 8, 24, 19)
// };

// const progresses = document.querySelectorAll(".progress[fraction]");

// update();

// function update() {
//   const now = new Date().getTime();
//   const seconds = (now - data.time) / 1000;
//   data.years = seconds / 31556952;
//   data.months = seconds / 2592000;
//   data.weeks = seconds / 604800;
//   data.days = seconds / 86400;
//   data.hours = seconds / 3600;
//   data.minutes = seconds / 60;
//   data.seconds = seconds;
//   data.savings = data.days * data.dailyCost;
//   data.dollars = Math.floor(data.savings)
//     .toString()
//     .replace(/\B(?=(\d{3})+(?!\d))/g, ",");
//   data.cents = (data.savings - Math.floor(data.savings))
//     .toFixed(2)
//     .split(".")[1];
//   updatePies();
//   document.getElementById("dollars").innerText = data.dollars;
//   document.getElementById("cents").innerText = data.cents;

//   requestAnimationFrame(update);
// }

// function updatePies() {
//   const radius = 25;
//   const circumference = radius * 2 * Math.PI;
//   progresses.forEach(progress => {
//     const value = data[progress.getAttribute("fraction")];
//     const complete = Math.floor(value);
//     let v = complete.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ",");
//     if (complete < 10) v = value.toFixed(2);
//     if (complete < 1) v = value.toFixed(3);
//     progress.querySelector("h2").innerText = v;
//     const percent = Math.round((value - complete) * 100 * 10) / 10;
//     const offset = circumference - (percent / 100) * circumference;
//     progress.querySelector(
//       ".left"
//     ).innerHTML = `<svg xmlns="http://www.w3.org/2000/svg" height="100" width="100" viewBox="0 0 100 100">
//     <circle class="bg" r="${radius}" cx="50" cy="50" />
//     <circle
//       class="prog"
//       r="${radius}"
//       cx="50"
//       cy="50"
//       stroke-dasharray="${circumference} ${circumference}"
//       stroke-dashoffset="${offset}"
//     />
//   </svg>`;
//   });
// }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
