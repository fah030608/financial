<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Financial Competency: 19-22 Years Old</title>
    <!-- Google Fonts: Sarabun -->
    <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-blue: #1a3a5f;
            --secondary-green: #2d6a4f;
            --accent-gold: #d4af37;
            --light-bg: #f4f7f6;
            --white: #ffffff;
            --text-dark: #333333;
            --transition: all 0.3s ease;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Sarabun', sans-serif;
        }

        body {
            background-color: var(--light-bg);
            color: var(--text-dark);
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: var(--white);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            overflow: hidden;
            animation: fadeIn 0.8s ease-out;
        }

        /* --- Header --- */
        header {
            background: linear-gradient(135deg, var(--primary-blue), var(--secondary-green));
            color: var(--white);
            padding: 40px 20px;
            text-align: center;
        }

        header h1 {
            font-size: 1.8rem;
            margin-bottom: 5px;
        }

        header p {
            font-weight: 300;
            opacity: 0.9;
        }

        .age-badge {
            display: inline-block;
            background: var(--accent-gold);
            color: var(--primary-blue);
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: bold;
            margin-top: 15px;
            font-size: 0.9rem;
        }

        /* --- Financial Characteristics Card --- */
        .highlight-box {
            margin: 30px;
            padding: 25px;
            border-left: 5px solid var(--accent-gold);
            background: #fffdf5;
            border-radius: 0 15px 15px 0;
        }

        .highlight-box h2 {
            color: var(--primary-blue);
            margin-bottom: 10px;
            font-size: 1.2rem;
        }

        /* --- K-S-A Interactive Tabs --- */
        .tabs-container {
            padding: 0 30px;
        }

        .tabs-menu {
            display: flex;
            gap: 10px;
            border-bottom: 2px solid #eee;
        }

        .tab-btn {
            padding: 12px 25px;
            border: none;
            background: none;
            cursor: pointer;
            font-weight: 600;
            color: #777;
            transition: var(--transition);
            border-bottom: 3px solid transparent;
        }

        .tab-btn.active {
            color: var(--secondary-green);
            border-bottom-color: var(--secondary-green);
        }

        .tab-content {
            display: none;
            padding: 20px 0;
            animation: fadeIn 0.5s ease;
        }

        .tab-content.active {
            display: block;
        }

        .ksa-list {
            list-style: none;
        }

        .ksa-list li {
            padding: 8px 0;
            display: flex;
            align-items: flex-start;
        }

        .ksa-list li::before {
            content: '•';
            color: var(--accent-gold);
            font-weight: bold;
            margin-right: 10px;
        }

        /* --- Sub-competency Section --- */
        .sub-comp-section {
            padding: 30px;
            background: #f9f9f9;
        }

        .sub-comp-grid {
            display: grid;
            gap: 15px;
            margin-top: 20px;
        }

        .comp-card {
            background: var(--white);
            border: 1px solid #ddd;
            border-radius: 10px;
            overflow: hidden;
            transition: var(--transition);
        }

        .comp-header {
            padding: 15px 20px;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: var(--white);
        }

        .comp-header:hover {
            background: #f0f4f2;
        }

        .comp-header h3 {
            font-size: 1rem;
            color: var(--primary-blue);
        }

        .comp-body {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
            background: #fafafa;
        }

        .comp-body.open {
            max-height: 200px;
            padding: 15px 20px;
            border-top: 1px solid #eee;
        }

        .chevron {
            width: 12px;
            height: 12px;
            border-right: 2px solid #999;
            border-bottom: 2px solid #999;
            transform: rotate(45deg);
            transition: transform 0.3s;
        }

        .comp-card.active .chevron {
            transform: rotate(-135deg);
        }

        /* --- Activity Ideas --- */
        .activities {
            padding: 30px;
            text-align: center;
        }

        .activity-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .activity-item {
            padding: 20px;
            border-radius: 15px;
            background: var(--light-bg);
            transition: transform 0.3s;
        }

        .activity-item:hover {
            transform: translateY(-5px);
            background: #e8efeb;
        }

        .activity-icon {
            font-size: 2rem;
            margin-bottom: 10px;
            display: block;
        }

        /* --- Banner --- */
        .footer-banner {
            background: var(--primary-blue);
            color: var(--white);
            padding: 30px;
            text-align: center;
            font-weight: 600;
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Responsive */
        @media (max-width: 600px) {
            header h1 { font-size: 1.4rem; }
            .tabs-menu { flex-direction: column; gap: 0; }
            .tab-btn { text-align: left; border-bottom: none; border-left: 3px solid transparent; }
            .tab-btn.active { border-bottom-none; border-left-color: var(--secondary-green); }
        }
    </style>
</head>
<body>

<div class="container">
    <!-- 1. Header -->
    <header>
        <p>📊 Financial Competency Framework</p>
        <h1>สมรรถนะทางการเงิน: วัยเรียนตอนปลาย / เริ่มทำงาน</h1>
        <p>Transition to Independence & Work Life</p>
        <div class="age-badge">กลุ่มอายุ 19 - 22 ปี</div>
    </header>

    <!-- 2. Financial Characteristics Card -->
    <section class="highlight-box">
        <h2>💡 คุณลักษณะทางการเงิน</h2>
        <p>เป็นช่วงวัยที่เปลี่ยนผ่านสู่การใช้ชีวิตอิสระ เริ่มมีรายได้จากงานพาร์ทไทม์หรือเริ่มงานประจำครั้งแรก มีความรับผิดชอบทางการเงินสูงขึ้น และเริ่มตัดสินใจเรื่องการเงินที่ซับซ้อนด้วยตนเอง</p>
    </section>

    <!-- 3. K–S–A Interactive Tabs -->
    <section class="tabs-container">
        <div class="tabs-menu" role="tablist">
            <button class="tab-btn active" onclick="openTab(event, 'knowledge')" role="tab">Knowledge (ความรู้)</button>
            <button class="tab-btn" onclick="openTab(event, 'skills')" role="tab">Skills (ทักษะ)</button>
            <button class="tab-btn" onclick="openTab(event, 'attitudes')" role="tab">Attitudes (ทัศนคติ)</button>
        </div>

        <div id="knowledge" class="tab-content active" role="tabpanel">
            <ul class="ksa-list">
                <li>เข้าใจระบบภาษีเงินได้บุคคลธรรมดาและการหักลดหย่อน</li>
                <li>ความเข้าใจเชิงลึกเกี่ยวกับผลิตภัณฑ์สินเชื่อและการบริหารหนี้</li>
                <li>รู้จักกลไกการทำงานของตลาดทุนและการลงทุนเบื้องต้น</li>
                <li>เข้าใจสิทธิผู้บริโภคทางการเงินและกฎหมายที่เกี่ยวข้อง</li>
            </ul>
        </div>

        <div id="skills" class="tab-content" role="tabpanel">
            <ul class="ksa-list">
                <li>สามารถวางแผนการเงินระยะยาวและคำนวณเงินออมเพื่อเป้าหมายใหญ่</li>
                <li>ทักษะการเปรียบเทียบความคุ้มค่าของสัญญาประกันชีวิตและสุขภาพ</li>
                <li>สามารถคัดกรองความเสี่ยงจากภัยทางการเงินออนไลน์และแชร์ลูกโซ่</li>
                <li>การบริหารจัดการพอร์ตรายรับ-รายจ่ายที่มีความผันผวน</li>
            </ul>
        </div>

        <div id="attitudes" class="tab-content" role="tabpanel">
            <ul class="ksa-list">
                <li>ตระหนักถึงความสำคัญของการสร้างเครดิตบูโรที่ดีตั้งแต่เริ่มต้น</li>
                <li>เห็นคุณค่าของการมีเงินสำรองฉุกเฉิน (Emergency Fund)</li>
                <li>มีวินัยในการออมก่อนใช้ แม้จะมีสิ่งเร้าตามกระแสนิยม</li>
                <li>ยอมรับความเสี่ยงในการลงทุนที่เหมาะสมกับช่วงอายุ</li>
            </ul>
        </div>
    </section>

    <!-- 4. Sub-competency Section -->
    <section class="sub-comp-section">
        <h2>🔍 รายละเอียดสมรรถนะย่อย</h2>
        <div class="sub-comp-grid">
            
            <div class="comp-card">
                <div class="comp-header" onclick="toggleComp(this)">
                    <h3>1. การวางแผนและการจัดการเงิน</h3>
                    <div class="chevron"></div>
                </div>
                <div class="comp-body">
                    <p>กำหนดเป้าหมายการออมเพื่อสร้างความมั่นคง จัดสรรรายได้เข้าสู่ระบบบัญชีที่ชัดเจน และบริหารหนี้สินอย่างเป็นระบบไม่ให้เกินกำลัง</p>
                </div>
            </div>

            <div class="comp-card">
                <div class="comp-header" onclick="toggleComp(this)">
                    <h3>2. การเลือกใช้บริการทางการเงิน</h3>
                    <div class="chevron"></div>
                </div>
                <div class="comp-body">
                    <p>เปรียบเทียบเงื่อนไขและดอกเบี้ยของสถาบันการเงินต่างๆ เข้าใจสัญญาผูกพันทางกฎหมาย และเลือกใช้ Digital Banking อย่างปลอดภัย</p>
                </div>
            </div>

            <div class="comp-card">
                <div class="comp-header" onclick="toggleComp(this)">
                    <h3>3. การรับรู้สิทธิและหน้าที่ทางการเงิน</h3>
                    <div class="chevron"></div>
                </div>
                <div class="comp-body">
                    <p>รู้หน้าที่ในการเสียภาษี รู้จักช่องทางการร้องเรียนเมื่อถูกเอาเปรียบ และเข้าใจความสำคัญของการรักษาข้อมูลส่วนบุคคลทางการเงิน</p>
                </div>
            </div>

        </div>
    </section>

    <!-- 5. Activity Ideas Section -->
    <section class="activities">
        <h2>🎯 กิจกรรมเสริมสร้างประสบการณ์</h2>
        <div class="activity-grid">
            <div class="activity-item">
                <span class="activity-icon">💰</span>
                <strong>First Jobber Planner</strong>
                <p>จำลองการจัดสรรเงินเดือนก้อนแรก</p>
            </div>
            <div class="activity-item">
                <span class="activity-icon">🛡️</span>
                <strong>Risk Hunter</strong>
                <p>เรียนรู้วิธีจับผิดกลโกงทางการเงิน</p>
            </div>
            <div class="activity-item">
                <span class="activity-icon">📈</span>
                <strong>Stock Simulation</strong>
                <p>ทดลองลงทุนผ่านแอปฯ จำลองตลาดหุ้น</p>
            </div>
        </div>
    </section>

    <!-- 6. Key Message Banner -->
    <div class="footer-banner">
        "เริ่มต้นวางแผนวันนี้ เพื่ออิสรภาพทางการเงินในวันหน้า"
    </div>
</div>

<script>
    // Logic สำหรับสลับ Tabs (Knowledge, Skills, Attitudes)
    function openTab(evt, tabName) {
        const contents = document.getElementsByClassName("tab-content");
        for (let i = 0; i < contents.length; i++) {
            contents[i].classList.remove("active");
        }

        const buttons = document.getElementsByClassName("tab-btn");
        for (let i = 0; i < buttons.length; i++) {
            buttons[i].classList.remove("active");
        }

        document.getElementById(tabName).classList.add("active");
        evt.currentTarget.classList.add("active");
    }

    // Logic สำหรับ Expand/Collapse รายละเอียดสมรรถนะย่อย
    function toggleComp(element) {
        const card = element.parentElement;
        const body = card.querySelector('.comp-body');
        
        // สลับ Class สำหรับการแสดงผล
        const isOpen = body.classList.contains('open');
        
        // ปิดอันอื่นก่อน (Optional: Accordion Mode)
        document.querySelectorAll('.comp-body').forEach(el => el.classList.remove('open'));
        document.querySelectorAll('.comp-card').forEach(el => el.classList.remove('active'));

        if (!isOpen) {
            body.classList.add('open');
            card.classList.add('active');
        }
    }
</script>

</body>
</html>
