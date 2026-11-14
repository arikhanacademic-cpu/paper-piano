# Paper Piano

Play a piano printed on paper, using your webcam and your browser. No install.

![Demo](demo.gif)

## Try it

[Play Paper Piano](https://arikhanacademic-cpu.github.io/paper-piano/)

## How to play

1. Print [the keyboard PDF](paper-piano-keyboard.pdf) at 100% scale.
2. Tape it down on a flat surface.
3. Point a camera at it from above or from in front at roughly 45 degrees.
4. Open the app and start the camera.
5. Click the four red corner dots in order 1-2-3-4.
6. Tap the keys to play.

## How it works

A homography maps the four corner dots to the keyboard layout. MediaPipe tracks all ten fingertips. A tap is detected as a fast downward movement relative to the wrist that suddenly stops. Notes play using Salamander Grand Piano samples via the Web Audio API.

## Tips

- Good lighting helps.
- Use the sensitivity slider to adjust tap detection.
- Switch to Slide mode if taps aren't detected.
- On a Mac, an iPhone works as a webcam via Continuity Camera.

## Credits

- MediaPipe (Google)
- Salamander Grand Piano samples
- Inspired by earlier paper piano projects.

## Run locally

Run `python3 -m http.server` in the project folder and open http://localhost:8000.

The camera needs HTTPS or localhost.
