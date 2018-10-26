# Audio

## Tools

|What|Link|
|----|----|
|Audacity | ubuntu apt tool |
| sox, libsox-fmt-mp3 | ubuntu apt tool |
|DTMF tone decoder | [http://dialabc.com/sound/detect/index.html](http://dialabc.com/sound/detect/index.html)|

## Documentation

## Tips and Tricks

1. Check spectogram in Audacity.
2. You can create a spectrogram in `sox` as well:

   ```
   sox Manon.mp3 -n spectrogram
   ```

   produces

   ![](/images/spectrogram.png)
