## [6.7.31] - 2022-02-04
### Changed
- Now join `Timer` fires join when content is live.

## [6.7.30] - 2022-02-03
### Added
- Join `Timer` started when `fireStart()` is called.

## [6.7.29] - 2021-11-29
### Added
- Title and resource retrieved automatically.

## [6.7.28] - 2021-11-19
### Added
- ExoPlayer 2.16 support.

## [6.7.27] - 2021-10-1
### Added
- ExoPlayer 2.15 support.
- Audio codec, video codec & urlToParse.

## [6.7.26] - 2021-09-02
### Fixed
- Workaround to avoid implementing empty ExoPlayer listeners.

## [6.7.25] - 2021-05-21
### Added
- windowChangedListener for resource and title reporting on playlists.

## [6.7.24] - 2021-05-17
### Added
- ExoPlayer 2.14 support.

## [6.7.23] - 2021-04-30
### Added
- ExoPlayer 2.13 new EventListeners overriden in Exoplayer2Adapter.

## [6.7.22] - 2021-04-19
### Fixed
- Join time after a pre-roll.

## [6.7.21] - 2021-04-15
### Fixed
- Ad quartiles.

## [6.7.20] - 2021-03-26
### Fixed
- Video events being triggered when an ad is playing.

## [6.7.19] - 2021-03-09
### Modified
- Deployment platform, moved from Bintray to JFrog.

## [6.7.18] - 2021-01-26
### Removed
- setBitrate method.
### Added
- More detailed HttpDataSourceException error report.

## [6.7.17] - 2021-01-11
### Fixed
- Pause and buffer being sent while playing an ad.

## [6.7.16] - 2020-12-11
### Added
- Ad quartiles.

## [6.7.15] - 2020-10-30
### Added
- QualityProvider released when unregistering listeners.

## [6.7.14] - 2020-10-27
### Added
- Live detection improved.

## [6.7.13] - 2020-10-26
### Fixed
- fireJoin() being sent on stateChangeReady() even if not live.

## [6.7.12] - 2020-09-25
### Added
- New methods implemented.

## [6.7.11] - 2020-09-23
### Added
- ExoPlayer 2.12 support.
  
## [6.7.10] - 2020-09-22
### Added
- Latency.

## [6.7.9] - 2020-08-06
### Added
- Exoplayer2AdAdapter class.

## [6.7.8] - 2020-08-05
### Fixed
- fireStart() & fireJoin() restricted when ad playing.

## [6.7.7] - 2020-07-23
### Fixed
- Error was not getting reported properly when it was of type source.

## [6.7.6] - 2020-07-06
### Updated
- Bump to ExoPlayer 2.11.7

## [6.7.5] - 2020-05-27
### Fixed
- Extra check for error type to add more info and prevent a crash in case of different type.

## [6.7.4] - 2020-05-22
### Added
- If InvalidResponseCodeException occurs, fireError will send its responseMessage in the metadata.

## [6.7.3] - 2020-05-04
### Added
- TotalBytes support.

## [6.7.2] - 2020-03-12
### Fixed
- Playrate.

## [6.7.1] - 2020-03-03
### Updated
- Youboralib version.

## [6.7.0] - 2020-02-13
### Refactored
- Adapter to work with the new Youboralib version.
### Removed
- Exoplayer2P2PAdapter.

## [6.6.6] - 2020-02-12
### Fixed
- To prevent some unexpected behaviour join time has been disabled on Exoplayer2HandlerAdapter

## [6.6.5] - 2020-02-06
### Fixed
- Race condition when removing listeners on Exoplayer2HandlerAdapter

## [6.6.4] - 2020-01-15
### Improved
- Use Player class instead of ExoPlayer class for all adapters (thanks to taku_semba).

## [6.6.3] - 2019-12-18
### Updated
- Exoplayer 2.11.0.

## [6.6.2] - 2019-12-17
### Updated
- Exoplayer 2.10.6.

## [6.6.1] - 2019-12-05
### Updated
- Youboralib version.

## [6.6.0] - 2019-11-22
### Added
- Adapter refactored.
- Player running in a non-UI thread support.

## [6.5.3] - 2019-10-22
### Added
- Dropped frames.
- System73 P2P support.

## [6.5.2] - 2019-10-11
### Improved
- Seek accuracy.

## [6.5.1] - 2019-09-18
### Added
- Exoplayer2StreamrootAdapter class.
- Teltoo P2P support.
### Deprecated
- Exoplayer2P2PAdapter class.

## [6.5.0] - 2019-09-03
### Added
- Playrate.

## [6.4.1] - 2019-06-05
### Added
- Streamroot P2P support.

## [6.4.0] - 2019-04-29
### Added
- IMA extension improvements.

## [6.3.4] - 2019-04-03
### Fixed
- Buffer should be now working as expected.

## [6.3.3] - 2019-03-15
### Fixed
- Now the Exoplayer2Adapter class is open.
- The events buildQualityProvider(), stateChangedBuffering(), stateChangedEnded(), 
stateChangedIdle(), stateChangedReady(), stateChangedPlayWhenReady() are open now.
- ExoPlayer event listeners are now implemented in Exoplayer2Adapter class.

## [6.3.2] - 2019-02-20
### Added
- In case of not wanting to fire start (and therefore joinTime) now there is a flag to disable it.
- BehindLiveWindowException is not considered fatal anymore.

## [6.3.1] - 2019-02-04
### Added
- Adapter migrated to Kotlin.

## [6.3.0] - 2018-12-18
### Updated
- Youboralib version updated to 6.3.1.

## [6.2.0] - 2018-11-08
### Added
- Support for Exoplayer 2.9.
- Infinity support.
### Fixed
- Crash when bitrate from CustomEventLogger is null.

## [6.0.16] - 2018-09-07
### Fixed
- Exception when not setting CustomEventLogger.

## [6.0.15] - 2018-09-05
### Added
- Now the CustomEventLogger class is included within the adapter.
### Fixed
- Disabled joinTime timer when EBVS.
- JoinTime not sent after ad on live.

## [6.0.14] - 2018-07-20
### Fixed
 - Fix rendition bitrate for HLS.
 
## [6.0.13] - 2018-07-10
### Fixed
 - Fix join time for live videos.

## [6.0.12] - 2018-06-27
### Added
 - Support for ExoPlayer 2.8.
### Fixed
 - Some cases join time could not be fired.

## [6.0.11] - 2018-05-22
### Fixed
 - Join time in case of IMA extension.

## [6.0.10] - 2018-05-14
### Added
 - Use STATE_IDLE or STATE_ENDED to stop playback.

## [6.0.9] - 2018-03-23
### Added
 - Support for ExoPlayer 2.7.
 - Compiled with YouboraLib 6.1.4.

## [6.0.8] - 2018-02-19
### Added
 - Compiled with YouboraLib 6.1.1.

## [6.0.7] - 2018-02-13
### Added
 - Compiled with YouboraLib 6.1.0.

## [6.0.6] - 2018-01-10
### Added
 - Support for ExoPlayer 2.6.
 
## [6.0.5] - 2018-01-10
### Added
 - Last version supporting ExoPlayer 2.5.
 - Offline mode to example.
 
## [6.0.4] - 2017-12-22
### Added
 - Last version supporting ExoPlayer 2.4.
 - Update to YouboraLib 6.0.9.
 
## [6.0.3] - 2017-12-18
### Added
 - Default playhead in case of live.
 
## [6.0.2] - 2017-12-15
### Added
 - Null check on playhead.
 - Automatic joinTime even when playback doesn't start from begining.
 
## [6.0.1] - 2017-10-06
### Added
 - Update ExoPlayer to 2.4.3.
 
## [6.0.0] - 2017-07-18
### Added
 - First release.