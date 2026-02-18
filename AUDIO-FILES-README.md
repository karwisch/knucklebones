# Default Audio Files Setup

This app uses default audio files that should be placed in the same folder as `index.html`.

## Required Files

Place these two audio files in the same directory as `index.html`:

```
knucklebones/
├── index.html
├── default-edit-sound.mp3      ← Edit cue sound (3-5 seconds)
└── default-finale-song.mp3     ← Finale song (full song)
```

## File Descriptions

### `default-edit-sound.mp3`
- **Purpose:** Plays when transitioning between scenes during the show
- **Duration:** 3-5 seconds recommended
- **Type:** Short sound effect or audio cue
- **Examples:** Ding, chime, drum hit, "edit" announcement

### `default-finale-song.mp3`
- **Purpose:** Plays at the end of the show during finale
- **Duration:** Full song (2-4 minutes typical)
- **Type:** Background music for finale scene
- **Examples:** Upbeat music, theme song, celebratory track

## File Format

- **Format:** MP3 (recommended) or any browser-supported audio format (WAV, OGG, M4A)
- **Bitrate:** Any (128-320 kbps recommended for good quality)
- **File size:** No strict limit, but smaller files load faster on mobile

## What Happens If Files Are Missing?

If the audio files are not found:
- The app will show **"Upload audio file"** instead of "Default edit sound"
- You can still use the app by uploading audio files manually via the UPLOAD buttons
- Console will show: `Could not load default edit sound from ./default-edit-sound.mp3`

## Testing

After adding the files:
1. Refresh the browser
2. Check console for: `✓ Default edit sound loaded successfully`
3. Look for "Default edit sound" (italicized) in the UI
4. Click the ▶ preview button to test playback

## Original Dropbox Files

The original default files were:
- Edit sound: `KnucklebonesEditSound.mp3` (from Dropbox)
- Finale song: `Silent-Partner-Mob-Battle-No-Copyright-Music.mp3` (from Dropbox)

If you have access to these original files, rename them:
- `KnucklebonesEditSound.mp3` → `default-edit-sound.mp3`
- `Silent-Partner-Mob-Battle-No-Copyright-Music.mp3` → `default-finale-song.mp3`

## Mobile Compatibility

✅ **Local files work great on mobile!**
- No CORS issues
- No network delays
- Reliable playback
- Faster loading

This is much better than the previous Dropbox-hosted files which had reliability issues on mobile devices.

## Troubleshooting

**"Upload audio file" shows instead of "Default edit sound"**
- Check that files are named exactly: `default-edit-sound.mp3` and `default-finale-song.mp3`
- Check that files are in the same folder as `index.html`
- Check browser console for error messages
- Try refreshing the page

**Audio doesn't play**
- Make sure files are valid MP3 files
- Try playing the files directly in your browser
- Check file permissions (should be readable)
- On mobile, tap "TAP TO ENABLE AUDIO" button first

**Console shows 404 errors**
- Files are not in the correct location
- Check file names are exactly correct (case-sensitive on some servers)
- Make sure you're accessing the app from the correct URL/folder
