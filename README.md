# Node-Red based Raspberry pi video player

## Media files

Video files should be located on a usb flash drive with a label of "VIDEO".

## Playlist mode
To read a playlist of videos, the video_config.json file on your USB flash drive should look like this:

```json
{
    "mode": "playlist",
    "playlist": ["video01.mp4", "video02.mp4"]
}
```

Where playlist is the list of video files you want to play.

## Button mode

If you want to trigger the video files using buttons connected to the GPIO pins, the video_config.json file on your USB flash drive should look like this:

```json
{
    "mode": "buttons",
    "playlist": ["video01.mp4", "video02.mp4"]
}
```

The playlist property is ignored in this case.

The following table shows what file will be triggered by which pin.  These are the physical pin numbers on the Raspberry pi.

| PIN    | File        |
|--------|-------------|
| PIN 3  | video01.mp4 |
| PIN 5  | video02.mp4 |
| PIN 7  | video03.mp4 |
| PIN 11 | video04.mp4 |




