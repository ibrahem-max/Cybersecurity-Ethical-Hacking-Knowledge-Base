# أساسيات الشبكات | Networking Foundations

## نموذج TCP/IP بصورة مبسطة
- **Link:** الإطارات وعناوين MAC والشبكة المحلية.
- **Internet:** عناوين IP والتوجيه.
- **Transport:** TCP وUDP والمنافذ.
- **Application:** DNS وHTTP وSMTP وSSH وغيرها.

## مفاهيم مهمة
- **IP address:** عنوان واجهة على شبكة.
- **Subnet/CIDR:** وصف نطاق عناوين، مثل `192.0.2.0/24` للأمثلة التوثيقية.
- **DNS:** تحويل الأسماء إلى سجلات مثل A/AAAA/CNAME/MX.
- **DHCP:** توزيع إعدادات الشبكة.
- **TCP handshake:** SYN، SYN-ACK، ACK؛ لا يعني نجاح الاتصال وحده أن التطبيق سليم.
- **TLS:** حماية سرية وسلامة الاتصال والتحقق من هوية الخادم وفق إعدادات الشهادة.
- **Firewall:** قواعد تسمح أو تمنع حركة وفق العناوين والمنافذ والحالة.

## أدوات تشخيص آمنة
- Windows: `ipconfig /all`, `nslookup example.com`, `tracert example.com`
- Linux: `ip addr`, `ip route`, `dig example.com`, `tracepath example.com`
- اختبار خدمة ضمن نظام تملكه: `curl -I https://example.com`
- لا تفحص شبكات الآخرين أو عناوين عامة دون إذن واضح.

## مختبر
أنشئ شبكتين افتراضيتين معزولتين، وثبّت خادم ويب تجريبيًا، وسجّل طلب HTTP ثم HTTPS، وقارن البيانات الظاهرة مع البيانات المشفرة. لا تستخدم بيانات دخول حقيقية في التجربة.

## مراجع
- Cloudflare Learning Center: https://www.cloudflare.com/learning/
- RFC Editor: https://www.rfc-editor.org/
- Wireshark User's Guide: https://www.wireshark.org/docs/
