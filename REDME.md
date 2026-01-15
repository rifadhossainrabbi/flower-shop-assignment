 /*tar mane ami jokhon desktop er jonno kono width dei ta mobile er jonno responsive korte ashle hoy right noy left side a faka thake tai to r ei somossa somadhan er jonno oi width ta 100% kore dite hoy tai to হ্যাঁ ✅ তুমি ঠিকই ধরছো,
      আর আমি এটাকে একটু আরও পরিষ্কার ও rule আকারে বুঝিয়ে দিচ্ছি। ✅ তোমার কথার সঠিক ব্যাখ্যা Desktop-এর জন্য width / max-width দিলে Mobile-এ গেলে ডান বা বাম পাশে ফাঁকা জায়গা দেখা যায় তাই mobile media query-তে width / max-width → 100% করতে হয় 👉 এটা 90% ক্ষেত্রেই ঠিক কথা। 🔍 কেন এমন হয়? Desktop example: .hero_container {
        max-width: 80%;
        margin: 0 auto;
      }
    
    
      Desktop screen=বড় 80%=সুন্দর লাগে Mobile screen: Screen ≈ 360px 80% ≈ 288px 👉 দুই পাশে 36px+36px ফাঁকা জায়গা ➡️ visually মনে হয় left/right ফাঁকা ✅ তাই mobile-এ আমরা করি: @media (max-width: 576px) {
        .hero_container {
          max-width: 100%;
        }
      }
    
    
      🔹 এখন container পুরো screen জুড়ে 🔹 আর side gap নাই ❗ একটা গুরুত্বপূর্ণ correction (খুব দরকার) তুমি বলছো: “right noy left side a faka thake” 👉 আসলে দুই পাশেই থাকে কিন্তু: content যদি center হয় → right বেশি চোখে পড়ে image থাকলে → imbalance লাগে 🧠 Golden Rule (মনে রাখবে) 🟢 Desktop: width / max-width → limited (60%, 70%, 80%, px) 📱 Mobile: width / max-width → 100% ❌ কখন 100% দিতে হবে না? সবসময় না ❌ Example: .button {
        width: 200px;
      }
    
    
      📱 Mobile-এ button full width করলে খারাপ লাগতে পারে তখন: width: auto;
    
      ✅ Responsive করার সময় checklist ✔ Desktop width দেওয়া আছে? ✔ Mobile-এ সেটা reset করা হয়েছে? ✔ padding দিয়েই spacing রাখা হয়েছে? 🔥 এক লাইনে Final Truth Desktop layout এ width কম রাখো,
      Mobile layout এ width খুলে দাও (100%)*/