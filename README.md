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
        /* --- BRAND COLOR PALETTE DEFINITION (CONSOLIDATED) --- */
        :root {
            /* Primary Text, Headings: Deep Blue */
            --c-primary: #004F71; 
            /* Action, Main Buttons, Secondary Text: Teal Blue */
            --c-action: #007B82; 
            /* Accent, Highlights (40 years, card borders): Gold/Orange */
            --c-accent: #F5A623; 
            /* List Icons, Checkmarks: Vibrant Greenish Teal */
            --c-green: #00A68D; 
            /* Body Background: Very light gray/blue */
            --c-light-bg: #f0f4f8;
            /* Lightest background for list items (Pale Teal/Cyan) */
            --c-light-list: #F0FDFB;
        }

        /* Base styles */
        body {
            font-family: 'Vazirmatn', sans-serif;
            background-color: var(--c-light-bg);
        }
        
        /* Utility Classes based on the consolidated palette */
        .text-primary { color: var(--c-primary); }
        .text-action { color: var(--c-action); }
        .text-accent { color: var(--c-accent); }
        .text-green { color: var(--c-green); }

        .bg-action { background-color: var(--c-action); }
        .bg-action:hover { background-color: #006b72; } /* Darker hover state for action */
        .bg-light-list { background-color: var(--c-light-list); }

        .border-accent { border-color: var(--c-accent); }
        .border-action { border-color: var(--c-action); }

        /* Ensures right-to-left direction for grid layouts */
        .rtl-grid {
            direction: rtl;
        }
        
        /* Hover effect for Collection Cards */
        .collection-card {
            transition: all 0.3s ease-in-out;
            cursor: default;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            background-color: white; /* Explicitly ensure cards are white */
        }
        .collection-card:hover {
            transform: none; 
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            border-bottom-width: 6px; 
        }
    </style>
</head>
<body class="text-gray-800">
    
    <!-- Main container for the infographic content -->
    <div class="container mx-auto p-4 md:p-12 max-w-7xl">

        <!-- Header section of the infographic -->
        <header class="text-center mb-16 pt-4 border-b-2 border-gray-200 pb-6 bg-white rounded-3xl shadow-xl">
            <!-- H1 uses Deep Blue -->
            <h1 class="text-5xl md:text-7xl font-black text-primary mb-3 tracking-wide">مجموعه پرنیا</h1>
            <!-- P uses Action Teal -->
            <p class="text-xl md:text-2xl text-action font-light">پیشرو و نوآور در صنعت طلا و خالق آثار فاخر ،کلکسیونی</p>
        </header>

        <!-- Main content grid -->
        <main class="grid grid-cols-1 md:grid-cols-2 gap-10 md:gap-16 rtl-grid">

            <!-- Section: Years of Experience and Innovation (Featured Block) -->
            <div class="md:col-span-2 bg-white rounded-3xl shadow-2xl p-8 md:p-12 flex flex-col md:flex-row items-center justify-around text-center border-t-8 border-accent">
                <div class="mb-6 md:mb-0">
                    <p class="text-2xl font-bold text-primary mb-[-1rem]">بیش از</p>
                    <!-- Highlight number uses Gold/Orange Accent -->
                    <p class="text-9xl font-extrabold text-accent leading-none">۴۰</p>
                    <p class="text-3xl font-bold text-primary mt-3">سال تجربه</p>
                    <p class="text-xl text-gray-600 mt-2">در سنت اصیل ظریف‌سازی طلا</p>
                </div>
                <!-- Visual separator -->
                <div class="border-t-2 md:border-t-0 md:border-r-2 border-gray-300 w-full md:w-auto md:h-40 mx-8 my-6 opacity-70"></div>
                <!-- Innovation Text -->
                <div class="md:w-1/2">
                    <p class="text-4xl font-extrabold text-primary mb-4">تولیدات تخصصی</p>
                    <p class="text-xl text-gray-700 font-medium leading-loose">تولید تمبر،مدالیون،تابلو،شمش،از جنس طلا و نقره، با بهره‌گیری از تکنولوژی‌های روز دنیا و حفظ اصالت هنری</p>
                </div>
            </div>

            <!-- Section: Licenses and Permissions -->
            <!-- Border uses Action Teal -->
            <div class="bg-white rounded-2xl shadow-xl p-6 md:p-8 border-t-4 border-action">
                <h2 class="text-3xl font-bold text-primary mb-6 text-center border-b pb-3 border-gray-100">لایسنس‌ها و مجوزها</h2>
                <div class="space-y-4 text-xl">
                    <!-- List items use custom light background and Green accent icon -->
                    <div class="flex items-center p-3 bg-light-list rounded-lg font-medium">
                        <span class="text-2xl ml-4 text-green">✅</span>
                        <span>دارای گواهینامه <span class="font-extrabold">ISO 9001</span> در مدیریت کیفیت</span>
                    </div>
                    <div class="flex items-center p-3 bg-light-list rounded-lg font-medium">
                        <span class="text-2xl ml-4 text-green">🏅</span>
                        <span>عضو رسمی <span class="font-extrabold">انجمن طلا و جواهر ایران</span></span>
                    </div>
                    <div class="flex items-center p-3 bg-light-list rounded-lg font-medium">
                        <span class="text-2xl ml-4 text-green">📜</span>
                        <span>پروانه میراث فرهنگی و صنایع دستی</span>
                    </div>
                    <div class="flex items-center p-3 bg-light-list rounded-lg font-medium">
                        <span class="text-2xl ml-4 text-green">👍</span>
                        <span>دارای استاندارد تولید طلای ۲۴ عیار با شماره <span class="font-extrabold">T99</span></span>
                    </div>
                    <div class="flex items-center p-3 bg-light-list rounded-lg font-medium">
                        <span class="text-2xl ml-4 text-green">🏛️</span>
                        <span>عضویت کمیته بین‌المللی موزها <span class="font-extrabold">icom</span></span>
                    </div>
                </div>
            </div>

            <!-- Section: Learn More (External Links) -->
            <!-- Border uses Action Teal -->
            <div class="bg-white rounded-2xl shadow-xl p-6 md:p-8 border-t-4 border-action">
                <h2 class="text-3xl font-bold text-primary mb-6 text-center border-b pb-3 border-gray-100">آشنایی بیشتر</h2>
                <div class="text-center space-y-4 w-full">
                    <p class="text-lg text-gray-700 mb-6">برای مشاهده کاتالوگ‌ها و وب‌سایت‌های مجموعه، از لینک‌های زیر بازدید فرمایید.</p>
                    
                    <!-- Primary action buttons use Action Teal -->
                    <a href="https://www.shemshetala.com/Content/UploadFiles/PARNIA_Co-Collection.pdf" target="_blank" class="block w-full text-center bg-action text-white font-bold py-3 px-6 rounded-xl hover:bg-action transition-colors shadow-md">
                        کاتالوگ مجموعه محصولات
                    </a>
                    <a href="https://www.shemshetala.com/Content/UploadFiles/PARNIA_Co_Shemsh.pdf" target="_blank" class="block w-full text-center bg-action text-white font-bold py-3 px-6 rounded-xl hover:bg-action transition-colors shadow-md">
                        کاتالوگ شمش پرنیا
                    </a>
                    <!-- Secondary links use neutral background -->
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
            
            <!-- Section: The Parnia Collection (Cards) -->
            <div class="md:col-span-2 bg-white rounded-3xl shadow-2xl p-8 md:p-12">
                <h2 class="text-4xl font-extrabold text-primary mb-10 text-center">بخش‌های اصلی مجموعه پرنیا</h2>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                    
                    <!-- Card 1: صنایع دستی پرنیا -->
                    <div class="collection-card p-6 rounded-xl text-center shadow-lg border-b-4 border-accent">
                        <i class="fas fa-gem text-6xl text-accent mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold text-primary mb-2">صنایع دستی پرنیا</h3>
                        <!-- Description margin increased from mb-4 to mb-6 -->
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-6">پیوند هنر و صنعت در تولید آثار نفیس طلا و نقره</p>
                    </div>

                    <!-- Card 2: کارخانه و کارگاه تولید طلا -->
                    <div class="collection-card p-6 rounded-xl text-center shadow-lg border-b-4 border-accent">
                        <i class="fas fa-industry text-6xl text-accent mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold text-primary mb-2">کارخانه و کارگاه تولید طلا</h3>
                        <!-- Description margin increased from mb-4 to mb-6 -->
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-6">تولیدات با کیفیت و مطابق با استانداردهای روز</p>
                    </div>

                    <!-- Card 3: انتشارات پرنیا -->
                    <div class="collection-card p-6 rounded-xl text-center shadow-lg border-b-4 border-accent">
                        <i class="fas fa-book-open text-6xl text-accent mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold text-primary mb-2">انتشارات پرنیا</h3>
                        <!-- Description margin increased from mb-4 to mb-6 -->
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-6">ترویج فرهنگ و تاریخ و مشاهیر ایران جهان در قالب نشر کتب فاخر</p>
                    </div>

                    <!-- Card 4: خانه سکه ایران -->
                    <div class="collection-card p-6 rounded-xl text-center shadow-lg border-b-4 border-accent">
                        <i class="fas fa-coins text-6xl text-accent mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold text-primary mb-2">خانه سکه ایران</h3>
                        <!-- Description margin increased from mb-4 to mb-6 -->
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-6">مرجع خرید شمش‌ها و آثار هنری تولید شده از جنس طلا و نقره</p>
                    </div>

                    <!-- Card 5: بنکداری طلا در بازار -->
                    <div class="collection-card p-6 rounded-xl text-center shadow-lg border-b-4 border-accent">
                        <i class="fas fa-building text-6xl text-accent mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold text-primary mb-2">بنکداری طلا در بازار</h3>
                        <!-- Description margin increased from mb-4 to mb-6 -->
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-6">فعالیت در بازار طلا و ارائه خدمات عمده‌فروشی</p>
                    </div>
                    
                    <!-- Card 6: موزه تمبرهای طلا و نقره ایران -->
                    <div class="collection-card p-6 rounded-xl text-center shadow-lg border-b-4 border-accent">
                        <i class="fas fa-university text-6xl text-accent mb-4 opacity-80"></i>
                        <h3 class="text-2xl font-extrabold text-primary mb-2">موزه تمبرهای طلا و نقره ایران</h3>
                        <!-- Description margin increased from mb-4 to mb-6 -->
                        <p class="text-gray-600 text-sm font-light leading-relaxed mb-6">نمایشگاه دائمی آثار ارزشمند و کلکسیونی</p>
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
        // Import necessary Firebase modules
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, signInWithCustomToken } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        // Global Firebase variables setup
        const firebaseConfig = typeof __firebase_config !== 'undefined' ? JSON.parse(__firebase_config) : {};
        const initialAuthToken = typeof __initial_auth_token !== 'undefined' ? __initial_auth_token : null;
        
        let app, db, auth;

        // --- Firebase Initialization and Auth (Mandatory for the environment) ---
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

        // All previous Gemini/Modal functions have been removed.
    </script>
</body>
</html>
