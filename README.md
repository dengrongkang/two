<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<title>纯HTML5+CSS3实现一棵自己跳舞的树</title>
	<!--<link rel="stylesheet" href="css/lanren.css">-->
  <style rel="stylesheet">
  .trunk, .trunk div {
    background: #136086;
    /*border-radius:$w;*/
    width: 100px;
    height: 10px;
    position: absolute;
    left:50%;
    top:70%;
    margin-left: -10px;
    -webkit-animation-name: rot;
            animation-name: rot;
    -webkit-animation-duration: 2.02s;
            animation-duration: 2.02s;
    -webkit-animation-iteration-count: infinite;
            animation-iteration-count: infinite;
    -webkit-animation-direction: alternate;
            animation-direction: alternate;
    -webkit-transform-origin: 5px 5px;
        -ms-transform-origin: 5px 5px;
            transform-origin: 5px 5px;
    -webkit-animation-timing-function: ease-in-out;
            animation-timing-function: ease-in-out;

}
.trunk.trunk, .trunk div.trunk {
    bottom: 0;
    left: 50%;
    -webkit-animation-name: rot-root;
            animation-name: rot-root;
    -webkit-animation-duration: 2.5s;
            animation-duration: 2.5s;
}
.trunk > div, .trunk div > div {
    /*opacity:0.9;*/
    top: 0;
    left: 100px;
    -webkit-animation-duration: calc(inherit / 2);
            animation-duration: calc(inherit / 2);
    /* don't works  */
}
.trunk > div:nth-child(2), .trunk div > div:nth-child(2) {
    /*animation-duration:15s;*/
    -webkit-animation-name: rot-inv;
            animation-name: rot-inv;
    -webkit-animation-duration: 1.7s;
            animation-duration: 1.7s;
}

@-webkit-keyframes rot {
    from {
      -webkit-transform: rotate(15deg) scale(0.72);
              transform: rotate(15deg) scale(0.72);
    }
    to {
      -webkit-transform: rotate(45deg) scale(0.72);
              transform: rotate(45deg) scale(0.72);
    }
}

@keyframes rot {
    from {
      -webkit-transform: rotate(15deg) scale(0.72);
              transform: rotate(15deg) scale(0.72);
    }
    to {
      -webkit-transform: rotate(45deg) scale(0.72);
              transform: rotate(45deg) scale(0.72);
    }
}
@-webkit-keyframes rot-inv {
    from {
      -webkit-transform: rotate(-45deg) scale(0.72);
              transform: rotate(-45deg) scale(0.72);
    }
    to {
      -webkit-transform: rotate(-15deg) scale(0.72);
              transform: rotate(-15deg) scale(0.72);
    }
}
@keyframes rot-inv {
    from {
      -webkit-transform: rotate(-45deg) scale(0.72);
              transform: rotate(-45deg) scale(0.72);
    }
    to {
      -webkit-transform: rotate(-15deg) scale(0.72);
              transform: rotate(-15deg) scale(0.72);
    }
}
@-webkit-keyframes rot-root {
    from {
      -webkit-transform: rotate(-95deg);
              transform: rotate(-95deg);
    }
    to {
      -webkit-transform: rotate(-85deg);
              transform: rotate(-85deg);
    }
}
@keyframes rot-root {
    from {
      -webkit-transform: rotate(-95deg);
              transform: rotate(-95deg);
    }
    to {
      -webkit-transform: rotate(-85deg);
              transform: rotate(-85deg);
    }
}
  </style>
</head>
<body>
<!-- 代码部分begin -->
<div class="trunk"><div><div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div></div><div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div></div></div><div><div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div></div><div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div><div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div><div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div><div><div><div><div></div><div></div></div><div><div></div><div></div></div></div><div><div><div></div><div></div></div><div><div></div><div></div></div></div></div></div></div></div></div></div>
<!-- 代码部分end -->
</body>
</html>
