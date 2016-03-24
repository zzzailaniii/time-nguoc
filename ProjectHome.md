function setcountdown(theyear,themonth,theday,thehour,theminute){
yr=theyear;mo=themonth;da=theday;ho=thehour; mi=theminute;
}
//////////CONFIGURE THE COUNTDOWN SCRIPT HERE//////////////////
//STEP 1: Configure the countdown-to date, in the format year, month, day:

//STEP 2: Change the two text below to reflect the occasion, and message to display on that occasion, respectively
var occasion="Tết"
var message\_on\_occasion="Chút Xíu Nữa Thôi À"
//STEP 3: Configure the below 5 variables to set the width, height, background color, and text style of the countdown area
var countdownwidth='500px'
var countdownheight='20px'
var countdownbgcolor='#ffffff'
var opentags='<font face='Verdana'><b>

<large>

'<br>
var closetags='<br>
<br>
</large><br>
<br>
</b<br>
<br>
Unknown end tag for </font><br>
<br>
'<br>
//////////DO NOT EDIT PASS THIS LINE//////////////////<br>
var montharray=new Array("Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec")<br>
var crosscount=''<br>
function start_countdown(){<br>
if (document.layers)<br>
document.countdownnsmain.visibility="show"<br>
else if (document.all||document.getElementById)<br>
crosscount=document.getElementById&&!document.all?document.getElementById("countdownie") : countdownie<br>
countdown()<br>
}<br>
if (document.all||document.getElementById)<br>
document.write('<span></span>')<br>
window.onload=start_countdown<br>
function countdown(){<br>
var today=new Date()<br>
var todayy=today.getYear()<br>
if (todayy < 1000)<br>
todayy+=1900<br>
var todaym=today.getMonth()<br>
var todayd=today.getDate()<br>
var todayh=today.getHours()<br>
var todaymin=today.getMinutes()<br>
var todaysec=today.getSeconds()<br>
var todaystring=montharray<a href='todaym.md'>todaym</a>+" "+todayd+", "+todayy+" "+todayh+":"+todaymin+":"+todaysec<br>
futurestring=montharray[mo-1]+" "+da+", "+yr +" "+ho+":"+mi+":00"<br>
dd=Date.parse(futurestring)-Date.parse(todaystring)<br>
dday=Math.floor(dd/(60*60*1000*24)<b>1)<br>
dhour=Math.floor((dd%(60*60*1000*24))/(60*60*1000)</b>1)<br>
dmin=Math.floor(((dd%(60*60*1000*24))%(60*60*1000))/(60*1000)