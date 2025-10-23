<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اینفوگرافیک مجموعه پرنیا</title>
    <!-- Tailwind CSS CDN for utility classes -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    <!-- Google Fonts for Vazirmatn font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    <style>
        /* Base styles for the body, setting font and background color */
        body {
            font-family: 'Vazirmatn', sans-serif;
            background-color: #f0f4f8; /* Very light gray/blue background */
        }
        /* Custom brand colors for text and background */
        .brand-text-primary { color: #004F71; } /* Deep Blue */
        .brand-text-secondary { color: #007B82; } /* Teal */
        .brand-accent-orange { color: #F5A623; } /* Gold/Orange */
        .brand-accent-green { color: #00A68D; } /* Vibrant Greenish Teal */
        /* Ensures right-to-left direction for grid layouts */
        .rtl-grid {
            direction: rtl;
        }
        /* Hover effect for Collection Cards */
        .collection-card {
            transition: all 0.3s ease-in-out;
            cursor: default; /* Changed cursor to default as the interaction is now a button */
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .collection-card:hover {
            transform: none; /* Removed translate effect for better focus on button */
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            border-bottom-width: 6px; 
        }
        .collection-card .gemini-btn:hover {
            transform: scale(1.05);
            background-color: #007B82;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- Modal for displaying Gemini output -->
    <div id="geminiModal" class="hidden fixed inset-0 bg-black bg-opacity-50 z-50 flex items-center justify-center p-4">
        <div class="bg-white rounded-xl p-8 max-w-lg w-full shadow-2xl relative">
            <h3 id="modalTitle" class="text-2xl font-bold brand-text-primary mb-4 border-b pb-2"></h3>
            <p id="modalContent" class="text-gray-700 text-lg leading-loose min-h-[50px]">...</p>
            <div id="modalLoading" class="hidden absolute inset-0 bg-white bg-opacity-80 flex items-center justify-center rounded-xl">
                <i class="fas fa-spinner fa-spin text-4xl brand-accent-orange"></i>
                <span class="mr-3 text-lg brand-text-primary">در حال تولید معرفی هوشمند...</span>
            </div>
            <button onclick="document.getElementById('geminiModal').classList.add('hidden')" class="absolute top-3 left-3 text-gray-500 hover:text-gray-900 transition-colors">
                <i class="fas fa-times text-2xl"></i>
            </button>
        </div>
    </div>
    
    <!-- Main container for the infographic content -->
    <div class="container mx-auto p-4 md:p-12 max-w-7xl">

        <!-- Header section of the infographic -->
        <header class="text-center mb-16 pt-4 border-b-2 border-gray-200 pb-6">
            <h1 class="text-5xl md:text-7xl font-black brand-text-primary mb-3 tracking-wide">مجموعه پرنیا</h1>
            <p class="text-xl md:text-2xl brand-text-secondary font-light">پیشرو و نوآور در صنعت طلا و خالق آثار فاخر ،کلکسیونی</p>
        </header>

        <!-- Main content grid -->
        <main class="grid grid-cols-1 md:grid-cols-2 gap-10 md:gap-16 rtl-grid">

            <!-- Section: Years of Experience and Innovation (Featured Block) -->
            <div class="md:col-span-2 bg-white rounded-3xl shadow-2xl p-8 md:p-12 flex flex-col md:flex-row items-center justify-around text-center border-t-8 border-teal-600">
                <div class="mb-6 md:mb-0">
                    <p class="text-2xl font-bold brand-text-primary mb-[-1rem]">بیش از</p>
                    <p class="text-9xl font-extrabold brand-accent-orange leading-none">۴۰</p>
                    <p class="text-3xl font-bold brand-text-primary mt-3">سال تجربه</p>
                    <p class="text-xl text-gray-600 mt-2">در سنت اصیل ظریف‌سازی طلا</p>
                </div>
                <!-- Visual separator -->
                <div class="border-t-2 md:border-t-0 md:border-r-2 border-gray-300 w-full md:w-auto md:h-40 mx-8 my-6 opacity-70"></div>
                <!-- Innovation Text -->
                <div class="md:w-1/2">
                    <p class="text-4xl font-extrabold brand-text-primary mb-4">تولیدات تخصصی</p>
                    <p class="text-xl text-gray-700 font-medium leading-loose">تولید تمبر،مدالیون،تابلو،شمش،از جنس طلا و نقره، با بهره‌گیری از تکنولوژی‌های روز دنیا و حفظ اصالت هنری</p>
                </div>
            </div>

            <!-- Section: Licenses and Permissions -->
            <div class="bg-white rounded-2xl shadow-xl p-6 md:p-8 border-t-4 border-blue-600">
                <h2 class="text-3xl font-bold brand-text-primary mb-6 text-center border-b pb-3 border-gray-100">لایسنس‌ها و مجوزها</h2>
                <div class="space-y-4 text-xl">
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg font-medium">
                        <span class="text-2xl ml-4 brand-accent-green">✅</span>
                        <span>دارای گواهینامه <span class="font-extrabold">ISO 9001</span> در مدیریت کیفیت</span>
                    </div>
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg font-medium">
                        <span class="text-2xl ml-4 brand-accent-green">🏅</span>
                        <span>عضو رسمی <span class="font-extrabold">انجمن طلا و جواهر ایران</span></span>
                    </div>
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg font-medium">
                        <span class="text-2xl ml-4 brand-accent-green">📜</span>
                        <span>پروانه میراث فرهنگی و صنایع دستی</span>
                    </div>
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg font-medium">
                        <span class="text-2xl ml-4 brand-accent-green">👍</span>
                        <span>دارای استاندارد تولید طلای ۲۴ عیار با شماره <span class="font-extrabold">T99</span></span>
                    </div>
                     <div class="flex items-center p-3 bg-teal-50 rounded-lg font-medium">
                        <span class="text-2xl ml-4 brand-accent-green">🏛️</span>
                        <span>عضویت کمیته بین‌المللی موزها <span class="font-extrabold">icom</span></span>
                    </div>
                </div>
            </div>

            <!-- Section: Learn More (External Links) -->
            <div class="bg-white rounded-2xl shadow-xl p-6 md:p-8 border-t-4 border-blue-600">
                <h2 class="text-3xl font-bold brand-text-primary mb-6 text-center border-b pb-3 border-gray-100">آشنایی بیشتر</h2>
                <div class="text-center space-y-4 w-full">
                    <p class="text-lg text-gray-700 mb-6">برای مشاهده کاتالوگ‌ها و وب‌سایت‌های مجموعه، از لینک‌های زیر بازدید فرمایید.</p>
                    
                    <a href="https://www.shemshetala.com/Content/UploadFiles/PARNIA_Co-Collection.pdf" target="_blank" class="block w-full text-center bg-teal-600 text-white font-bold py-3 px-6 rounded-xl hover:bg-teal-700 transition-colors shadow-md">
                        کاتالوگ مجموعه محصولات
                    </a>
                    <a href="https://www.shemshetala.com/Content/UploadFiles/PARNIA_Co_Shemsh.pdf" target="_blank" class="block w-full text-center bg-teal-600 text-white font-bold py-3 px-6 rounded-xl hover:bg-teal-700 transition-colors shadow-md">
                        کاتالوگ شمش پرنیا
                    </a>
                    <!-- Changed link styling to secondary button style -->
                    <a href="https://gssmuseum.com/about/" target="_blank" class="block w-full text-center bg-gray-200 text-gray-800 font-bold py-3 px-6 rounded-xl hover:bg-gray-300 transition-colors">
                        وب‌سایت موزه تمبرهای طلا و نقره ایران
                    </a>
                    <a href="https://gssmuseum.com/about/" target="_blank" class="block w-full text-center bg-gray-200 text-gray-800 font-bold py-3 px-6 rounded-xl hover:bg-gray-300 transition-colors">
                        وب‌سایت خانه سکه ایران
                    </a>
                    <a href="https://www.niyaco.com" target="_blank" class="block w-full text-center bg-gray-200 text-gray-800 font-bold py-3 px-6 rounded-xl hover:bg-gray-300 transition-colors">
                        وب‌سایت صنایع دستی پرنیا
                    </a>
                </div>
            </div>
            
            <!-- Section: The Parnia Collection (Modern & Minimalist Layout) -->
            <div class="md:col-span-2 bg-white rounded-3xl shadow-2xl p-8 md:p-12">
                <h2 class="text-4xl font-extrabold brand-text-primary mb-10 text-center">بخش‌های اصلی مجموعه پرنیا</h2>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                    
                    <!-- Card 1: صنایع دستی پرنیا -->
                    <div class="collection-card bg-white p-6 rounded-xl text-center shadow-lg border-b-4 border-teal-600">
                        <i class="fas fa-gem text-6xl brand-accent-green mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold brand-text-primary mb-2">صنایع دستی پرنیا</h3>
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-4">پیوند هنر و صنعت در تولید آثار نفیس طلا و نقره</p>
                        <button onclick="generateSectionIntroduction('صنایع دستی پرنیا', 'پیوند هنر و صنعت در تولید آثار نفیس طلا و نقره')" class="gemini-btn bg-teal-600 text-white font-bold py-2 px-4 rounded-lg transition-all shadow-md">
                            ✨ معرفی هوشمند
                        </button>
                    </div>

                    <!-- Card 2: کارخانه و کارگاه تولید طلا -->
                    <div class="collection-card bg-white p-6 rounded-xl text-center shadow-lg border-b-4 border-orange-500">
                        <i class="fas fa-industry text-6xl brand-accent-orange mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold brand-text-primary mb-2">کارخانه و کارگاه تولید طلا</h3>
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-4">تولیدات با کیفیت و مطابق با استانداردهای روز</p>
                        <button onclick="generateSectionIntroduction('کارخانه و کارگاه تولید طلا', 'تولیدات با کیفیت و مطابق با استانداردهای روز')" class="gemini-btn bg-teal-600 text-white font-bold py-2 px-4 rounded-lg transition-all shadow-md">
                            ✨ معرفی هوشمند
                        </button>
                    </div>

                    <!-- Card 3: انتشارات پرنیا -->
                    <div class="collection-card bg-white p-6 rounded-xl text-center shadow-lg border-b-4 border-orange-500">
                        <i class="fas fa-book-open text-6xl brand-accent-orange mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold brand-text-primary mb-2">انتشارات پرنیا</h3>
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-4">ترویج فرهنگ و تاریخ و مشاهیر ایران جهان در قالب نشر کتب فاخر</p>
                        <button onclick="generateSectionIntroduction('انتشارات پرنیا', 'ترویج فرهنگ و تاریخ و مشاهیر ایران جهان در قالب نشر کتب فاخر')" class="gemini-btn bg-teal-600 text-white font-bold py-2 px-4 rounded-lg transition-all shadow-md">
                            ✨ معرفی هوشمند
                        </button>
                    </div>

                    <!-- Card 4: خانه سکه ایران -->
                    <div class="collection-card bg-white p-6 rounded-xl text-center shadow-lg border-b-4 border-orange-500">
                        <i class="fas fa-coins text-6xl brand-accent-orange mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold brand-text-primary mb-2">خانه سکه ایران</h3>
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-4">مرجع خرید شمش‌ها و آثار هنری تولید شده از جنس طلا و نقره</p>
                        <button onclick="generateSectionIntroduction('خانه سکه ایران', 'مرجع خرید شمش‌ها و آثار هنری تولید شده از جنس طلا و نقره')" class="gemini-btn bg-teal-600 text-white font-bold py-2 px-4 rounded-lg transition-all shadow-md">
                            ✨ معرفی هوشمند
                        </button>
                    </div>

                    <!-- Card 5: بنکداری طلا در بازار -->
                    <div class="collection-card bg-white p-6 rounded-xl text-center shadow-lg border-b-4 border-orange-500">
                        <i class="fas fa-building text-6xl brand-accent-orange mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold brand-text-primary mb-2">بنکداری طلا در بازار</h3>
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-4">فعالیت در بازار طلا و ارائه خدمات عمده‌فروشی</p>
                        <button onclick="generateSectionIntroduction('بنکداری طلا در بازار', 'فعالیت در بازار طلا و ارائه خدمات عمده‌فروشی')" class="gemini-btn bg-teal-600 text-white font-bold py-2 px-4 rounded-lg transition-all shadow-md">
                            ✨ معرفی هوشمند
                        </button>
                    </div>
                    
                    <!-- Card 6: موزه تمبرهای طلا و نقره ایران -->
                    <div class="collection-card bg-white p-6 rounded-xl text-center shadow-lg border-b-4 border-orange-500">
                        <i class="fas fa-university text-6xl brand-accent-orange mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold brand-text-primary mb-2">موزه تمبرهای طلا و نقره ایران</h3>
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-4">نمایشگاه دائمی آثار ارزشمند و کلکسیونی</p>
                        <button onclick="generateSectionIntroduction('موزه تمبرهای طلا و نقره ایران', 'نمایشگاه دائمی آثار ارزشمند و کلکسیونی')" class="gemini-btn bg-teal-600 text-white font-bold py-2 px-4 rounded-lg transition-all shadow-md">
                            ✨ معرفی هوشمند
                        </button>
                    </div>
                </div>
            </div>
            
        </main>

        <!-- Footer section -->
        <footer class="text-center mt-16 py-6 border-t border-gray-300">
            <p class="text-gray-600">&copy; ۱۴۰۴ - مجموعه پرنیا. کلیه حقوق محفوظ است.</p>
        </footer>

    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, signInWithCustomToken } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        // Global Firebase variables setup
        const firebaseConfig = typeof __firebase_config !== 'undefined' ? JSON.parse(__firebase_config) : {};
        const initialAuthToken = typeof __initial_auth_token !== 'undefined' ? __initial_auth_token : null;
        
        let app, db, auth;

        // --- Firebase Initialization and Auth ---
        window.onload = async () => {
            try {
                if (Object.keys(firebaseConfig).length) {
                    app = initializeApp(firebaseConfig);
                    auth = getAuth(app);
                    db = getFirestore(app);

                    if (initialAuthToken) {
                        await signInWithCustomToken(auth, initialAuthToken);
                        console.log("Firebase signed in with custom token.");
                    } else {
                        await signInAnonymously(auth);
                        console.log("Firebase signed in anonymously.");
                    }
                } else {
                    console.error("Firebase config not available. Running without Firebase.");
                }
            } catch (error) {
                console.error("Firebase initialization or sign-in failed:", error);
            }
        };

        /**
         * Shows the modal with content and manages loading state.
         * @param {string} title - The title of the section.
         * @param {string} content - The content to display.
         * @param {boolean} isLoading - Whether the loading spinner should be visible.
         */
        function showModal(title, content, isLoading) {
            const modal = document.getElementById('geminiModal');
            document.getElementById('modalTitle').textContent = title;
            document.getElementById('modalContent').textContent = content;
            document.getElementById('modalLoading').classList.toggle('hidden', !isLoading);
            modal.classList.remove('hidden');
        }

        /**
         * Calls the Gemini API to generate a professional introduction for a section.
         * Uses exponential backoff for retries.
         * @param {string} sectionName - The name of the section (e.g., 'صنایع دستی پرنیا').
         * @param {string} sectionDescription - The static description of the section.
         */
        window.generateSectionIntroduction = async (sectionName, sectionDescription) => {
            const userQuery = `عنوان بخش: ${sectionName}. وظیفه اصلی: ${sectionDescription}. بر اساس این اطلاعات، یک معرفی بسیار کوتاه (حداکثر دو جمله و لحن فاخر) برای این بخش بنویسید که جذابیت آن را برای مشتریان کلکسیونی یا سرمایه‌گذاران نشان دهد.`;
            const systemPrompt = "شما یک کارشناس خبره در زمینه طلا، صنایع دستی فاخر، و مجموعه داری هستید. لحن شما باید بسیار حرفه‌ای، فاخر، و گیرا باشد. پاسخ شما باید فقط شامل متن معرفی بدون هیچ مقدمه یا عنوان اضافی باشد.";
            const apiKey = ""; 
            const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=${apiKey}`;
            const maxRetries = 3;

            showModal(sectionName, 'در حال پردازش...', true);

            for (let attempt = 0; attempt < maxRetries; attempt++) {
                try {
                    const payload = {
                        contents: [{ parts: [{ text: userQuery }] }],
                        systemInstruction: { parts: [{ text: systemPrompt }] },
                        // No grounding tool needed as the task is creative writing based on provided context.
                    };

                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });

                    if (!response.ok) {
                        // Throw error to trigger retry or catch block
                        throw new Error(`HTTP error! status: ${response.status}`);
                    }

                    const result = await response.json();
                    const generatedText = result.candidates?.[0]?.content?.parts?.[0]?.text;

                    if (generatedText) {
                        showModal(sectionName, generatedText, false);
                        return; // Success, exit function
                    } else {
                         throw new Error("API response incomplete or empty content.");
                    }

                } catch (error) {
                    console.error(`Attempt ${attempt + 1} failed for Gemini API call:`, error);
                    if (attempt < maxRetries - 1) {
                        // Exponential backoff delay (1s, 2s, 4s)
                        const delay = Math.pow(2, attempt) * 1000;
                        await new Promise(resolve => setTimeout(resolve, delay));
                    } else {
                        // Final failure
                        showModal(sectionName, 'متأسفانه در حال حاضر امکان تولید معرفی هوشمند وجود ندارد. لطفاً دقایقی دیگر تلاش کنید.', false);
                    }
                }
            }
        };

    </script>
</body>
</html>
