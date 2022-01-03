  * {
   --ss-transparent: #00000000;
    --ss-black: black;
    --ss-white: white;
    --ss-offwhite: black;
    --ss-yellow0: black;
    --ss-yellow: black;
    --ss-yolk0: black;
    --ss-yolk: black;
    --ss-yolk2: black;
    --ss-red0: black;
    --ss-red: black;
    --ss-red2: black;
    --ss-red-bright: black;
    --ss-pink: black;
    --ss-pink1: black;
    --ss-pink-light: black;
    --ss-brown: red;
    --ss-blue00:black;
    --ss-blue0: black;
    --ss-blue1: black;
    --ss-blue2: #c71616;
    --ss-blue3: red;
    --ss-blue4: red;
    --ss-blue5: red;
    --ss-green0: black;
    --ss-green1: black;
    --ss-green2: black;
    --ss-orange1: black;
    --ss-vip-gold: linear-gradient(to right, #D1A943, #CFCDAF, #CC8630, #D1AA44, #CC8630);
    --ss-gold: #D1AA44;
    --ss-clear: rgba(255, 255, 255, 0);
    --ss-blue2clear: black;
    --ss-shadow: black;
    --ss-blueshadow: black; 
    --ss-darkoverlay: rgba(0, 0, 0, 0.8);
    --ss-darkoverlay2: rgba(0, 0, 0, 0.2);
    --ss-lightoverlay: linear-gradient(0deg, rgba(0,0,0,1) 0%, rgba(255,0,0,1) 100%);
    --ss-lightbackground: rgba(0, 0, 0, 0.8);
    --ss-blueblend1: rgba(0, 0, 0, 0.8);
    --ss-scrollmask1: black;
    --ss-scrollmask2: black;
    --ss-fieldbg: linear-gradient(#91CADB, #ffffff, #ffffff, #ffffff, #ffffff);
    --ss-nugSecs: 3600s;
    --ss-white-60: rgba(255, 255, 255, .6);
    --ss-white-90: rgba(255, 255, 255, .9);
    --ss-me-player-bg: rgb(233, 13, 13);
    --ss-them-blue-bg: rgb(0, 0, 0);
    --ss-them-blue-color: black;
    --ss-them-red-bg: rgb(133, 0, 0, .8);
    --ss-them-red-color: #ff4145;
    --ss-me-red-bg: rgb(0, 0, 0);
    --ss-me-blue-bg: rgb(0, 0, 0);
    font-size: 1.95vh;
    scrollbar-width: thin;
    scrollbar-color: black
  }

 /**
 * Tooltip Styles
 */

/* Add this attribute to the element that needs a tooltip */
.tool-tip {
	position: relative;
	z-index: 2;
	cursor: pointer;
	margin: 0 .2em;
	transition: opacity ease-in-out .3s;
  }
  
  /* Hide the tooltip content by default */
.tool-tip span,
.tool-tip .tool-tip--bubble,
.tool-tip span:after,
.tool-tip div.tool-tip--bubble:after {
	transition: opacity ease-in-out .3s;
	visibility: hidden;
	opacity: 0;
	pointer-events: none;
}
.tool-tip span,
.tool-tip div.tool-tip--bubble {
	position: absolute;
	bottom: 115%;
	left: 50%;
	-webkit-transform: translateX(-50%);
	transform: translateX(-50%);
	margin-bottom: 5px;
	min-height: 2rem;
	width: 20em;
	font-weight: 600;
	line-height: 1.3;
	display: block;
  }

  .tool-tip span strong,
  .tool-tip .tool-tip--bubble strong {
	  font-weight: 800;
	  display: inline !important;
  }
  
  /* Triangle hack to make tooltip look like a speech bubble */
  .tool-tip span:after,
  .tool-tip div.tool-tip--bubble:after {
	background: 0;
	position: absolute;
	left: 50%;
	-webkit-transform: translate(-50%, 30%);
	transform: translate(-50%, 30%);
	width: 0;
	border-top: 1.7rem solid var(--ss-white);
    border-right: .8rem solid transparent;
    border-left: .8rem solid transparent;
	content: " ";
	font-size: 0;
	line-height: 0;
	filter: drop-shadow(4px 4px 0 var(--ss-blue2));
  }
  
/* Show tooltip content on hover */
.tool-tip.active span,
.tool-tip.active span:after,

.tool-tip:hover span,
.tool-tip span:after,

.tool-tip.active .tool-tip--bubble,
.tool-tip.active .tool-tip--bubble:after,

.tool-tip:hover .tool-tip--bubble,
.tool-tip:hover .tool-tip--bubble:after,
.tool-tip .tool-tip--bubble:after,
.tool-tip .tool-tip--bubble:hover {
	visibility: visible;
	opacity: 1;
}

.tool-tip--right span {
    bottom: 60%;
    left: 215%;
	z-index: 300;
}

.tool-tip--right span:after {
	bottom: auto;
    top: 18px;
    left: -16px;
	-webkit-transform: rotate(65deg);
	transform: rotate(65deg);
}



#event-notifications {
	margin-top: -3.9em;
}

#panel_front_play #event-notifications img {
	width: 10em;
}

/* Nugget popup */
#miniGameFrame {
	margin-bottom: 4em;
}

/* Nugget timer */
.chicken-panel--upgraded {
	position: fixed;
    left: 2.5em;
    bottom: 2.5em;
}
.chicken-panel--no-upgraded {
	position: fixed;
    left: 0;
    bottom: 0;
}
.nugget-timer--wrapper, .nugget-timer--wrapper * {
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
}

 .nugget-timer--wrapper:after {
    content: '';
    position: fixed;
    width: 9.7em;
    height: 9.7em;
    border: .3em solid var(--ss-yellow);
    border-radius: 100%;
    z-index: 1000;
    bottom: 1em;
    left: .8em;
}

.nugget-timer--wrapper:before {
	content: '';
    position: fixed;
    width: 7.1em;
    height: 7.1em;
    border: .3em solid var(--ss-yellow);
    border-radius: 100%;
    z-index: 50;
    bottom: 2.1em;
    left: 2.1em;
} */

.nugget-timer--wrapper {
  width: 8.1em;
  height: 8.1em;
}

.nugget-timer--wrapper .timer,
.nugget-timer--wrapper .timer-background,
.nugget-timer--wrapper .mask {
	border-style: solid;
	border-width: 1em;
	animation-iteration-count: 1 !important;
}

.nugget-timer--wrapper .timer {
  width: 50%;
  height: 100%;
  transform-origin: 100% 50%;
  position: absolute;
  border-color: var(--ss-yolk);
}

.nugget-timer--wrapper .spinner {
  border-radius: 100% 0 0 100% / 50% 0 0 50%;
  z-index: 200;
  border-right: none;
  animation: rota var(--ss-nugSecs) linear infinite;
}

.nugget-timer--wrapper:hover .spinner,
.nugget-timer--wrapper:hover .filler,
.nugget-timer--wrapper:hover .mask {
  animation-play-state: running;
}

.nugget-timer--wrapper .filler {
  border-radius: 0 100% 100% 0 / 0 50% 50% 0;
  left: 50%;
  opacity: 0;
  z-index: 100;
  animation: opa var(--ss-nugSecs) steps(1, end) infinite reverse;
  border-left: none;
}

.nugget-timer--wrapper .timer-background {
  width: 100%;
  height: 100%;
  position: absolute;
  background: none;
  border-color: var(--ss-blue3);
  border-radius: 100%;
  z-index: 100;
}

.nugget-timer--wrapper .mask {
  width: 50%;
  height: 100%;
  position: absolute;
  background: inherit;
  border-color: var(--ss-blue3);
  border-radius: 100% 0 0 100% / 50% 0 0 50%;
  border-right: none;
  opacity: 1;
  z-index: 300;
  animation: opa var(--ss-nugSecs) steps(1, end) infinite;
}

@keyframes rota {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
@keyframes opa {
  0% {
    opacity: 1;
  }
  50%, 100% {
    opacity: 0;
  }
}

/* Ad blocker 8 */
.ad-blocker-popup {
	position: relative;
	z-index: 4;
}

/* .wrapper .spinner,
.wrapper .filler,
.wrapper.mask {
	animation-delay: -1500s;
} */

/**--------------------------------Music Widget -------------*/
.in-game-widgets {
	position: absolute;
	left: 1em;
	bottom: 11em;
	z-index: 5;
}
.music-widget {
    min-width: 21.2em;
	max-width: 21.2em;
	margin-top: var(--ss-space-sm);
	background-color: white;
	padding: .7em;
	opacity: 1;
}

.music-widget--fade-out {
	opacity: 0;
	transition: opacity 1s linear;
}

/* .music-widget,
.music-widget--cover-image {
	border: var(--ss-space-sm) solid var(--ss-blue3);
} */
.music-widget--wrapper {
	display: flex;
	flex-wrap: nowrap;
}

.music-widget--content {
	order: 2;
	flex: 0 1 14em;
	overflow: hidden;
    padding: 0;
    margin: 0;
}

.music-widget--content header {
	background-color: var(--ss-blue3)
}

.music-widget--now-playing {
	font-size: .8em;
	padding-left: .4em;
	padding-right: .4em;
}

.music-widget--now-playing,
.music-widget--song-title,
.music-widget--album-title {
	margin: 0;
	text-align: left;
}

.music-widget--album-title,
.music-widget--song-title {
	font-size: .7em;

}

.music-widget--album-title a,
.music-widget--song-title a {
	font-size: 1em;
}

.music-widget--album-title,
.music-widget--album-title a,
.music-widget--song-title,
.music-widget--song-title a {
	white-space: nowrap;
	text-decoration: none;
}

.music-widget--album-title,
.music-widget--album-title a,
.music-widget--song-title,
.music-widget--song-title a,
.music-widget--album-title {
	color: var(--ss-blue3);
}

.music-widget--song-title {

}

.music-widget--content-wrapper {
	overflow: hidden;
	height: 1em;
}

.text-slide {
	padding-left: 100%;
	will-change: transform;
	animation: slide 15s linear infinite;
}

.music-widget--cover-image {
	order: 1;
	margin-right: .3em;
	height: 4em;
	flex: 0 0 4em;
	background-color: var(--ss-blue2);
	display: flex;
	flex-wrap: nowrap;
	align-items: center;
	justify-content: center;
	position: relative;
}

.music-widget--cover-controls button {
	background: none;
	border: 0;
}

.music-widget--cover-control-icon {
	display: none;
	position: relative;
	z-index: 2;
}

.music-widget--cover-image:hover .music-widget--cover-control-icon {
	display: block;
	cursor: pointer;
}

.music-widget--cover-image img {
	max-width: 3.5em;
	min-width: 3.5em;
}

.music-widget--cover-image .ss-absolute {
	position: absolute;
	position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.music-widget--sponsor {
	order: 3;
	margin-left: .3em;
	flex: 0 0 5%;
}

.music-widget--sponsor {
	display: flex;
	flex-direction: column;
	justify-content: space-between;

}

.music-widget--sponsor .music-widget--sponsor-icon {
	max-width: 100%;
	color: var(--ss-orange1);
}

.music-widget--volume-control input[type='range']::-webkit-slider-runnable-track {
	height: 10px;
	-webkit-appearance: none;
	color: white;
	margin-top: -1px;
}

.music-widget--volume-control h3,
.music-widget--volume-control label {
	font-size: .7em;
}

.music-widget--volume-control .ss_slider.label {
	color: var(--ss-blue3);
}

.music-widget--volume-control input[type=range]::-webkit-slider-runnable-track {
	cursor: pointer;
	background: var(--ss-blue3);
	height: .1em;
}
  
.music-widget--volume-control input[type=range]::-moz-range-track {
	cursor: pointer;
	background: var(--ss-blue3);
	height: .1em;
}
.music-widget--sponsor--settings-btn {
	background: none;
	border: 0;
	color: var(--ss-blue4);
	cursor: pointer;
}

/**---text color ---*/
.music-widget--cover-control-icon,
.music-widget--now-playing {
	color: var(--ss-white);
}

@keyframes slide {
	0% {
		transform: translate(0, 0);
	  }
	  100% {
		transform: translate(-200%, 0);
	  }
  }

/** ---------------------------------------------- PWA */
.btn-pwa {
	height: 2.5em;
	margin-top: .6em;
	cursor: pointer;
}
.btn-pwa-download {
	display: flex;
	align-items: center;
	padding: .3em;
	margin: 0 auto;
}
.pwa-btn-img-box {
	position: relative;
	margin-right: 1.5em;
}

.pwa-btn-img-box,
.pwa-btn-img-box img {
	height: 5em;
    width: 5em;
}
.pwa-btn-img-box i {
	position: absolute;
	bottom: 0;
	left: 0;
}
.pwa-popup .popup_sm_content{
	text-align: left;
	width: 90%;
}

  
  #subStorePopup {
	background: linear-gradient(red, black);
	padding-left: 5em;
	min-width: 45em;
    padding-right: 5em;
}

.shotReticle.fill.normal {
	border-color: black;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.3em;
	padding: 0.3em;
}

.shotReticle.border.normal {
	border-color: black;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.3em;
}

#logo {
	width: 100%;
	min-width: var(--ss-min-width);
	height: var(--ss-header-height);
	position: absolute;
	text-align: center;
	top: 3em;
	left: 0;
	margin: 0 auto;
	pointer-events: none;
}

#logo img {
	height: 100%;
	pointer-events: auto;
  content: url('https://www.linkpicture.com/q/image-removebg-preview-6_2.png');
}

#mainFooter {
	display: flex;
	flex-direction: row;
	height: var(--ss-footer-height);
	margin: 0 auto;
	width: 100%;
	position: relative;
	text-align: center;
	font-size: 0.8em;
	letter-spacing: 0.01em;
	min-width: var(--ss-min-width);
}
 
#mainFooter:after { /* Added Code  */ 
content: 'Theme For Vital by Skull ‎‏‏‎   ‏‏‎ ‎‏‏‎ ‎‏‏‎ ‎‏‏‎     ‎' !important;
font-family: 'Nunito', sans-serif;
 
    text-align: center;
  
  align-items: center;
 
  font-weight: bold;
    font-size: 1.9em;
    letter-spacing: 0.01em;
color: White;
}
 
.playerSlot--icons .hidden {
	display: none;
}
 
.playerSlot--icons i {
	margin-right: .2em;
}
 
.playerSlot--icons .vip-egg {
	text-shadow: 1px 1px 2px rgb(0 0 0 / 50%);
  content: url('https://www.linkpicture.com/q/image-removebg_1.png') !important;
  max-height: 1.1em;
  max-width: 1em;
}
.egg_icon {
	height: 2.0em;
	margin: var(--ss-space-micro) var(--ss-space-sm) 0 0;
  content: url('https://www.linkpicture.com/q/image-removebg_1.png')
}
 .egg_icon_sm {
	height: 1.8em;
	width: auto;
	margin: 0 var(--ss-space-micro) 0 var(--ss-space-md);
	margin-top: -0.10em;
	vertical-align: middle;
}

#killBox h3{
  display:none;
}
 
#killBox::before{
  font-size: 1em;
  font-weight: 900;
  content: 'YOU CLAPPED'!important;
  color: red;
}
#KILL_STREAK::before{
  display: normal !important;
}
#deathBox h3{
  display:none;
}
 
#deathBox::before{
  font-size: 1.3em;
  font-weight: 900;
  content: 'Clapped By'!important;
  text-shadow: black;
  color: red;
}
 
#healthContainer {
	position: absolute;
	left: 50%; bottom: 1em;
	transform: translateX(-50%);
	display: inline-block;
	width: 6em; height: 6em;
	background: #c00e0e;
	border-radius: 50%;
	text-align: center;
}
#grenadeThrow {
	width: 100%;
	height: 50%;
	border-radius: 0.05em;
	background: red;
}
 
#deathBox {
	position: absolute;
	display: none;
	width: 100%;
	transform-origin: center top;
	top: 17%;
	color: #000;
	text-align: center;
}
 
#gameMessage {
	position: absolute;
	display: gred;
	top: 45%; left: 60%;
	color: white;
	text-align: center;
	z-index: 6;
}
 
.chat {
	position: absolute;
	font-weight: bold;
	color: white;
	z-index: 6;
}
 
#chatOut {
	display: red;
	bottom: 2.5em;
	left: 1em;
 
}
 
#chatIn {
	display: none;
	color: white;
	bottom: 1em;
	left: 1em;
	width: 30%;
	border: white;
	background: red;
}
 
#killTicker {
	position: absolute;
	text-align: right;
	right: 1em;
	top: 10em;
	height: 7em;
	transform-origin: top right;
	text-shadow: #000;
}
 
 
#health {
}
 
#healthHp {
	font-family: 'Nunito', sans-serif;
    font-weight: bold;
    fill: black;
    font-size: 1.2em;
    transform: translateY(-3.45em);
}
 
.healthBar {
	transform-origin: center;
	transform: rotate(90deg);
	fill: black;
	stroke: red;
	stroke-width: 1em;
	stroke-dasharray: 14.4513em;
	transition: all 0.3s ease-in-out;
}
 
.healthYolk {
	fill: #771414c5;
}
 
.healthSvg {
	width: 100%; height: 100%;
}
 
 
#ammo {
	text-align: right;
	font-size: 3.22em;
	font-family: 'Nunito', sans-serif;
	font-weight: bold;
	line-height: 1em;
	margin: 0;
	
	padding-right: 1.40em;
	padding-top: 0em;
	margin-bottom: 0.1em;
 
	background-image: url('https://www.linkpicture.com/q/unnamed-removebg-preview_1.png');
    background-position: right center;
	background-size: 1em;
    background-repeat: no-repeat;
}
#best_streak_container h1 {
	margin: 0; padding: 0;
	display: inline;
 
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
 
	font-family: 'Nunito', sans-serif !important;
	font-size: 2.4em !important;
	color: var(--ss-white) !important;
	font-weight: bold !important;
	text-transform: lowercase;
 
	padding-left: 1.45em;
	padding-top: 0em;
 
	background-image: url('https://www.linkpicture.com/q/image-removebg-preview-2_4.png');
    background-position: left center;
	background-size: 1.37em;
    background-repeat: no-repeat;
}
#maskmiddle {
	background: url('https://media.discordapp.net/attachments/821765634844262432/834322579686424576/Vital.png') center center no-repeat;
	background-size: contain;
	width: 100vh;
	height: 100vh;
}
 
#maskleft, #maskright {
	background: black;
	flex: 1;
} 
  .account_eggs {
	display: flex;
	vertical-align: center;
	height: 2.3em;
	min-width: 6.4em;
	background: var(--ss-transparent);
	text-align: right;
	padding: 0.05em var(--ss-space-lg) 0 var(--ss-space-md);
	position: relative;
}
}
.crosshair {
	position: absolute;
	transform-origin: 50% top;
	top: 50%;
	border: solid 0.05em black;
	height: 0.8em;
	margin-bottom: 0.12em;
	opacity: 0.7;
 
	left: calc(50% - 0.15em);
	background: var(--ss-transparent);
	width: 0.3em;
}
.crosshair.normal {
	left: calc(50% - 0.15em);
	background: black;
	width: 0.3em;
}
 .crosshair.powerful {
   animation: colorchange 10s linear 1s infinite;
   -webkit-animation: colorchange 5s linear 0s infinite    alternate;
    position: absolute;
    transform-origin: 50% top;
    top: 50%;
    border: solid 0.05em black;
    height: 1.0em;
    margin-bottom: 0.12em;
    opacity: 0.9;

    left: calc(50% - 0.15em);
    background: colorchange !important;
    width: 0.3em;
 {
    position: absolute;
    transform-origin: 50% top;
    top: 50%;
    border: solid 0.05em black;
    height: 1.0em;
    margin-bottom: 0.12em;
    opacity: 0.9;

    left: calc(50% - 0.15em);
    background: colorchange !important;
    width: 0.3em;
}
    @keyframes colorchange
    {
      0%   {background: #ff0000;}
      20%  {background: #ad00ff;}
      40%  {background: #0033ff;}
      60%  {background: #00d7ff;}
      80%  {background: #2fff00;}
      100% {background: #ffd800;}
   }


#dotReticle {
	position: absolute;
	left: 50%; top: 50%;
	transform: translate(-50%, -50%);
	background: solid;
	width: 0.7em; height: 0.7em;
	border-radius: 100%;
}

#shotReticleContainer {
	position: absolute;
	text-align: center;
	left: 50%; top: 50%;
	transform: translate(-50%, -50%);
	opacity: 0.7;
	overflow-x: hidden;
}

#reticleContainer {
	position: fixed;
	top: 0; left: 0;
	width: 100%; height: 100%;
}

#crosshairContainer {
	position: absolute;
	left: 50%; top: 50%;
	transform: perspective(0px);
}

.shotReticle {
	box-sizing: border-box;
	position: absolute;
	left: 50%;
	width: 2.5em;
	height: 100%;
	transform-origin: center;
	background: transparent;
	border: solid;
	border-left: solid transparent;
	border-right: solid transparent;
	border-radius: 1.25em 1.25em 1.25em 1.25em;
}

.shotReticle:nth-child(1n) {
	transform: translateX(-50%) rotate(0deg);
}

.shotReticle:nth-child(2n) {
	transform: translateX(-50%) rotate(90deg);
}

.shotReticle.fill{
}

.shotReticle.border {
}

.shotReticle.fill.normal {
	border-color: black;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.1em;
	padding: 0.3em;
}

.shotReticle.fill.powerful { 
	animation: colorchange3 10s linear 1s infinite;
  -webkit-animation: colorchange3 3s linear 0s infinite alternate;
  border-color: inherit;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.3em;
	padding: 0.3em;
}
    @keyframes colorchange3
    {
      0%   {color: #ff0000;}
      20%  {color: #ad00ff;}
      40%  {color: #0033ff;}
      60%  {color: #00d7ff;}
      80%  {color: #2fff00;}
      100% {color: #ffd800;}
   }

.shotReticle.border.normal {
	border-color: black;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.1em;
}

.shotReticle.border.powerful {
  border-color: black;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.4em;
} 
#readyBrackets {
	position: absolute;
	left: 50%; top: 50%;
	transform: translate(-50%, -50%);
	opacity: 0.5;
}

#readyBrackets.ready {
	animation: armed 0.2s linear;
	width: 4em; height: 4em;
	border-color: rgb(0, 0, 0);
}

#readyBrackets.notReady {
	animation: unarmed 0.2s linear;
	width: 8em; height: 8em;
	border-color: rgb(255, 0, 0);
}

.readyBracket {
	position: absolute;
	width: 0.8em; height: 0.8em;
	border: solid;
	border-color: inherit;
	border-width: 0.3em 0 0 0.3em;
	transform-origin: top left;
}

.readyBracket:nth-child(1) {
	left: 100%;
	transform: rotate(90deg);
}

.readyBracket:nth-child(2) {
	left: 100%; top: 100%;
	transform: rotate(180deg);
}

.readyBracket:nth-child(3) {
	top: 100%;
	transform: rotate(270deg);
}

</style>`
    }
    document.body ? addScript() : document.addEventListener("DOMContentLoaded", e => addScript());
})();
