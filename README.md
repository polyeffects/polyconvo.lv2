polyconvo.lv2
=============

modified from zeroconvolv2 to allow patch file setting and gain control. It is a [LV2](http://lv2plug.in) plugin to convolve audio signals.

Note that LV2 allows preset-bundles (many presets can be in a single bundle),
and a plugin can also have many of those preset-bundles.
(idea: "church reverb preset collection", "theatre reverb collection", etc.)


The plugin offers a framework for various IR sources (file, memory,
decoded virtual I/O).

The convolver adds one cycle (nominal block-size) latency and is able
to process any number of samples up to the nominal block-size, including
non-power-of-two blocksizes.

This plugin uses background processing and is suitable to process
long impulse-responses. Configurations up to true-stereo (4 channels)
are supported.

Only tested in Ingen and jalv.

Install
-------


```bash
make
sudo make install PREFIX=/usr
```
