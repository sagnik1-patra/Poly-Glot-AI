🇬🇧 British Accent Coach + Text-to-Speech

An interactive pronunciation coach and offline text-to-speech tool that helps you practice speaking English in a British accent.
It highlights pronunciation tips for tricky words, applies British spellings automatically (color → colour, theater → theatre), and uses Microsoft Hazel (en-GB) via Windows SAPI for speech.

✨ Features

✅ British Spelling Normalizer
Converts American spellings (color, organize, flavor) into British forms (colour, organise, flavour).

✅ Accent Coach
Highlights common pronunciation adjustments for British English:

Drop non-rhotic “r” (far → /fɑː/).

Keep crisp [t] (not American flapped [ɾ]).

Apply BATH /ɑː/ vowel (bath, dance, glass).

Apply LOT /ɒ/ vowel (hot, coffee, dog).

Maintain /juː/ in words like tune, student (BrE: /ˈstjuːdənt/).

✅ British TTS with Microsoft Hazel
Speaks text in a natural British accent (offline).

✅ Save Audio
Exports speech to a .wav file and auto-plays inside Jupyter Notebook.

📂 Project Structure
british-accent-coach/
│
├── accent_coach.py       # main script (coach + TTS)
├── demo_notebook.ipynb   # Jupyter interactive demo
├── README.md             # this file
└── samples/              # generated audio samples

⚙️ Requirements

Windows 10/11 with British voice installed (e.g., Microsoft Hazel).

Settings → Time & Language → Speech → Manage voices → Add voice → English (United Kingdom)

Python 3.9+ (64-bit)

Packages:

pip install pywin32 ipython

🚀 Usage
1. Run in Jupyter Notebook

Paste the full script into a notebook cell.
Then run:

msg = "Please organise the meeting at the theatre."


The system will:

Show British spelling version.

Print pronunciation tips.

Speak the sentence with Microsoft Hazel.

Save a .wav and auto-play it inline.

2. Run from Python Script
python accent_coach.py


Enter a sentence when prompted.

🎧 Example

Input:

colorful theater in the center


Output report:

Original: colorful theater in the center
Britishised: colourful theatre in the centre

Pronunciation tips:
 • theatre: Non-rhotic /r/
 • centre: Use /t/ clearly, no American flap


And you’ll hear Hazel say:

“Colourful theatre in the centre.”

🔊 Output Samples

british_practice.wav → spoken version of your input.

📝 Notes

Works offline (no internet required).

If engine.say doesn’t produce audio in Jupyter, use the “save + play” method.

Supports both live speech and WAV file generation.
![Confusion Matrix Heatmap](polyglot_confusion_heatmap.png)
💡 Future Improvements

Add IPA phoneme transcription with phonemizer
.

Extend coach with rhythm/intonation guidance.

Web app UI with Streamlit or Gradio.
Author
SAGNIK PATRA
