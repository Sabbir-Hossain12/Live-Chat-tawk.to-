# 💬 Tawk.to Integration Guide (Laravel)

## 📘 Overview
[Tawk.to](https://www.tawk.to) is a **free live chat and customer messaging platform** that helps you monitor and chat with visitors on your website.  
It offers:
- Real-time chat widget  
- Offline messaging (tickets)  
- REST API access (read-only)  
- Agent and visitor analytics  

You can integrate Tawk.to into your Laravel application for both:
- **Front-end live chat widget**
- **Back-end chat data fetching via API**

---

## 🧩 1. Widget Integration

### ✅ Step 1: Copy and Paste the Script
Place this snippet **before the closing `</body>` tag** in your main Blade layout file  
(e.g. `resources/views/layouts/app.blade.php`):

```html
<!--Start of Tawk.to Script-->
<script type="text/javascript">
    var Tawk_API = Tawk_API || {}, Tawk_LoadStart = new Date();
    (function(){
        var s1 = document.createElement("script"),
            s0 = document.getElementsByTagName("script")[0];
        s1.async = true;
        s1.src = 'https://embed.tawk.to/690ae700727def194d09d2ab/1j999cn29';
        s1.charset = 'UTF-8';
        s1.setAttribute('crossorigin', '*');
        s0.parentNode.insertBefore(s1, s0);
    })();
</script>
<!--End of Tawk.to Script-->

