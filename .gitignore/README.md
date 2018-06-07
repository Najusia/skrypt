// Skrypt
// @name SoundsTips
// @namespace None
// @author NoNameGame
// @description Sounds
// @include https://showup.tv/
// @grant none
// @run-at document-end
//
// ==/UserScript==
if ( window.location.pathname === "/site/start_transmission" || window.location.pathname.match(/^\/prv/) ) {
var mSoundTips = [
=new Audio("C:\Program Files\sounds\11.mp3"),
=new Audio(" https://freesound.org/people/pooky1/sounds/398237/"),
=new Audio(" https://freesound.org/people/rekks888/sounds/342616/"),
=new Audio(" https://freesound.org/search/?q=hip+hop"),
=new Audio(" https://www.youtube.com/watch?v=M807UwF3-oU"),
=new Audio(" https://freesound.org/people/Drakensson/sounds/428954/"),
];
var mTokenNumber = parseInt(document.getElementById("tokensCountContainer").)
setInterval(function() {
var tokens = parseInt(document.getElementById("tokensCountContainer").innerText),
added = tokens - mTokenNumber,
soundId = -1;
if ( added >= 10 && added <= 11 )
soundId = 0;
else if ( added >= 12 && added <= 14 )
soundId = 1;
else if ( added >= 15 && added <= 15 )
soundId = 2;
else if ( added >= 16 && added <= 49 )
soundId = 3;
else if ( added >= 50 && added <= 99 )
soundId = 4;
else if ( added >= 100 && added <= 999 )
soundId = 5;
else if ( added >= 1000 )
soundId = 5;
if ( soundId >= "0" ) {
mSoundTips[soundId].play();
mTokenNumber = tokens;

}, 250);

