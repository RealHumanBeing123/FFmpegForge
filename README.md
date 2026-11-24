# FFmpegForge

Like GitKit, but for FFmpeg, and still offline. The HTML file is all that you need.

Pick a task, choose your options, and get a ready-to-run `ffmpeg` command that updates as you go. Nothing is sent anywhere: the page makes no network requests.

Tasks covered:
- Convert: change the format, video codec (H.264, H.265, AV1, VP9, or copy with no re-encoding), quality, speed, size, frame rate, audio codec, bitrate, channels and sample rate.
- Make a video smaller: pick how much smaller, shrink the picture, or aim for a file size such as "under 25 MB".
- Cut a clip: by start and end time or by length, either fast (no re-encoding) or exact.
- Audio: extract or convert to MP3, M4A, Opus, OGG, FLAC or WAV, choose an audio track, trim, change the volume and even out the loudness.
- Make a GIF: with a custom colour palette for much better quality, plus width, speed, colours and looping.
- Pictures from a video: one thumbnail, one every few seconds, every frame, or a contact sheet (grid of thumbnails).
- Pictures to video: a slideshow with seconds per picture, a fixed size with bars, and optional music.
- Edit: resize, crop (square, 16:9, 9:16, 4:5 or your own), rotate or flip, change speed (sound included), black and white, noise reduction, burn in subtitles, and change the volume.
- Logo or watermark: position, size, distance from the edge and see-through level.
- Combine: add or replace audio, mix in background music, and add a subtitle track.
- Join clips: fast (same format) or flexible (different sizes and formats).

Beyond the options themselves, I added a few more things:

- Explanation panel: it breaks the command into parts and says what each one does.

- Quick-start recipes: 20 examples such as MKV to MP4 without losing quality, squeezing a video under 25 MB, a fast cut, a GIF, a thumbnail, a vertical video for Reels and TikTok, a logo in the corner and quiet background music.

- Shell choices: bash/zsh, PowerShell or cmd, with the right quoting.

- General options: replace or protect existing files, quieter output, remove metadata, and a box for any extra options of your own.

- Warnings: for mismatches that FFmpeg would reject or that give odd results (for example H.264 inside WebM, an audio-only file name on a video task, size settings while copying, fast cuts that start at a keyframe, and a target file size that can only be approximate).

Only the options for the task you pick are shown, so the page stays short.

I ran the recipes and over 400 option combinations through a real copy of FFmpeg to check the commands work. The NVIDIA and Mac hardware encoders could not be tried here (no graphics card or Mac), so those two are untested.

Less common features (streaming, screen recording, two-pass encoding, filters beyond those above, hardware decoding) are left out. Use the extra options box or see `ffmpeg -h`.

You need FFmpeg installed to run the commands the page builds. The page itself works in any browser.

Just open `FFmpegForge.html` in any browser. It works with no internet connection.

<img width="740" height="976" alt="ff1" src="https://github.com/user-attachments/assets/890bedc3-8938-49f5-aaa7-bbedb83bc93d" />

