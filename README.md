# boky-config
Signed feature switches for Boky (no user data).
# boky-config

مفاتيح ميزات تطبيق بوكي (Boky) لكل المستخدمين.

- الملف `features.json` تكتبه وتوقّعه **شاشة الماستر** داخل بوكي، ولا يُعدَّل يدوياً.
- كل نسخة من بوكي تقرؤه مرة في اليوم من:
  `https://raw.githubusercontent.com/Green-Issland-Livestock/boky-config/main/features.json`
- لا يُطبَّق إلا إن كان موقّعاً (Ed25519) بمفتاح مالك مُدرج في التطبيق،
  وأحدث مما طُبّق قبله. أي تعديل يدوي يكسر التوقيع فيُتجاهل.
- الملف يحدد إظهار الميزات وإخفاءها فقط؛ لا يحوي أسراراً ولا بيانات عملاء،
  ولا يُرسل التطبيق أي معلومة عند قراءته.

Feature switches for the Boky app. `features.json` is written and signed by
the in-app Master screen; apps apply it only if the Ed25519 signature matches
a trusted owner key compiled into the app. No secrets, no user data.
