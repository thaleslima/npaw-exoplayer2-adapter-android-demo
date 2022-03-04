# BUG: YouboraAdapter does not send the resume after pre-roll

## HOW TO SIMULATE THE BUG
1) run demo    
2) select the video HLS/Apple 4x3 basic stream
3) open logcat and filter by youbora
4) see logcat that youboraAdapter did not send the resume after pre-roll

## ATTENTION: this bug only happens when the startPosition is set in the player
``` Java
long startPositionMs = 30000;
player.setMediaItem(mediaItems.get(0), startPositionMs);
player.prepare();
```

logs:
![Logs](logs.png)
