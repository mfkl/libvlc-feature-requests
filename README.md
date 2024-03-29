# libvlc-feature-requests

The goal of this repo is to track and put together a list of LibVLC APIs users and bindings maintainers would like to see come alive.

There are no commitment whatsoever whether they will ever be implemented and accepted into the main VLC tree.

## Performance benchmark mode
- Provide a way to initialize objects in "benchmark" mode. This could allow to log time spent in custom callbacks and compare with a test run with the default libvlc callbacks (no FFI interop), and provide a report somehow.

## Logging
- Per player logging.
- Formatted log callbacks. ( https://mailman.videolan.org/pipermail/vlc-devel/2019-May/124685.html )
- Better logging granularity. Select a specific module for more detailed logging for example. some good ideas: https://gstreamer.freedesktop.org/documentation/tutorials/basic/debugging-tools.html?gi-language=c

## Plugin path
- libvlc_set_plugins_path function: VLC_PLUGIN_PATH can be unconvenient/unsufficient/unusable in some cases.

## Callbacks
- muxed callbacks API
- sout callbacks API
- records callback API https://code.videolan.org/videolan/vlc/-/merge_requests/206
  - https://code.videolan.org/videolan/VLCKit/-/blob/master/libvlc/patches/0011-libvlc-media_player-Add-record-method.patch
  - https://code.videolan.org/videolan/VLCKit/-/blob/master/libvlc/patches/0012-libvlc-events-Add-callbacks-for-record.patch

## Filters
- audio/video GPU filters API

## 360

- Force equirectangular playback API for badly/missing tagged 360 video
- Force bird eye view for properly tagged 360 video
- Add Quaternion viewpoint API (in addition to the existing Euler angles viewpoint API)

## Progress bar timing
- Higher update frequency for time/position events

## Multi vout support via libvlc_media_player_select_tracks_by_ids
to be able to build a video wall easily from window handles.

## Gapless playback

https://code.videolan.org/videolan/vlc/-/issues/549

## Change HWND target during playback

## Disable OSD by default
do not inherit by default and add API to turn it on/off
