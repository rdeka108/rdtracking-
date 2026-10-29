# FieldTrace APK kaise banayein (bina code ke)

Yeh folder FieldTrace ka Android app hai. APK file GitHub apne computer par free mein bana dega. Aapko code nahi likhna hai — sirf files upload karni hain.

Samay: lagbhag 15 minute (pehli baar).

---

## Step 1 — GitHub account banayein

1. Computer par https://github.com/signup kholein.
2. Email, password, username daal kar free account banayein.

## Step 2 — Naya repository (folder) banayein

1. Login ke baad https://github.com/new kholein.
2. **Repository name:** `fieldtrace-android`
3. **Private** chunein.
4. Neeche **"Add a README file"** ko tick NA karein.
5. **Create repository** dabayein.

## Step 3 — Files upload karein

1. Jo ZIP file aapko mili hai (`FieldTrace-Android.zip`), use computer par **Extract / Unzip** karein.
2. Naye repository page par link **"uploading an existing file"** par click karein.
3. Unzip kiye hue folder ke **andar ki sab files aur folders** select karke browser mein drag-and-drop karein.
   - Dhyan dein: `.github` naam ka folder bhi upload hona chahiye. Windows mein agar dikh nahi raha, to File Explorer mein **View → Hidden items** tick karein.
4. Neeche **Commit changes** dabayein.

## Step 4 — APK banne dein

1. Repository page par upar **Actions** tab kholein.
2. Agar poochhe to **"I understand my workflows, go ahead and enable them"** dabayein.
3. Left side **Build FieldTrace APK** → right side **Run workflow** → hara **Run workflow** button.
4. 5–10 minute wait karein. Hara ✔ aane par build poora.

## Step 5 — APK download karein

1. Hare ✔ wale build par click karein.
2. Neeche **Artifacts** mein **FieldTrace-APK** par click karein — ZIP download hoga.
3. Use unzip karein — andar `app-debug.apk` hai. Yahi aapka app hai.

## Step 6 — Phone par install karein

1. `app-debug.apk` ko phone par bhejein (WhatsApp, USB cable ya Google Drive se).
2. Phone par file kholein. "Install unknown apps" ki permission maange to **Allow** karein.
3. **Install** dabayein.
4. App kholein → login karein (jaise ravi@demo.app / demo1234).
5. Privacy notice par **Agree** karein. Location poochhe to **"Allow all the time"** chunein, notification poochhe to **Allow**.

Tracking chalu hone par notification bar mein "FieldTrace is sharing your location" dikhega — iska matlab background tracking chal rahi hai.

---

## Agar build red ❌ ho jaaye

Red build par click karein, error ka screenshot lekar mujhe bhej dein — main theek kar dunga.

## Zaroori baatein (sach-sach)

- **Background tracking:** app band (minimize) hone par bhi har ~30 minute location jayegi, notification ke saath. Lekin agar employee app ko recent-apps se swipe karke hata de, phone band kar de, ya battery saver app ko rok de — tab updates ruk jayenge. Xiaomi, Oppo, Vivo, Realme phones mein **Settings → Battery → FieldTrace → "No restrictions"** karna padega.
- **Pehle phone par test karein:** maine yeh app asli phone par test nahi kiya hai (yahan Android phone nahi hai). 1–2 din ek phone par chala kar dekhein ki location har 30 minute aa rahi hai ya nahi.
- **Yeh "debug" APK hai:** apni team ko seedha de sakte hain. Google Play Store par daalne ke liye "release" version aur Google Play Developer account ($25, ek baar) chahiye — jab chahein, main woh step bhi bata dunga.
- **iPhone:** iPhone app ke liye Mac computer aur Apple Developer account ($99/saal) chahiye. Tab tak iPhone wale browser se app chala sakte hain.
- **App ka address:** app abhi `https://preview--beacon-fieldtrace-base.apper.so` kholta hai. Agar Apper mein app ka address badle, to `capacitor.config.json` mein `url` badal kar files dobara upload karein — naya APK ban jayega.
