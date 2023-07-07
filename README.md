# python-rtmidi-wheels

## Notice

This repository has been deprecated with the release of [python-rtmidi][1]
1.5.0-1.5.4 which has introduced 3.10/3.11 wheels to the original package,
additionally with Linux and Apple Silicon wheels! 🎉

## Description

A repository hosting CPython prebuilt wheels for the [python-rtmidi][1] package.
Only python-rtmidi 1.4.9 wheels are available at this time.

When installing python-rtmidi with pip, the [`--find-links`][2] parameter
can be used to append this repository's wheel in the index. For example:

```sh
pip install --find-links https://thegamecracks.github.io/python-rtmidi-wheels/ python-rtmidi
```

This is only necessary when installing for CPython 3.10 or 3.11, as
wheels already exist on PyPI for older versions. Once the original
package releases 3.10/3.11 wheels, this project will be deprecated.

Credits to [liudonghua123's fork][3] for building 3.10 and 3.11 wheels
that were currently missing from the PyPI release of python-rtmidi.
This repository was made to make it easier to install `python-rtmidi`
on CPython 3.10 and 3.11 via pip, rather than manually downloading the
wheels from their release page.

[1]: https://pypi.org/project/python-rtmidi/
[2]:https://pip.pypa.io/en/stable/cli/pip_install/#cmdoption-f
[3]: https://github.com/liudonghua123/python-rtmidi
