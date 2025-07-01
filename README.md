<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اینفوگرافیک مجموعه پرنیا</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Vazirmatn', sans-serif;
            background-color: #f0f4f8;
        }
        .brand-text-primary { color: #004F71; }
        .brand-text-secondary { color: #007B82; }
        .brand-bg-primary { background-color: #004F71; }
        .brand-bg-secondary { background-color: #007B82; }
        .brand-accent-orange { color: #F5A623; }
        .brand-accent-green { color: #00A68D; }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 500px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .flowchart-node {
            border: 2px solid #007B82;
            background-color: white;
            padding: 1rem;
            border-radius: 0.5rem;
            text-align: center;
            font-weight: 500;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
        }
        .flowchart-node:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
            border-color: #F5A623;
        }
        .flowchart-line {
            width: 2px;
            background-color: #007B82;
            margin: 0 auto;
        }
        .rtl-grid {
            direction: rtl;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <div class="container mx-auto p-4 md:p-8">

        <header class="text-center mb-16">
            <h1 class="text-4xl md:text-6xl font-black brand-text-primary mb-2">مجموعه پرنیا</h1>
            <p class="text-xl md:text-2xl brand-text-secondary font-light">پیوند هنر، تاریخ و فناوری</p>
        </header>

        <main class="grid grid-cols-1 md:grid-cols-2 gap-8 md:gap-12 rtl-grid">

            <div class="md:col-span-2 bg-white rounded-xl shadow-lg p-8 flex flex-col md:flex-row items-center justify-around text-center">
                <div class="mb-6 md:mb-0">
                    <p class="text-8xl font-black brand-accent-orange">40</p>
                    <p class="text-2xl font-bold brand-text-primary">سال تجربه</p>
                    <p class="text-lg text-gray-600">در سنت اصیل ظریف‌سازی طلا</p>
                </div>
                <div class="border-t-2 md:border-t-0 md:border-r-2 border-gray-200 w-full md:w-auto md:h-32 mx-8"></div>
                <div>
                     <p class="text-3xl font-bold brand-text-primary">نوآوری در خلق آثار فاخر</p>
                     <p class="text-lg mt-2 text-gray-600">تولید تمبر و مدالیون‌های یادبود از طلا و نقره</p>
                </div>
            </div>

            <div class="bg-white rounded-xl shadow-lg p-6 md:p-8">
                <h2 class="text-2xl font-bold brand-text-primary mb-6 text-center">ویژگی‌های منحصر به فرد محصولات</h2>
                <div class="space-y-4 text-lg">
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg">
                        <span class="text-2xl ml-4 brand-accent-green">🥇</span>
                        <span>تولید از <span class="font-bold">طلا و نقره</span> با عیار استاندارد</span>
                    </div>
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg">
                        <span class="text-2xl ml-4 brand-accent-green">🏛️</span>
                        <span>ضرب به سبک <span class="font-bold">نقش برجسته</span> با جزئیات هنرمندانه</span>
                    </div>
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg">
                        <span class="text-2xl ml-4 brand-accent-green">🖼️</span>
                        <span>طراحی <span class="font-bold">یک‌رو</span>، متمایز از سکه‌های متداول</span>
                    </div>
                    <div class="flex items-center p-3 bg-teal-50 rounded-lg">
                        <span class="text-2xl ml-4 brand-accent-green">✨</span>
                        <span>حاشیه <span class="font-bold">دندانه‌دار</span>، الهام‌گرفته از تمبرهای پستی</span>
                    </div>
                </div>
            </div>

            <div class="bg-white rounded-xl shadow-lg p-6 md:p-8 flex flex-col justify-center items-center">
                <h2 class="text-2xl font-bold brand-text-primary mb-6 text-center">جایگاه در میان کلکسیون‌داران</h2>
                <div class="chart-container">
                    <canvas id="rarityChart"></canvas>
                </div>
                <p class="text-center mt-4 text-gray-600 text-lg">بخش بزرگی از آثار تولید شده به دلیل استقبال بالا، به سرعت <span class="font-bold">نایاب یا کمیاب</span> شده‌اند.</p>
            </div>

            <div class="md:col-span-2 bg-white rounded-xl shadow-lg p-6 md:p-8">
                <h2 class="text-3xl font-bold brand-text-primary mb-8 text-center">اکوسیستم جامع پرنیا</h2>
                 <div class="flex flex-col items-center">
                    <div class="flowchart-node w-2/3 md:w-1/3 brand-bg-primary text-white">صنایع دستی پرنیا (هسته مرکزی)</div>
                    <div class="flowchart-line h-8"></div>
                    <div class="grid grid-cols-2 lg:grid-cols-4 gap-4 md:gap-8 w-full">
                        <div class="flex flex-col items-center">
                             <div class="flowchart-node w-full h-full flex items-center justify-center">موزه تمبرهای طلا و نقره</div>
                        </div>
                        <div class="flex flex-col items-center">
                             <div class="flowchart-node w-full h-full flex items-center justify-center">خانه سکه ایران</div>
                        </div>
                        <div class="flex flex-col items-center">
                            <div class="flowchart-node w-full h-full flex items-center justify-center">بنکداری طلا در بازار</div>
                        </div>
                        <div class="flex flex-col items-center">
                             <div class="flowchart-node w-full h-full flex items-center justify-center">انتشارات پرنیا</div>
                        </div>
                    </div>
                </div>
                <p class="text-center mt-8 text-gray-600 text-lg">هر بخش از مجموعه به صورت تخصصی فعالیت می‌کند تا خدماتی کامل و یکپارچه ارائه دهد.</p>
            </div>
            
            <div class="bg-white rounded-xl shadow-lg p-6 md:p-8 flex flex-col justify-center items-center">
                <h2 class="text-2xl font-bold brand-text-primary mb-6 text-center">ارکان اعتبار و کیفیت</h2>
                <div class="chart-container">
                    <canvas id="credentialsChart"></canvas>
                </div>
                 <p class="text-center mt-4 text-gray-600 text-lg">تضمین کیفیت و اصالت با معتبرترین گواهی‌نامه‌های ملی و بین‌المللی.</p>
            </div>
            
             <div class="bg-white rounded-xl shadow-lg p-6 md:p-8 flex flex-col justify-center items-center">
                <h2 class="text-2xl font-bold brand-text-primary mb-6 text-center">آشنایی بیشتر</h2>
                <div class="text-center space-y-4 w-full">
                     <p class="text-lg text-gray-700">برای مشاهده کاتالوگ‌ها و وب‌سایت‌های مجموعه، از لینک‌های زیر بازدید فرمایید.</p>
                     <a href="https://www.shemshetala.com/Content/UploadFiles/PARNIA_Co-Collection.pdf" target="_blank" class="block w-full text-center bg-teal-600 text-white font-bold py-3 px-6 rounded-lg hover:bg-teal-700 transition-colors">
                        کاتالوگ مجموعه محصولات
                     </a>
                     <a href="https://www.shemshetala.com/Content/UploadFiles/PARNIA_Co_Shemsh.pdf" target="_blank" class="block w-full text-center bg-teal-600 text-white font-bold py-3 px-6 rounded-lg hover:bg-teal-700 transition-colors">
                        کاتالوگ شمش پرنیا
                     </a>
                      <a href="https://gssmuseum.com/about/" target="_blank" class="block w-full text-center bg-gray-200 text-gray-800 font-bold py-3 px-6 rounded-lg hover:bg-gray-300 transition-colors">
                        وب‌سایت موزه
                     </a>
                      <a href="https://www.niyaco.com" target="_blank" class="block w-full text-center bg-gray-200 text-gray-800 font-bold py-3 px-6 rounded-lg hover:bg-gray-300 transition-colors">
                        وب‌سایت صنایع دستی پرنیا
                     </a>
                </div>
            </div>

        </main>

        <footer class="text-center mt-16 py-6 border-t border-gray-300">
            <p class="text-gray-600">&copy; 1404 - مجموعه پرنیا. کلیه حقوق محفوظ است.</p>
        </footer>

    </div>

    <script>
        const tooltipTitleCallback = (tooltipItems) => {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
                return label.join(' ');
            }
            return label;
        };

        const rarityCtx = document.getElementById('rarityChart').getContext('2d');
        new Chart(rarityCtx, {
            type: 'doughnut',
            data: {
                labels: ['نایاب و کمیاب', 'در گردش'],
                datasets: [{
                    label: 'وضعیت محصولات',
                    data: [85, 15],
                    backgroundColor: [
                        '#007B82',
                        '#F5A623',
                    ],
                    borderColor: '#ffffff',
                    borderWidth: 4,
                    hoverOffset: 8
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                cutout: '70%',
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            font: {
                                family: 'Vazirmatn',
                                size: 14
                            },
                            color: '#374151'
                        }
                    },
                    tooltip: {
                        rtl: true,
                        textDirection: 'rtl',
                        titleFont: { family: 'Vazirmatn' },
                        bodyFont: { family: 'Vazirmatn' },
                        callbacks: {
                           title: tooltipTitleCallback
                        }
                    }
                }
            }
        });

        const credentialsCtx = document.getElementById('credentialsChart').getContext('2d');
        new Chart(credentialsCtx, {
            type: 'radar',
            data: {
                labels: ['مدیریت کیفیت (ISO)', 'استاندارد محصول (T99)', 'اعتبار فرهنگی (میراث فرهنگی)', 'انطباق صنفی (اتحادیه)'],
                datasets: [{
                    label: 'پوشش استانداردها',
                    data: [90, 85, 95, 80],
                    backgroundColor: 'rgba(0, 123, 130, 0.2)',
                    borderColor: '#007B82',
                    pointBackgroundColor: '#007B82',
                    pointBorderColor: '#fff',
                    pointHoverBackgroundColor: '#fff',
                    pointHoverBorderColor: '#007B82',
                    borderWidth: 2
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    r: {
                        angleLines: {
                            color: '#e5e7eb'
                        },
                        grid: {
                            color: '#e5e7eb'
                        },
                        pointLabels: {
                            font: {
                                family: 'Vazirmatn',
                                size: 12
                            },
                            color: '#1f2937'
                        },
                        ticks: {
                           display: false,
                           backdropColor: 'transparent',
                           stepSize: 20
                        }
                    }
                },
                plugins: {
                    legend: {
                       display: false
                    },
                    tooltip: {
                        rtl: true,
                        textDirection: 'rtl',
                        titleFont: { family: 'Vazirmatn' },
                        bodyFont: { family: 'Vazirmatn' },
                        callbacks: {
                           title: tooltipTitleCallback
                        }
                    }
                }
            }
        });
    </script>

</body>
</html>
