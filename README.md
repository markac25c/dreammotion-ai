DreamMotion AI — Full Starter Project (PWA + API scaffold)

क्या शामिल है:
- Mobile-friendly app interface
- Image-to-video और Text-to-video mode selection
- Prompt, style, duration, aspect ratio controls
- Image preview
- My Videos / Account UI
- PWA manifest + service worker (installable web-app foundation)
- Node.js API scaffold for generation jobs

महत्वपूर्ण:
यह अभी production-ready या पूर्ण AI generator नहीं है। असली वीडियो बनाने के लिए server/api.js में किसी video-generation provider की API integration करनी होगी। अलग-अलग providers के free limits/charges होते हैं; unlimited free generation की गारंटी नहीं है।
Login और video history अभी demo/local UI हैं; production use से पहले secure authentication और database/storage जोड़ें।
किसी भी provider की API key को public HTML/JavaScript में न रखें।

मोबाइल पर preview:
1. ZIP extract करें।
2. public/index.html को HTML preview app में खोलें या static hosting पर deploy करें।
3. PWA install और service worker के लिए HTTPS hosting चाहिए।
4. Backend चलाने के लिए Node.js hosting/computer environment चाहिए; सिर्फ फोन पर local HTML खोलने से backend नहीं चलेगा।

API scaffold:
- server/api.js: demo endpoints; असली provider call जोड़ने की जगह स्पष्ट रूप से चिह्नित है।
- server/package.json: dependencies/commands.
