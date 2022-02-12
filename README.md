# StopWatch
a simple StopWatch using only JavaScript

<h2>StopWatch</h2> 

<form name = "form_main">
  <div>
   
    <span id = "hour">00</span> :
    <span id = "minute">00</span> :
    <span id = "second">00</span> :
    <span id = "millisecond">000</span>
  </div>

  <br />
  <button type = "button" name = "start">start</button>
  <button type = "button" name = "pause">pause</button>
  <button type = "button" name = "reset">reset</button>
    
</form> 


<script>




var hour = 0
var minute = 0
var second = 0
var millisecond = 0

var cron 

document.form_main.start.onclick = () => start()
document.form_main.pause.onclick = () => pause()
document.form_main.reset.onclick = () => reset()


function start (){
  pause()
  cron = setInterval(() => {timer();}, 10)


}

function pause(){
  clearInterval(cron)

}

function reset(){
hour = 0
minute = 0
second = 0
millisecond = 0

document.getElementById('hour').innerText = "00"
document.getElementById('minute').innerText = "00"
document.getElementById('second').in
