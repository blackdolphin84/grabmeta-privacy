---
title: GrabMeta privacy policy
---

# GrabMeta privacy policy

Last updated: 19 November 2026

Contact: 18@blackdolphin.io


This policy describes GrabMeta as it works in this repository. If you later add accounts, ads, analytics, or a server, update the policy and the Data safety form before shipping that build.

## English

GrabMeta is an Android app that saves a public video from Facebook, Instagram, YouTube, or X (Twitter) onto the phone and can hand that file to WhatsApp or another app. The developer does not operate a server for GrabMeta and does not have a GrabMeta user account.

### Data that leaves the phone

When you tap Download, or when you share a link into GrabMeta, the app sends that video URL over HTTPS to the site that hosts the video, so it can fetch the public file:

- Facebook pages on facebook.com
- Instagram pages and media endpoints on instagram.com and i.instagram.com
- YouTube pages on youtube.com, and the video addresses YouTube returns (typically on googlevideo.com). Extraction runs on the phone with the NewPipeExtractor library.
- X's public embed endpoint on cdn.syndication.twimg.com, and the video file on video.twimg.com. If that does not return a video, the app tries api.fxtwitter.com and then api.vxtwitter.com.

The request uses a generic Chrome user-agent string. It does not include your name, email, phone number, contacts, the Android advertising ID, or a precise location. Those services see your IP address, as they would for any connection your phone makes to them. Facebook and Instagram may set cookies (for example `csrftoken` or `datr`). GrabMeta keeps those cookies in memory only, for the life of the app process, and sends them back only to the same site. They are discarded when the process ends.

GrabMeta does not ask for, and does not store, your password for any of those services. Private, friends-only, login-only, and (on X) sensitive posts are not supported.

The developer does not receive the URL, the cookies, or the video. There is no GrabMeta account of the download.

### Data that stays on the phone

- The video file, and the title when the page provides one, is saved in your gallery at Movies/GrabMeta through Android's MediaStore. It stays there until you delete it. Sharing it is a separate action you take, through WhatsApp or the Android share sheet. GrabMeta does not upload the file.
- One setting is stored in app preferences: whether to open WhatsApp after a download. Android backup may include that preference if you have device backup turned on. It is not sent to the developer.
- While GrabMeta is in the foreground and the link box is empty, the app reads the clipboard to look for a supported link. Any other clipboard text is ignored. Clipboard contents are not stored and are not sent anywhere unless you then download that link.
- To decide whether to open WhatsApp or WhatsApp Business, the app checks whether those two packages are installed. The result stays on the phone.

GrabMeta does not include an advertising SDK, an analytics SDK, or a crash-reporting SDK.

### Permissions

- Internet, and permission to see whether the network is connected.
- On Android 8, 8.1, and 9 (API 26–28) only, storage write permission, so the video can be saved in the public Movies folder. Android 10 (API 29) and later use MediaStore and do not use this permission. The app does not request access to all files, and it does not request permission to read your photos or videos.
- The app is allowed to see WhatsApp, WhatsApp Business, and apps that can receive or play a video. It does not request permission to list every app on the device.

### Children

GrabMeta is not directed at children under 13, and it should not be placed in Google Play's Designed for Families program. Downloaded videos are whatever the public post contains. The app does not filter them.

### Retention and deletion

The developer has no account to delete and no server copy of your URL, cookies, or videos. Cookies are dropped when the app process ends. Delete a video from the gallery to remove the file. Uninstall GrabMeta to remove the on-device setting. You can email 18@blackdolphin.io if you have a question; there is no server-side record to erase.

### Sharing

The developer does not sell data. The URL is sent to the companies and services listed above only to fetch the video you asked for. Their own privacy policies cover what they do with that request.


<div dir="rtl" markdown="1">

## עברית

GrabMeta היא אפליקציית אנדרואיד ששומרת בטלפון סרטון ציבורי מפייסבוק, מאינסטגרם, מיוטיוב או מ-X (טוויטר), ויכולה להעביר את הקובץ לוואטסאפ או לאפליקציה אחרת. למפתח אין שרת של GrabMeta ואין חשבון משתמש של GrabMeta.

### מידע שיוצא מהטלפון

כשלוחצים על "הורד", או כשמשתפים לינק אל GrabMeta, האפליקציה שולחת את כתובת הסרטון ב-HTTPS לאתר שמארח את הסרטון, כדי להביא את הקובץ הציבורי:

- דפי פייסבוק ב-facebook.com
- דפי אינסטגרם ונקודות מדיה ב-instagram.com וב-i.instagram.com
- דפי יוטיוב ב-youtube.com, וכתובות הסרטון שיוטיוב מחזירה (בדרך כלל ב-googlevideo.com). החילוץ רץ בטלפון באמצעות הספרייה NewPipeExtractor.
- נקודת ההטמעה הציבורית של X ב-cdn.syndication.twimg.com, וקובץ הסרטון ב-video.twimg.com. אם זה לא מחזיר סרטון, האפליקציה מנסה את api.fxtwitter.com ואחר כך את api.vxtwitter.com.

הבקשה משתמשת במחרוזת User-Agent כללית של Chrome. היא לא כוללת שם, דוא"ל, מספר טלפון, אנשי קשר, מזהה פרסום של אנדרואיד או מיקום מדויק. השירותים האלה רואים את כתובת ה-IP, כמו בכל חיבור שהטלפון יוצר אליהם. פייסבוק ואינסטגרם עשויות להגדיר עוגיות (למשל `csrftoken` או `datr`). GrabMeta שומרת את העוגיות האלה בזיכרון בלבד, כל עוד תהליך האפליקציה רץ, ושולחת אותן בחזרה רק לאותו אתר. הן נמחקות כשהתהליך נגמר.

GrabMeta לא מבקשת ולא שומרת את הסיסמה שלך לאף אחד מהשירותים האלה. פוסטים פרטיים, לחברים בלבד, כאלה שדורשים התחברות, וב-X גם פוסטים שסומנו כרגישים, לא נתמכים.

המפתח לא מקבל את הכתובת, את העוגיות או את הסרטון. אין אצלו תיעוד של ההורדה.

### מידע שנשאר בטלפון

- קובץ הסרטון, והכותרת אם הדף סיפק אותה, נשמרים בגלריה ב-Movies/GrabMeta דרך MediaStore של אנדרואיד. הם נשארים שם עד שמוחקים אותם. שיתוף הוא פעולה נפרדת שלך, דרך וואטסאפ או גיליון השיתוף של אנדרואיד. GrabMeta לא מעלה את הקובץ.
- הגדרה אחת נשמרת בהעדפות האפליקציה: האם לפתוח את וואטסאפ אחרי הורדה. גיבוי של אנדרואיד עשוי לכלול את ההעדפה הזו אם גיבוי המכשיר פועל. היא לא נשלחת למפתח.
- כש-GrabMeta בחזית ותיבת הלינק ריקה, האפליקציה קוראת את לוח ההעתקה כדי לחפש לינק נתמך. כל טקסט אחר בלוח ההעתקה מתעלמים ממנו. תוכן הלוח לא נשמר ולא נשלח לשום מקום, אלא אם אחר כך מורידים את הלינק הזה.
- כדי להחליט אם לפתוח את וואטסאפ או את וואטסאפ ביזנס, האפליקציה בודקת אם שתי החבילות האלה מותקנות. התוצאה נשארת בטלפון.

ב-GrabMeta אין ערכת פרסום, אין ערכת ניתוח שימוש ואין ערכת דיווח על קריסות.

### הרשאות

- אינטרנט, והרשאה לראות אם יש חיבור לרשת.
- באנדרואיד 8, 8.1 ו-9 (API 26 עד 28) בלבד, הרשאת כתיבה לאחסון, כדי לשמור את הסרטון בתיקיית Movies הציבורית. מאנדרואיד 10 (API 29) ואילך נעשה שימוש ב-MediaStore וההרשאה הזו לא בשימוש. האפליקציה לא מבקשת גישה לכל הקבצים, ולא מבקשת הרשאה לקרוא תמונות או סרטונים.
- לאפליקציה מותר לראות את וואטסאפ, וואטסאפ ביזנס, ואפליקציות שיכולות לקבל או לנגן סרטון. היא לא מבקשת הרשאה לרשימת כל האפליקציות במכשיר.

### ילדים

GrabMeta לא מיועדת לילדים מתחת לגיל 13, ואין לרשום אותה לתוכנית Designed for Families של Google Play. הסרטונים שמורדים הם מה שיש בפוסט הציבורי. האפליקציה לא מסננת אותם.

### שמירה ומחיקה

למפתח אין חשבון למחוק ואין עותק בשרת של הכתובת, העוגיות או הסרטונים. העוגיות נמחקות כשתהליך האפליקציה נגמר. מוחקים סרטון מהגלריה כדי להסיר את הקובץ. מסירים את GrabMeta כדי להסיר את ההגדרה שבמכשיר. אפשר לכתוב אל 18@blackdolphin.io אם יש שאלה; אין רשומה בשרת שאפשר למחוק.

### שיתוף

המפתח לא מוכר מידע. הכתובת נשלחת לחברות ולשירותים שברשימה למעלה רק כדי להביא את הסרטון שביקשת. מדיניות הפרטיות שלהם מכסה את מה שהם עושים עם הבקשה.

</div>
