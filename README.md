# NOVA: hands-free voice assistant (Android)

Neela JARVIS jaisa HUD, "Hey Nova" bolkar phone chalaiye: apps kholna, call, WhatsApp call/message, torch, volume, music, alarm, scroll, back/home aur bahut kuch.

## APK kaise banayein (Android Studio ke bina, sirf phone/browser se)

1. github.com par free account banayein, naya repository banayein (naam: `nova`).
2. Is zip ke andar ke saare files repository mein upload karein (Add file > Upload files). `.github` folder bhi upload hona chahiye.
3. Repository mein **Actions** tab kholein > **Build Nova APK** > **Run workflow**.
4. 3-5 minute baad run complete hoga. Us run ko kholein, neeche **Artifacts** mein **Nova-APK** download karein, zip kholein, `app-debug.apk` install karein.
   (Install karte waqt "Unknown sources / Install unknown apps" allow karna padega.)

Agar build fail ho to run ka error text mujhe bhej dein, main theek kar dunga.

## Android Studio se banana ho to

Android Studio (Koala ya naya) mein **Open** > is folder ko chuniye > Gradle sync > **Run**.

## Pehli baar setup (app khulne ke baad)

Neeche ke buttons ek ek karke dabayein, jab tick (✓) aa jaye to wo ho gaya:

| Button | Kyun zaroori hai |
|---|---|
| PERMS | Mic, contacts, call, notification ki permission |
| OVERLAY | "Display over other apps". Iske bina background se apps khulna block ho sakta hai |
| ACCESS | Accessibility ON karein. Back, home, scroll, tap, screenshot, WhatsApp message "Send" ke liye. Android 13+ par pehle App info > ⋮ > **Allow restricted settings** karna padta hai |
| BATTERY | Battery optimization band, taki Nova background mein band na ho |

Phir **START NOVA** dabayein. Notification mein "Nova sun raha hai" dikhega. Ab phone lock hone par bhi (jab tak Android ne service band na ki ho) "Hey Nova ..." bol sakte hain.

## Kaise bolein

Pehle "Hey Nova" (ya sirf "Nova"), phir command. Sirf "Hey Nova" bolenge to wo "Ji, boliye" bolegi aur agla vakya seedha command maanegi.

- WhatsApp kholo, Instagram kholo
- Saloni ko call karo / Saloni ko WhatsApp call karo
- Saloni ko message bhejo ki main late hoon (ya sirf "message bhejo", phir wo poochhegi kya likhna hai)
- Torch on / off, volume badhao / kam karo / mute
- Gaana chalao, pause, agla gaana
- YouTube par arijit singh chalao
- Rasta batao Connaught Place
- Alarm lagao subah 6 baje, 10 minute ka timer
- Battery kitni hai, time kya hai, aaj ki date
- Back, home, recent apps, notification, screenshot, screen lock
- Neeche scroll karo, agli reel
- Click Send (screen par dikh rahe button ka naam bolkar)
- Call utha lo, call kaat do
- Nova so jao (assistant band)

App mein **LANG** se Hindi ya English recognition chun sakte hain (Hinglish ke liye Hindi theek rehta hai).

## Seemayein (sach)

- Wi-Fi, Bluetooth, flight mode Android khud se on/off nahi karne deta. Nova unka panel/settings khol deti hai, ek tap aapko karna padega.
- Recognition Google ki speech service se hoti hai (internet chahiye). Kuch phones par har sunne se pehle halki beep aa sakti hai.
- WhatsApp message/call WhatsApp ke andar ke buttons dabakar chalte hain, WhatsApp update hone par kabhi kabhi button ka naam badal sakta hai.
- Naam bolte waqt contact mein jo naam saved hai wahi (ya milta-julta) bolna behtar rehta hai.
- Ye personal use ke liye bana hai (debug APK), Play Store ke liye nahi.
