Begena web app: Play (instrument, recorder, audio import) + Tuner
- Upload index.html + samples/ to any static host over HTTPS (Vercel, Netlify, GitHub Pages). HTTPS is needed for the tuner microphone.
- Opening index.html straight from disk will not load the samples (the browser blocks fetch on file://).
- Tunings are in the K object, note -> sample file in NOTE (both near the top of the script).
- Import audio detects the tuning (Selamta / Wanen / Anchi Hoye) from the notes it hears; the tuning buttons are only a tie-breaker.
- The tuner reference (A = 440 Hz by default) is saved in the browser and is also used by Import audio.
