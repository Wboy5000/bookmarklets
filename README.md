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

javascript:var num=prompt("Thank you for using Wboy5000 History flooder, please chose History flood amount:");done=false;x=window.location.href;for (var i=1; i<=num; i++){history.pushState(0, 0, i==num?x:i.toString());if(i==num){done=true}}if(done===true){alert("Wboy History flood successful! this website you are on now appears in your history "+num+(num==1?" time.":" times."))}

inspect element

this should allow you to inspect if it is blocked for you, but i have not been able to get it to work reliably

javascript:(function () { var script = document.createElement('script'); script.src="//cdn.jsdelivr.net/npm/eruda"; document.body.appendChild(script); script.onload = function () { eruda.init() } })();

edit element

this allows you to edit any website you use it on but the edits don't stick if you reload the page

javascript:document.body.contentEditable = 'true'; document.designMode='on'; void 0

3d

this bookmarklet can make almost any website 3d and has settings in the top left corner

javascript:(function(){var js=document.body.appendChild(document.createElement("script"));js.onerror=function(){alert("Sorry, the script could not be loaded.")};js.src="https://rawgit.com/Krazete/bookmarklets/master/tri.js"})();

youtube video unblocker

javascript:(function () {if (window.location.toString().includes('www.youtube.com/watch?v%27)) { window.open(%27https://www.youtube-nocookie.com/embed/%27 + window.location.toString().split(%27=%27)[1]) }})()

Mini snake in browser

This is an extrmely fun mini pixelated snake

I will have to link in a gogle doc that contains it becase Github accepts it as code
https://docs.google.com/document/d/1jNxnbcLHjwjuLgMDp_Id_dHnAupV9BGnHjA8lZqKW3Q/edit?usp=sharing 

Tab cloack

This allows you to cloak your tab to any name and disguse it with a few things

(function () {document.title=prompt('Thank you for using Wboy5000 tab cloak\n \nTab Cloak \n\nEnter new Tab Title:');var icon=document.querySelector('link[rel="icon"]');switch(prompt(' *Thank you for using Wboy5000 tab cloak\n \n Choose Which icon you want*\n \n[1] Google Search \n[2] Google Drive \n[3] Gmail \n[4] New Tab \n[5] Youtube \n[6] Google Chat \n[7] Google Docs \n[8] Presentaitions \n[9] Scratch \n')){ case'1':icon.setAttribute('href','https://www.google.com/favicon.ico');break; case'2':icon.setAttribute('href','https://ssl.gstatic.com/images/branding/product/2x/hh_drive_96dp.png');break; case'3':icon.setAttribute('href','https://ssl.gstatic.com/ui/v1/icons/mail/rfr/gmail.ico');break; case'4':icon.setAttribute('href','https://i.imgur.com/rPKJ5NZ.png');break; case'5':icon.setAttribute('href','https://www.youtube.com/favicon.ico');break; case'6':icon.setAttribute('href','https://ssl.gstatic.com/ui/v1/icons/mail/images/favicon_chat_r2.ico');break; case'7':icon.setAttribute('href','https://ssl.gstatic.com/docs/documents/images/kix-favicon7.ico');break; case'8':icon.setAttribute('href','https://ssl.gstatic.com/docs/presentations/images/favicon5.ico');break; case'9':icon.setAttribute('href','https://scratch.mit.edu/favicon.ico');break;}})()
