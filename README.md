# أدلة SonarQube

مجلدان HTML يُنشران معًا. كل دليل يفتح الآخر بالاسم، لذلك تبقى الملفات الثلاثة في جذر المستودع.

| الملف | الصفحة |
|---|---|
| `index.html` | صفحة البداية |
| `SonarQube_Guide_AR_v2.html` | الدليل الشامل: الشاشات والأرقام |
| `SonarQube_Playbook_AR_v2.html` | دليل التطبيق على أي مشروع |

## النشر على GitHub Pages

1. أنشئ مستودعًا عامًا جديدًا على GitHub باسم `sonar-guides`. لا تضف README من الموقع.
2. افتح PowerShell في هذا المجلد.
3. ابدأ Git وارفع الملفات الثلاثة:

```powershell
git init
git add index.html SonarQube_Guide_AR_v2.html SonarQube_Playbook_AR_v2.html README.md
git commit -m "Publish the SonarQube guides"
git branch -M main
git remote add origin https://github.com/YOUR-USER/sonar-guides.git
git push -u origin main
```

4. في المستودع افتح Settings ثم Pages.
5. تحت Build and deployment اختر Deploy from a branch.
6. اختر الفرع `main` والمجلد `/ (root)` ثم Save.
7. انتظر دقيقة أو اثنتين، ثم افتح `https://YOUR-USER.github.io/sonar-guides/`.

استبدل `YOUR-USER` باسم حسابك على GitHub. المستودع العام مطلوب حتى تعمل GitHub Pages على الخطة المجانية.
