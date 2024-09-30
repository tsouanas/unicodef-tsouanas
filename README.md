# unicodef-tsouanas

This project consist of my own [unicodef] input files, mostly
[ThaTeX]-influenced, together with their compiled outputs.
You can install and use them without installing [unicodef].

See [unicodefs.md] for a list of all sequences defined by the provided files in `defs/`.

See [unicodef] for more info on how to install and use these.

Also included is my Makefile that facilitates building and installing from within the repo.
First clone this repo:

```sh
git clone https://github.com/tsouanas/unicodef-tsouanas
```

## Using make(1):

Inside the `unicodef-tsouanas` directory you can run:

* `make` runs `unicodef.py` on `defs/*` generating files at `outfiles/`;
* `make install` copies all oufiles to `~/.unicodef/`;
* `make uninstall` removes `~/.unicodef/`;
* `make macosinstall` installs then copies `unicodefs.dict` to `~/Library/KeyBindings/DefaultKeyBinding.dict`;
* `make macosuninstall` uninstalls and also removes `~/Library/KeyBindings/DefaultKeyBinding.dict`;
* `make clean` removes all outfiles.

Since this repo already comes with the compiled outfiles, you do not need to run `make` in order to build them.
(You only need to do this if you want to edit the input files or add your own.)

**Warning for macOS users.**
If you are already using a `DefaultKeyBinding.dict`, then `make macosinstall`
will overwrite the existing file, and `make macosuninstall` will delete it.

[unicodefs.md]: unicodefs.md
[unicodef]:     https://github.com/tsouanas/unicodef
[ThaTeX]:       https://github.com/tsouanas/thatex

