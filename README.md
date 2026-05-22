html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>فريانة منصة | مراجعة مثال التهيئة العمرانية 2026</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Cairo', 'Tahoma', 'Segoe UI', sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #e9ecef 100%);
            color: #1a2a3a;
            line-height: 1.7;
        }

        /* شريط التنقل */
        .navbar {
            background: linear-gradient(135deg, #1e3c2c 0%, #2a4a35 100%);
            color: white;
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 20px rgba(0,0,0,0.1);
        }

        .navbar-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            background: rgba(255,255,255,0.2);
            padding: 0.5rem 1rem;
            border-radius: 30px;
        }

        .logo span {
            color: #ffd700;
        }

        .nav-links {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 25px;
            transition: all 0.3s ease;
            font-size: 0.9rem;
        }

        .nav-links a:hover {
            background: #ffd700;
            color: #1e3c2c;
        }

        /* الحاوية الرئيسية */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* البطاقات */
        .card {
            background: white;
            border-radius: 20px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h2 {
            color: #1e3c2c;
            border-right: 5px solid #ffd700;
            padding-right: 1rem;
            margin-bottom: 1.5rem;
            font-size: 1.8rem;
        }

        .card h3 {
            color: #2a5a3a;
            margin: 1rem 0 0.5rem;
            font-size: 1.3rem;
        }

        /* الجداول */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 1.5rem 0;
            background: #f8f9fa;
            border-radius: 12px;
            overflow: hidden;
        }

        th, td {
            border: 1px solid #dee2e6;
            padding: 12px;
            text-align: center;
        }

        th {
            background: #2a4a35;
            color: white;
            font-weight: bold;
        }

        td {
            background: white;
        }

        /* الأزرار */
        .btn {
            display: inline-block;
            background: #1e3c2c;
            color: white;
            padding: 10px 25px;
            border-radius: 30px;
            text-decoration: none;
            margin-top: 1rem;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background: #ffd700;
            color: #1e3c2c;
        }

        .btn-outline {
            background: transparent;
            border: 2px solid #1e3c2c;
            color: #1e3c2c;
        }

        .btn-outline:hover {
            background: #1e3c2c;
            color: white;
        }

        /* معرض الصور */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }

        .gallery-item {
            background: #f8f9fa;
            border-radius: 15px;
            overflow: hidden;
            text-align: center;
            padding: 1rem;
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 12px;
        }

        /* قائمة الإجراءات */
        .procedure-list {
            list-style: none;
            padding: 0;
        }

        .procedure-list li {
            background: #f8f9fa;
            margin: 0.5rem 0;
            padding: 1rem;
            border-radius: 12px;
            border-right: 4px solid #ffd700;
        }

        /* منطقة التوصيات */
        .recommendations {
            background: linear-gradient(135deg, #1e3c2c 0%, #2a4a35 100%);
            color: white;
            border-radius: 20px;
            padding: 2rem;
            margin-top: 2rem;
        }

        .recommendations h2, .recommendations h3 {
            color: #ffd700;
        }

        .recommendations li {
            margin: 0.5rem 0;
        }

        /* الفوتر */
        .footer {
            background: #1a2a3a;
            color: #aaa;
            text-align: center;
            padding: 2rem;
            margin-top: 2rem;
        }

        /* استجابة للهواتف */
        @media (max-width: 768px) {
            .navbar-container {
                flex-direction: column;
                gap: 1rem;
            }
            .container {
                padding: 1rem;
            }
            .card {
                padding: 1.5rem;
            }
            th, td {
                font-size: 0.8rem;
                padding: 8px;
            }
        }

        /* مؤشرات إحصائية */
        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 1rem;
            margin: 1.5rem 0;
        }

        .stat-box {
            background: linear-gradient(135deg, #2a4a35, #1e3c2c);
            color: white;
            text-align: center;
            padding: 1.5rem;
            border-radius: 15px;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: bold;
            color: #ffd700;
        }

        .stat-label {
            font-size: 0.9rem;
            margin-top: 0.5rem;
        }
    </style>
</head>
<body>

    <!-- شريط التنقل -->
    <div class="navbar">
        <div class="navbar-container">
            <div class="logo">🏘️ فريانة <span>منصة</span></div>
            <div class="nav-links">
                <a href="#home">الرئيسية</a>
                <a href="#about">عن التهيئة</a>
                <a href="#expansion">مناطق التوسع</a>
                <a href="#survey">الاستبيان</a>
                <a href="#gallery">المعاينات</a>
                <a href="#recommendations">التوصيات</a>
            </div>
        </div>
    </div>

    <div class="container">

        <!-- القسم الرئيسي -->
        <div id="home" class="card">
            <h2>📌 مراجعة مثال التهيئة العمرانية لبلدية فريانة 2026</h2>
            <p>تتناول هذه الدراسة إشكالية التوسع العمراني غير المنظم والبناء العشوائي في مدينة فريانة بولاية القصرين، من خلال تقييم عملية مراجعة مثال التهيئة العمرانية الذي تمت المصادقة عليه في أبريل 2026.</p>
            <p><strong>إعداد الطالبة:</strong> هيفاء جابلي<br>
            <strong>إشراف:</strong> الأستاذة مهى بوجليدة / المهندسة رحمة شرميطي<br>
            <strong>السنة الجامعية:</strong> 2025-2026</p>
            <div class="stats">
                <div class="stat-box">
                    <div class="stat-number">414</div>
                    <div class="stat-label">هكتار مساحات التوسع الجديدة</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">84%</div>
                    <div class="stat-label">من السكان بنوا دون رخصة</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">68%</div>
                    <div class="stat-label">لا يعلمون بوجود نظام المعلومات الجغرافي</div>
                </div>
            </div>
        </div>

        <!-- عن التهيئة العمرانية -->
        <div id="about" class="card">
            <h2>🏛️ ما هي التهيئة العمرانية؟</h2>
            <p>التهيئة العمرانية هي مجموعة القواعد والإجراءات والتقنيات التي تهدف إلى تنظيم استعمالات الأراضي وتوزيع الوظائف الحضرية (سكنية، تجارية، صناعية، خدمية، ترفيهية) داخل المحيط البلدي، وذلك وفق رؤية استراتيجية شاملة.</p>
            <h3>الفرق بين بلدية فريانة ومعتمدية فريانة</h3>
            <p><strong>معتمدية فريانة:</strong> تضم 12 عمادة (فريانة الوسطى، العرق، الأحواش، الصخيرات، العرعار، حناشي، تلابت، بوشبكة، أم علي، بوحاية، قعرة النعام، عبد العظيم).</p>
            <p><strong>بلدية فريانة:</strong> تضم 6 عمادات فقط (فريانة الوسطى، العرق، الأحواش، الصخيرات، العرعار، حناشي). أما العمادات الست الأخرى فتابعة لبلدية تلابت.</p>
        </div>

        <!-- المخطط القديم والجديد -->
        <div id="expansion" class="card">
            <h2>📊 المقارنة بين المخطط القديم والجديد</h2>
            <table>
                <thead>
                    <tr><th>العنصر</th><th>مخطط 2008</th><th>مخطط 2026</th><th>الدلالة</th></tr>
                </thead>
                <tbody>
                    <tr><td>مساحة التوسع الإجمالية</td><td>1072 هكتار</td><td>1486 هكتار (بإضافة 414 هكتار)</td><td>اعتراف بحجم الزحف العمراني</td></tr>
                    <tr><td>قطاع العرق</td><td>جزء مبرمج، جزء غير مبرمج</td><td>223 هكتار توسع</td><td>إقرار بأن العرق الشرقي أصبح نسيجاً عمرانياً</td></tr>
                    <tr><td>المستشفى الجهوي الجديد</td><td>غير مبرمج</td><td>تم تخصيص موقع له</td><td>إقرار بأن المستشفى أقيم خارج المخطط القديم</td></tr>
                    <tr><td>المدرسة الإعدادية</td><td>غير مبرمجة</td><td>تم تخصيص موقع لها</td><td>تعكس حاجيات سكانية لم يتنبأ بها المخطط القديم</td></tr>
                </tbody>
            </table>

            <h3>مساحات التوسع المعتمدة في المخطط الجديد (2026)</h3>
            <table>
                <thead><tr><th>المنطقة</th><th>المساحة (هكتار)</th></tr></thead>
                <tbody>
                    <tr><td>منطقة العرق</td><td>223</td></tr>
                    <tr><td>حي عبد الرحيم</td><td>142</td></tr>
                    <tr><td>الزردة (الكيس)</td><td>31</td></tr>
                    <tr><td>الهوري</td><td>18</td></tr>
                    <tr><td><strong>الجمل</strong></td><td><strong>414</strong></td></tr>
                </tbody>
            </table>
        </div>

        <!-- أسباب مراجعة المخطط -->
        <div class="card">
            <h2>⚠️ لماذا تمت مراجعة المخطط؟</h2>
            <ul class="procedure-list">
                <li><strong>فشل المخطط القديم (2008) في استيعاب المتغيرات:</strong> صمم في ظل اقتصاد فلاحي وهجرة سلبية، فلم يستطع مواكبة الطفرة العمرانية.</li>
                <li><strong>ظاهرة الكونتيرا وتحويلات التونسيين بالخارج:</strong> تدفقت أموال ضخمة من دول الخليج منذ 2016، اتجهت بالكامل نحو البناء والعقار.</li>
                <li><strong>ظهور أحياء ومرافق بكاملها خارج المخطط:</strong> العرق الشرقي (حي الحدائق)، الزرداء، المستشفى الجهوي الجديد، المدرسة الإعدادية، الملعب البلدي.</li>
                <li><strong>غياب المراجعة الدورية طيلة 18 سنة:</strong> المخطط القديم لم يُراجع منذ 2008 حتى 2026، مما سمح بتراكم الفجوات.</li>
            </ul>
        </div>

        <!-- نتائج الاستبيان -->
        <div id="survey" class="card">
            <h2>📋 نتائج الاستبيان الميداني (50 شخصاً)</h2>
            <table>
                <thead><tr><th>السؤال</th><th>النتيجة</th></tr></thead>
                <tbody>
                    <tr><td>بنيت منزلي بعد سنة 2016</td><td>72%</td></tr>
                    <tr><td>لم أحصل على رخصة بناء مسبقة</td><td>84%</td></tr>
                    <tr><td>سبب عدم الحصول على الرخصة: صعوبة الإجراءات</td><td>52%</td></tr>
                    <tr><td>سبب عدم الحصول على الرخصة: طول المدة</td><td>28%</td></tr>
                    <tr><td>أصف التوسع بأنه عشوائي</td><td>76%</td></tr>
                    <tr><td>السبب الرئيسي لكثرة البناء: عودة التونسيين بالخارج والكونتيرا</td><td>62%</td></tr>
                    <tr><td>لا أعلم بوجود نظام معلومات جغرافي للمخططات</td><td>68%</td></tr>
                    <tr><td>الإجراءات البلدية صعبة أو صعبة جداً</td><td>64%</td></tr>
                </tbody>
            </table>
        </div>

        <!-- الهجرة السلبية -->
        <div class="card">
            <h2>🚶 الهجرة السلبية في فريانة (صافي -619 شخص سنوياً)</h2>
            <p>تعاني معتمدية فريانة من هجرة سلبية، أي أن عدد المغادرين أكبر من عدد الوافدين. الشباب يغادرون بسبب قلة فرص العمل، وضعف الخدمات الجامعية، والمناخ الجاف، وبعد المنطقة عن السواحل.</p>
            <p><strong>لكن المفارقة:</strong> الهجرة تفقد المدينة السكان، لكن الأموال تعود إليها. فالتونسي العامل بالخارج يحرص على تحويل مدخراته إلى وطنه، وأفضل وعاء استثماري هو العقار والبناء. هذه الظاهرة وحدها فجرت الطلب على الأراضي وأحدثت الانفجار العمراني.</p>
        </div>

        <!-- معرض المعاينات الميدانية -->
        <div id="gallery" class="card">
            <h2>📸 معاينات ميدانية (رفض مطالب الربط)</h2>
            <p>خلال فترة التربص، شاركت في المعاينات الأسبوعية لمطالب ربط الماء والكهرباء. سجلت أسباباً متكررة للرفض: الموقع الجغرافي (صبغة فلاحية)، القرب من مجاري الأودية، المنطقة المعزولة (غياب التجمع السكاني)، المطلب الفردي في المناطق الريفية.</p>
            <div class="gallery">
                <div class="gallery-item">
                    <div style="background:#e9ecef; height:200px; display:flex; align-items:center; justify-content:center; border-radius:12px;">📷 معاينة مطلب ربط ماء - المنطقة الريفية</div>
                    <p>معاينة مطلب ربط ماء - مناطق ريفية</p>
                </div>
                <div class="gallery-item">
                    <div style="background:#e9ecef; height:200px; display:flex; align-items:center; justify-content:center; border-radius:12px;">📷 جلسة دراسة رخص البناء (2 أفريل 2026)</div>
                    <p>جلسة دراسة رخص البناء (2 أفريل 2026)</p>
                </div>
                <div class="gallery-item">
                    <div style="background:#e9ecef; height:200px; display:flex; align-items:center; justify-content:center; border-radius:12px;">📷 إعلان نشر المخطط الجديد بالرائد الرسمي</div>
                    <p>إعلان نشر المخطط الجديد (29 أفريل 2026)</p>
                </div>
            </div>
        </div>

        <!-- دليل الإجراءات المبسط -->
        <div class="card">
            <h2>📝 كيف تحصل على رخصة بناء؟ (دليل مبسط)</h2>
            <ul class="procedure-list">
                <li><strong>الخطوة 1:</strong> التوجه إلى مصالح البلدية (مصلحة التعمير) للحصول على استمارة طلب رخصة البناء.</li>
                <li><strong>الخطوة 2:</strong> تجهيز الوثائق المطلوبة (شهادة الملكية، شهادة عدم المطابقة، مخطط هندسي، إثبات الدخل السنوي عند الاقتضاء).</li>
                <li><strong>الخطوة 3:</strong> تقديم الملف كاملاً إلى مصالح البلدية ودفع المعاليم المطلوبة.</li>
                <li><strong>الخطوة 4:</strong> معاينة ميدانية من طرف لجنة مشتركة (مهندس البلدية، ممثل عن الشركة التونسية للكهرباء والغاز، شركة استغلال وتوزيع المياه، مصالح الفلاحة، الشرطة).</li>
                <li><strong>الخطوة 5:</strong> الحصول على الموافقة أو رفض مسبب.</li>
            </ul>
            <p><strong>ملاحظة:</strong> إذا كان البناء قائماً دون رخصة، يتم معاينته بعد البناء، وقد يتم رفض الربط بالشبكات الأساسية إذا كان الموقع غير مناسب (قرب من وادٍ، صبغة فلاحية، إلخ).</p>
        </div>

        <!-- التوصيات -->
        <div id="recommendations" class="recommendations">
            <h2>💡 التوصيات</h2>
            <ul style="margin: 1rem 0 0 2rem;">
                <li><strong>إلزامية المراجعة الدورية كل 5 سنوات:</strong> بدلاً من 18 سنة، مع ربط المخطط بنظام معلومات جغرافي آني.</li>
                <li><strong>إطلاق تطبيق هاتفي (عمّاري/فريانة منصة):</strong> يقدم الخريطة التفاعلية، حاسبة المسافة عن الأودية، متابعة طلبي، تبليغ عن مخالفة، دليل الإجراءات المصور.</li>
                <li><strong>تبسيط مسار المصادقة:</strong> تقليص عدد الهياكل المتدخلة أو تفعيل مبدأ "الصمت موافقة" بشكل جذري.</li>
                <li><strong>حملات توعية ميدانية ورقمية:</strong> لرفع نسبة الوعي بالمخطط الجديد وبأهمية الترخص.</li>
                <li><strong>توقيع اتفاقية تعاون مع بلدية القصرين الجنوبية:</strong> لحل إشكال المناطق الحدودية كالمقيسمات.</li>
            </ul>
        </div>

        <!-- المراجع -->
        <div class="card">
            <h2>📚 المراجع</h2>
            <ul>
                <li>إدارة التعمير والتهيئة الترابية. (2011). <strong>أطلس ولاية القصرين</strong>. وزارة التجهيز والإسكان والتهيئة الترابية.</li>
                <li>المعهد الوطني للإحصاء. (1984-2024). <strong>الإحصاء العام للسكان والسكنى</strong>.</li>
                <li>المندوبية الجهوية للتنمية الفلاحية بالقصرين. (2011). <strong>التقرير السنوي</strong>.</li>
                <li>وزارة التجهيز والإسكان والتهيئة الترابية. (2008). <strong>الأمر عدد 3479 لسنة 2008</strong>.</li>
                <li>وزارة الداخلية. (2020). <strong>الأمر الحكومي عدد 926 لسنة 2020</strong>.</li>
                <li>وزارة الداخلية. (2023). <strong>المرسوم عدد 09 لسنة 2023</strong>.</li>
                <li>ولاية القصرين. (2026). <strong>قرار والي القصرين عدد 1 لسنة 2026</strong>.</li>
            </ul>
        </div>

    </div>

    <!-- الفوتر -->
    <div class="footer">
        <p>© 2026 هيفاء جابلي - مذكرة تخرج لنيل شهادة الجيوماتيك والتهيئة</p>
        <p>جامعة تونس - كلية العلوم الإنسانية والاجتماعية</p>
        <p>تحت إشراف الأستاذة مهى بوجليدة والمهندسة رحمة شرميطي</p>
    </div>

</body>
</html>
