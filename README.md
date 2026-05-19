# Rudy
"Won't you be my Darling?" — Zero Two (002) Zero-Two is a minimalist, "headless" Android application inspired by the main heroine of DARLING in the FRANXX. Designed to be an invisible digital companion, the app allows users to interact with Zero Two’s voice and spirit directly from their home screen with a single tap.

.
🎧 The Experience
Unlike traditional applications, Zero-Two has no homepage or buttons.
When you click the app icon:
1.
The app launches invisibly using a Transparent Theme.
2.
It immediately selects one of 83 randomized audio clips (including her iconic "Darling" lines).
3.
The activity finishes instantly, returning you to your home screen while the audio plays in the background.
It is designed to feel like a spontaneous interaction rather than a tool—a quick whisper from your partner before she returns to the front lines.
🛠️ Technical Highlights
•
Strelizia Core: The app logic is housed in StreliziaActivity, named after the powerful FRANXX piloted by Zero Two and Hiro.
•
Headless Architecture: Utilizes an Activity with android:theme="@style/Theme.Transparent" that executes its logic in onCreate and calls finish() immediately.
•
Dynamic Resource Engine: Uses a randomized resource identification system to pull from an expandable library of 83+ high-quality .mp3 files.
•
Background Persistence: Leverages applicationContext within the MediaPlayer to ensure the audio finishes playing even after the activity has been destroyed.
•
Easter Egg: Every initialization sends a hidden handshake to the system log:
Log.d("Strelizia", "Partner found. Initializing Strelizia...")
🚀 Installation & Setup
1.
Clone the Project:
Shell Script
git clone https://github.com/[Your-Username]/Zero-Two.git
2.
Add Your Audio: Drop your .mp3 files into app/src/main/res/raw/.
3.
Customize the List: Update the audioFileNames list in StreliziaActivity.kt to match your file names.
4.
Build: Open in Android Studio and click Build APK.
📖 Inspiration
This project is a tribute to Zero Two (002), the human-klaxo sapien hybrid and elite Parasite. Once a solitary fighter known as the "Partner Killer," she found her purpose in her "Darling," Hiro. This app aims to capture her vibrant, unpredictable, and affectionate personality in a simple digital form.
Created with ❤️ by Rudy.
