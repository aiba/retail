
# retail

This script is much like `tail -F *` except it takes a directory and scans the containing files at runtime, watching for new files and continuously tailing the current set of files inside the given directory.

This is useful for e.g. `tail -f logs/`.

See also:
  * https://serverfault.com/questions/541852/tail-f-on-new-files
  * https://github.com/madivad/retail

I stole the name `retail` from [@madivad](https://github.com/madivad) but this new implementation is my own.  His implementation doesn't work on macos, unfortunately.

# Running

You need [babashka](https://github.com/borkdude/babashka) to run this.  On macos you can install this with `brew install borkdude/brew/babashka`.

Once babashka is installed, you can `chmod +x retail` and run it directly.

# Example Usage:

```bash
retail ./logs/
```
