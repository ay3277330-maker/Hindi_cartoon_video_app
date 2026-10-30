# मोबाइल से APK बनाने का तरीका (IADO AI)

यह प्रोजेक्ट अभी सोर्स कोड है; APK इस ZIP के अंदर पहले से नहीं है। इस प्रोजेक्ट में GitHub Actions workflow जोड़ा गया है, जो GitHub पर कोड डालने के बाद Android debug APK बना सकता है।

## जरूरी बातें
- GitHub अकाउंट चाहिए। GitHub की शर्तों के अनुसार अकाउंट इस्तेमाल करें; नाबालिग हों तो अभिभावक की मदद लें।
- यह तरीका ऑनलाइन बिल्ड करता है; मोबाइल पर Android Studio इंस्टॉल करने की जरूरत नहीं।
- APK अभी शुरुआती ऐप है। इसमें फोटो पिकर/प्रीव्यू और डेमो UI है; पूरा वीडियो एडिटर, AI जनरेशन और असली HD एक्सपोर्ट अभी नहीं हैं।

## बिल्ड कैसे होगा
1. GitHub पर नया खाली repository बनाएँ।
2. इस ZIP को पहले फोन में Extract करें।
3. प्रोजेक्ट की सभी फाइलें और `.github/workflows/build-apk.yml` सहित GitHub repository में अपलोड करें।
4. GitHub repository में **Actions** टैब खोलें।
5. **Build IADO AI APK** चुनें और **Run workflow** दबाएँ।
6. बिल्ड सफल होने पर workflow run के नीचे **Artifacts** में `IADO-AI-debug-apk` डाउनलोड करें।
7. ZIP artifact खोलें; उसके अंदर `app-debug.apk` होगा। Android सुरक्षा पूछे तो केवल अपने भरोसेमंद स्रोत से बनी APK इंस्टॉल करें।

यह debug APK परीक्षण के लिए है, Play Store पर प्रकाशित करने वाली signed release फाइल नहीं।
