# APK বানানোর ধাপ (৫ মিনিট, ফ্রি)

1. github.com এ লগইন করে **New repository** বানাও (নাম: study-hub, Public বা Private দুটোই চলবে)।
2. রিপোতে **Add file → Upload files** চাপো। এই ZIP আনজিপ করে ভেতরের সব ফাইল/ফোল্ডার (`www`, `.github`, `package.json`, `capacitor.config.json`, `.gitignore`) টেনে ছেড়ে দাও। **Commit changes** চাপো।
   - `.github` ফোল্ডার ফোনে/ফাইল ম্যানেজারে লুকানো থাকতে পারে। লুকানো ফাইল দেখার অপশন অন করো। না পেলে Add file → Create new file এ গিয়ে নাম দাও `.github/workflows/build-apk.yml` আর ফাইলের লেখা পেস্ট করো।
3. রিপোর **Actions** ট্যাবে যাও। "Build APK" চলতে শুরু করবে (৪-৬ মিনিট)। না চললে বাঁ পাশে **Build APK → Run workflow** চাপো।
4. সবুজ টিক এলে ওই run খুলে নিচে **Artifacts** থেকে `Arumatics-Study-Hub-apk` ডাউনলোড করো। ZIP খুললে `app-debug.apk` পাবে।
5. ফোনে APK ইনস্টল করো। "Unknown sources" বা "এই সোর্স থেকে ইনস্টল" অনুমতি চাইলে দিয়ে দাও।

## নোট
- প্রগ্রেস ফোনের ভেতরেই সেভ থাকে। অ্যাপ আনইনস্টল করলে মুছে যাবে।
- ডিকশনারি লুকআপের জন্য ইন্টারনেট লাগবে।
- আইকন এখন Capacitor-এর ডিফল্ট। চাইলে নিজের আইকন দিতে বলো।
- এটা debug APK, নিজের ফোনে ব্যবহারের জন্য ঠিক আছে। Play Store-এ দিতে হলে signed release বিল্ড লাগবে।
