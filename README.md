# DeepVoice Studio (PWA starter)

## মোবাইল থেকে চালানোর সবচেয়ে সহজ উপায়
1. ZIP ফাইলটি Extract করুন।
2. `index.html`, `manifest.webmanifest` এবং `sw.js` একই ফোল্ডারে রাখুন।
3. এই ফোল্ডারটি GitHub repository-তে upload করুন।
4. Repository Settings → Pages → Deploy from branch → `main` এবং `/ (root)` নির্বাচন করে Save করুন।
5. GitHub Pages-এর HTTPS লিংক Android Chrome-এ খুলুন।
6. Chrome-এর menu থেকে **Install app** বা **Add to Home screen** চাপুন।

## কী আছে
- Audio file import এবং microphone recording
- Documentary / Islamic History / News / Natural Deep presets
- Pitch, bass, low-mid, presence, compressor, noise gate এবং limiter controls
- Before/After toggle
- WAV export
- MP3 export (প্রথমবার encoder CDN থেকে আনতে ইন্টারনেট প্রয়োজন)

## সীমাবদ্ধতা ও সতর্কতা
- Pitch control resampling ব্যবহার করে, তাই pitch কমালে playback duration-ও বাড়ে। এটি উচ্চমানের pitch-preserving time-stretch নয়।
- Noise gate নীরব অংশে noise কমায়; চলমান fan/traffic noise-এর পূর্ণ AI removal নয়।
- MP3 encoder প্রথমবার CDN থেকে লোড হয়। WAV export অফলাইনে কাজ করে।
- এটি একটি প্রাথমিক PWA prototype, native Android APK নয়।
- বড় অডিও ফাইল প্রসেস করতে ফোনের RAM ও ব্রাউজারের সীমা প্রভাব ফেলতে পারে।
