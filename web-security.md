# أمن تطبيقات الويب | Web Application Security

## مجالات مراجعة شائعة
- **Broken Access Control:** تحقق من الصلاحية في جهة الخادم لكل مورد وإجراء.
- **Cryptographic Failures:** تجنب التخزين أو النقل غير الآمن للبيانات الحساسة.
- **Injection:** استخدم الاستعلامات المعلّمة/المحضّرة وافصل البيانات عن الأوامر.
- **Insecure Design:** عرّف نموذج التهديد ومتطلبات الأمان مبكرًا.
- **Security Misconfiguration:** عطّل الإعدادات الافتراضية غير اللازمة وأزل التفاصيل الحساسة من رسائل الخطأ.
- **Authentication Failures:** استخدم مصادقة متعددة العوامل، وحماية من التخمين، واستردادًا آمنًا للحساب.
- **Integrity Failures:** تحقق من مصدر التبعيات والبناء والتحديثات.
- **Logging and Monitoring Failures:** سجّل أحداثًا مفيدة دون تسجيل كلمات المرور أو الرموز السرية.
- **SSRF:** قيّد الخروج إلى الشبكة، واسمح بوجهات محددة، وتحقق من إعادة التوجيه وعناوين IP.
- **CSRF/XSS:** طبّق حماية CSRF المناسبة، وترميز المخرجات بحسب السياق، وسياسات CSP كطبقة إضافية.

## قائمة مراجعة للمطور
- تحقق من الهوية والصلاحية على الخادم، وليس في الواجهة فقط.
- استخدم HTTPS وملفات ارتباط `Secure`, `HttpOnly`, و`SameSite` بحسب الحاجة.
- ضع الأسرار في مدير أسرار ولا تضعها في المستودع.
- طبّق حدود المعدل والتحقق من المدخلات وقواعد أعمال واضحة.
- حدّث التبعيات وافحصها آليًا، وراجع نتائج الفحص يدويًا.
- أضف اختبارات وصول سلبية وإيجابية.
- استجب للأخطاء دون كشف stack traces أو معلومات داخلية.

## مختبرات مقصودة للتدريب
- OWASP Juice Shop: https://owasp.org/www-project-juice-shop/
- OWASP WebGoat: https://owasp.org/www-project-webgoat/
- PortSwigger Web Security Academy: https://portswigger.net/web-security

استخدم هذه البيئات وفق شروطها، ويفضّل تشغيلها محليًا أو في حساب تدريبي. لا تختبر مواقع إنتاجية دون تصريح مكتوب.

## المراجع
- OWASP Top 10: https://owasp.org/www-project-top-ten/
- OWASP ASVS: https://owasp.org/www-project-application-security-verification-standard/
- OWASP Cheat Sheet Series: https://cheatsheetseries.owasp.org/
