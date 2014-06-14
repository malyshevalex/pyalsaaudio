PyAlsaAudio
===========

Author: Casper Wilstrup (cwi@aves.dk)

Contributors: Tyler Yahn (codingalias@gmail.com)

This package contains wrappers for accessing the ALSA api from Python. It
is currently fairly complete for PCM devices. The next goal is to have
complete mixer supports as well. MIDI sequencer support is low on the
priority list, but volunteers are welcome.

This software is licensed under the PSF license - the same one used
by the majority of the python distribution. Basically you can use it
for anything you wish (even commercial purposes). There is no warranty
whatsoever.

Requirements
------------

A working install of ALSA with proper kernel support is needed.

The package has been verified to work with the following

  * [alsa-lib 1.0.27.2-1](http://www.alsa-project.org/main/index.php/Download)

Installation
------------

To install, first build the package:

```
  $ python setup.py build
```

And then, after verifying everything built successfully, as root:
  
```
# python setup.py install
```


Using the API
-------------

There is a reasonably useful API documentation included in the module
documentation, which can be found in the doc subdirectory of the source
distribution.

There are also three example programs included with the source:

  * `playbacktest.py`
   * Which plays back raw sound data read from stdin
  * `recordtest.py`
   * Which captures sound from the microphone at writes it raw to stdout.
  * `mixertest.py`
   * Which can be used to manipulate the mixers.
