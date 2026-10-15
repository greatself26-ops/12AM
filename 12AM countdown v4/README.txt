12 AM COUNTDOWN - FINAL VERSION
===============================

WHAT'S INSIDE
  website/                      The site (deploy this folder to Netlify)
  ios-lockscreen-widget/        iPhone lock-screen widget script (for the Scriptable app)

1) DEPLOY ON NETLIFY
  - Unzip this file.
  - Go to https://app.netlify.com/drop and log in.
  - Drag the "website" folder (not the zip) onto the page.
  - Open your Netlify link.
  To update later: drag the updated "website" folder onto your site's Deploys tab.

2) YOUR SETTINGS (website/index.html, around line 481)
  MEET_LINK, WHATSAPP_NUMBER and PASSCODE are filled in. Edit, save, redeploy.
  The passcode is visible to anyone who views the page source.

3) SUPERNOVA
  Plays once a day when the countdown reaches 48 seconds (11:59:12 PM local time).
  To preview it any time, add #supernova to the end of your link and open it
  (example: https://your-site.netlify.app/#supernova).
  To change the moment, edit NOVA_AT = 48 in index.html.

4) INSTALL AS AN APP (use the live https link, not a file on your computer)
  - The INSTALL button (top right) is always shown. On Chrome/Edge/Android it opens the
    install prompt; if the browser doesn't offer one, it shows what to tap instead.
  - iPhone (Safari): Share > Add to Home Screen.
  After redeploying, open the installed app twice to see the update.

5) IPHONE LOCK-SCREEN WIDGET (iOS 16+)
  - Install the free "Scriptable" app, tap +, paste ios-lockscreen-widget.js.
  - Change SITE_URL to your Netlify link.
  - Lock screen: long-press > Customize > Lock Screen > Add Widgets > Scriptable.
  Shows a live H:MM:SS countdown (iOS widgets can't tick a 5-digit number).

6) ANDROID LOCK-SCREEN WIDGET
  Needs a native Android widget (not included).
