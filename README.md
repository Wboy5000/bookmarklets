# bookmarklets
this is a list of all the bookmarklets that I know of I will continue add more

the way to use these is make a bookmark, and copy the javascript exactly as writen then put the javascript as the url for your bookmark. To activate it just click on the bookmark. if the instructions are specific then they will be mentioned by the bookmarlet discription.


auto clicker bookmarklet

this bookmarklet can click up to 175 cps

javascript:var DELAY = 1;var autoClickerStyleElement = document.createElement("style");autoClickerStyleElement.innerHTML="*{cursor: crosshair !important;}";document.body.appendChild(autoClickerStyleElement);function addClicker(e) {if(!e.isTrusted) {return;}if(e.target.classList.contains("auto-clicker-target")) {e.target.classList.remove("auto-clicker-target");} else {e.target.classList.add("auto-clicker-target");}document.body.removeChild(autoClickerStyleElement);document.body.removeEventListener("click", addClicker);e.preventDefault();autoClick(e.target);}function autoClick(element) {if(element.classList.contains("auto-clicker-target")) {element.click();setTimeout(function(){ autoClick(element); }, DELAY);}}document.body.addEventListener("click", addClicker, 0);

3d webpage 

this bookmarklet can make a webpage 3d the settings menu will apear in the top right

javascript:(function(){var js=document.body.appendChild(document.createElement("script"));js.onerror=function(){alert("Sorry, the script could not be loaded.")};js.src="https://rawgit.com/Krazete/bookmarklets/master/tri.js"})();

snake hacks

this bookmarklet gives you some insane snake hacks. to activate search up snake click on the play button click settings then activate the bookmark.

javascript:(function () {req = new XMLHttpRequest(); req.open('GET', 'https://raw.githubusercontent.com/DarkSnakeGang/GoogleSnakeCustomMenuStuff/main/custom.js'); req.onload = function() { eval(this.responseText + 'snake.more_menu();'); }; req.send();})()

font bomb

a on screen bomb will be placed when mouse clicked that can move words. this is very buggy and I do not recomend.

javascript:(function () {var s = document.createElement('script');s.setAttribute('src', 'http://fontbomb.ilex.ca/js/main.js');document.body.appendChild(s);}());

add skip

this bookmarklet allows you to skip any add( on youtube only ).

javascript:if(document.getElementsByClassName("video-ads")[0].innerHTML !==""){ var banner = false; for(var i = 0; i < document.getElementsByClassName("ytp-ad-overlay-close-button").length; i++){ document.getElementsByClassName("ytp-ad-overlay-close-button")[i].click(); banner = true;} if(banner === false){ document.getElementsByClassName("html5-main-video")[0].currentTime = document.getElementsByClassName("html5-main-video")[0].duration; document.getElementsByClassName("ytp-ad-skip-button")[0].click();} }void 0;

history flooder

this bookmarklet can flood your history however many times you want. I do not recomend flooding with extremly high numbers 

javascript:var num=prompt("History flood amount:");done=false;x=window.location.href;for (var i=1; i<=num; i++){history.pushState(0, 0, i==num?x:i.toString());if(i==num){done=true}}if(done===true){alert("History flood successful! "+window.location.href+" now appears in your history "+num+(num==1?" time.":" times."))}

inspect element

this should allow you to inspect if it is blocked for you, but i have not been able to get it to work

javascript:(function () { var script = document.createElement('script'); script.src="//cdn.jsdelivr.net/npm/eruda"; document.body.appendChild(script); script.onload = function () { eruda.init() } })();
