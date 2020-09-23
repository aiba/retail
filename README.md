
This is a script that is much like `tail -F *` except it takes a directory and expands it into files at runtime, watching for new files and continuously tailing the current set of files inside that directory.

This is useful for e.g. `tail -f logs/`.

See also:
  * https://serverfault.com/questions/541852/tail-f-on-new-files
  * https://github.com/madivad/retail

I stole the name from @madivad.  His implementation doesn't work on macos, unfortunately.

