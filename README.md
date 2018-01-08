navi.el 
=========

This library implements rendering of popup box with "Navi, the fairy" from The Legend of Zelda, Ocarina of Time. You can make her say various things by calling `navi-say` function. To hide the pop-up, simply invoke any command (move forward/backward, type, `C-g` etc., any event is recognized).

By default Navi show tip using `pos-tip`. you may prefer using `popup`.

`(setq navi-tip-show-function #'navi-popup-tip-show)`

As inspiration, two functions are provided: `navi-describe-function` and `navi-describe-variable`. Bind any of these functions to a key, then while point is over a function/variable, call it. A popup with helpfull Navi will appear, telling you about the function/variable (using `describe-function` and `describe-variable` respectively).

This package depends on `pos-tip` or `popup`.

Code is pretty much word-for-word stolen from (and is forked from): https://github.com/Fuco1/clippy.el
Original code is roughly based on: http://www.emacswiki.org/emacs/PosTip#toc3

The original inspiration to write the clippy package came from [http://www.geekzone.co.nz/foobar/5656](http://www.geekzone.co.nz/foobar/5656), a crazy discussion on #emacs and Fuco1's terrible headache stopping him from doing anything more productive.

Mine was because I grew up with the game and writing this similarly made it easier for me to procrastinate any real work.
