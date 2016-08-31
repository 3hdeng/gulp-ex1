canvas beginpath
fill

//=== git clone
https://github.com/ryanburgess/react-clock
https://github.com/apeman-react-labo/apeman-react-clock#readme



$ cd gulp-ex1
$ npm install
$ npm run test
$ ./node_modules/.bin/gulp example

$ open index.html, then browser
https://demo-react-clock-deng3h.c9users.io/react-clock/index.html

$

//===
http://jsfiddle.net/rainev/vx4r5qzv/
window.requestAnimationFrame

css
.circle {
  width: 240px;
  height: 240px;
  position: relative;
  border: 12px solid #000;
  border-radius: 50%;
  background: url(http://i.imgur.com/LQ4S51k.png);
  background-size: 240px 240px;
  background-repeat: no-repeat;
}

.face {
  width: 100%;
  height: 100%;
}

# :after selector inserts something after the content of each selected element(s).
# https://developer.mozilla.org/en-US/docs/Web/CSS/::after

.face:after {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 12px;
  height: 12px;
  margin: -6px 0 0 -6px;
  background: #000;
  border-radius: 6px;
  content: "";
  display: block;
}
# negative margin + positive padding

.hour {
  width: 0;
  height: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  margin: -4px 0 -4px -25%;
  padding: 4px 0 4px 25%;
  background: #000;
  transform-origin: 100% 50%;
}

.minute {
  width: 0;
  height: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  margin: -40% -3px 0;
  padding: 40% 3px 0;
  background: #000;
  transform-origin: 50% 100%;
}

.second {
  width: 0;
  height: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  margin: -40% -1px 0 0;
  padding: 40% 1px 0;
  background: #D40000;
  transform-origin: 50% 100%;
}

