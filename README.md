# libvlc-feature-requests

The goal of this repo is to track and put together a list of LibVLC APIs users and bindings maintainers would like to see come alive.

There are no commitment whatsoever whether they will ever be implemented and accepted into the main VLC tree.

## Performance benchmark mode
- Provide a way to initialize objects in "benchmark" mode. This could allow to log time spent in custom callbacks and compare with a test run with the default libvlc callbacks (no FFI interop), and provide a report somehow.

## Logging
- Per player logging.
- Formatted log callbacks. ( https://mailman.videolan.org/pipermail/vlc-devel/2019-May/124685.html )

## Plugin path
- libvlc_set_plugins_path function: VLC_PLUGIN_PATH can be unconvenient/unsufficient/unusable in some cases.

## Callbacks
- muxed callbacks API
- sout callbacks API
- records callback API
  - https://code.videolan.org/videolan/VLCKit/-/blob/master/libvlc/patches/0011-libvlc-media_player-Add-record-method.patch
  - https://code.videolan.org/videolan/VLCKit/-/blob/master/libvlc/patches/0012-libvlc-events-Add-callbacks-for-record.patch

## Filters
- audio/video GPU filters API
