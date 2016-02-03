# Node-Red based Raspberry pi video player

To read a playlist of videos, the video_config.json file in /boot should look like this:

```json
{
    "mode": "playlist",
    "playlist": ["video01.mp4", "video02.mp4"]
}
```

Where playlist is the list of video files you want to play.  These files should be located on a usb flash drive with a label of "VIDEO".

