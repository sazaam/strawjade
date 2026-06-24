# strawjade
Jade Templating Engine portage to browser-use Javascript

This project got changed, actually almost cancelled, 
I attempted to have a browser-use jade templating system, but after being complete on my part, (it simulated jade as I needed) I realized the original jade-browser.js library did the job in a completely different approach, and with much, much better results and stability.
The original jade template language got abandonned and changed into Pug.js, which I always thought very bothersome aon top of a very ugly name. Anyway, I forked backed latest version of jade.js (1.11) available on the internet and re-worked it in order to make all internal calls async. (it calls other jade files when requiring the 'extends' or 'include' patterns).


Now the strawjade.js file does nothing but require the other jade_async.js file internally, (beware of the ./strawnode_modules/ convention when working with [strawnode](github.com/sazaam/strawnode/)). If you only need jade templates, jade_async.js will work the same as original Jade (Jade.render(), Jade.parse() ...) for browser-use.


Aside from these latest Async modifications, all credits go to original Jade team owners, and the license is the same as jade's original one. 

It is the most fun, code-friendly easy-to-use templating engine in my opinion still today.