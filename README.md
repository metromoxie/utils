utils
=====

General utilities with no other home.

delay-traffic is a shell script for adding delay to network traffic on your
Linux machine. This is useful in experiments where network delay matters but you
want to normalize the delay across your experiments. This is most useful when
you are doing local network access, otherwise general network delay will be
added in addition to the artificial latency, thus defeating the normalization
this provides.

jslint-rhino-wrap.js is a script for running the wonderful JavaScript code
quality tool JSLint on local files on the command line. This script is built to
run under the solid Mozilla Rhino platform, so make sure to install that first
before trying to use this script. The script also requires a local copy of
JSLint (https://raw.github.com/douglascrockford/JSLint/master/jslint.js). You
run the script script by uttering the following at the command line: rhino
jslint_rhino_wrap.js jslint.js [options]... [files]... You may find it useful to
write a script to specify a permanent path to your jslint.js file. Further
options are specified in the comments at the top of th script.
