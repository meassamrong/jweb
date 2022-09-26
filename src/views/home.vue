<template>
    <div class="home">
        <div class="walpaper">
            <img id="walpapers" alt="" src="https://thetravelauthor.com/wp-content/uploads/2022/06/angkorwat.jpg">
        </div>
        <div class="datetime">
        <div class="date">
          <span id="dayname">Day</span>,
          <span id="month">Month</span>
          <span id="daynum">00</span>,
          <span id="year">Year</span>
        </div>
        <div class="time">
          <span id="hour">00</span>: <span id="minutes">00</span>:
          <span id="seconds">00</span>
          <span id="period">AM</span>
        </div>
      </div>
        <div class="nav">

        </div>
    </div>


    <div class="control-footer">
        <div class="container">
            <div class="footer-menu">
                <ul>
                    <li><i class="bi bi-github"></i></li>
                    <li><i class="bi bi-chat-dots"></i></li>
                    <li><i class="bi bi-terminal"></i></li>
                    <li><i class="bi bi-x-diamond-fill"></i></li>
                    <li><i class="bi bi-person-circle"></i></li>
                    <li><i class="bi bi-lock"></i></li>
                    <li><i class="bi bi-discord"></i></li>
                </ul>
            </div>
        </div>

    </div>
</template>

<style>
#walpapers {
    width: 100%;
    height: 100vh;
    position: absolute;
    z-index: -1;
    filter: blur(3px);
    transform: scale(1.05) translate(-25px, 20px);
}
.times{
    position: absolute;
    z-index: 999;
    top: 5%;
    left: 50%;
    transform: translate(-50%);

}
.datetime{
    color: #fff;
    background: #10101e45;
    font-family: "Segoe UI", sans-serif;
    width: 340px;
    padding: 15px 10px;
    border: 3px solid #2E94E3;
    border-radius: 5px;
    -webkit-box-reflect: below 1px linear-gradient(transparent, rgba(255, 255, 255, 0.1));
    transition: 0.5s;
    transition-property: background, box-shadow;
  }
  
  .date{
    font-size: 20px;
    font-weight: 600;
    text-align: center;
    letter-spacing: 3px;
  }
  
  .time{
    font-size: 60px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .time span:not(:last-child){
    position: relative;
    margin: 0 6px;
    font-weight: 600;
    text-align: center;
    letter-spacing: 3px;
  }
  
  .time span:last-child{
    background: #2E94E3;
    font-size: 30px;
    font-weight: 600;
    text-transform: uppercase;
    margin-top: 10px;
    padding: 0 5px;
    border-radius: 3px;
  }















.control-footer {
    bottom: 5%;
    width: 100%;
    position: absolute;
    height: auto;
    position: fixed;
}
.footer-menu {
    text-align: center;
    background-color:rgba(255, 255, 255, 0.651);
    border-radius: 10px;

}
.footer-menu ul {
    font-size: 0px;
    padding: 0;
    margin: 0;
    list-style: none;
}

.footer-menu ul li {
    display: inline-block;
    font-size: 45px;
    padding: 0px 15px;
    cursor: pointer;
    transition: all 250ms linear;
    border-radius: 10px;
    margin-bottom: 5px;

}
.footer-menu ul li:hover {
    background-color: rgba(255, 255, 255, 1);
    font-size: 40px;

}
</style>