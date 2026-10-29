# REPLOCK web app

## Run on iPhone
1. Host `index.html` and `manifest.webmanifest` on an HTTPS website. Camera access does not normally work from a local file URL.
2. Open the HTTPS URL in Safari and tap **Start camera**.
3. Allow camera access. Position the phone sideways so your shoulder, elbow, and wrist on one side are visible.
4. Configure challenge rules and optionally allow notifications.
5. Optional: Safari Share → Add to Home Screen.

## Included
- Mobile-first web UI
- MediaPipe Pose Landmarker body-pose detection
- Heuristic push-up counter (bent elbow then extended elbow)
- Adjustable rep goal, minutes per rep, reward cap, reminder interval
- Local browser storage for settings and reward balance
- Camera starts on user action and stops when the page is hidden

## Limitations
- This is a web prototype. It cannot lock the iPhone, replace the passcode screen, or restrict other apps.
- The page's hourly reminders may not run while Safari is suspended. Reliable background notifications need web push infrastructure and a hosted service worker.
- Pose detection is approximate and may miscount. Stop if you feel pain; don't treat it as medical advice.
- The pose library/model are downloaded at runtime; internet is required.
- No camera frames are uploaded by the included app code.
