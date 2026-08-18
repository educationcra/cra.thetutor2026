<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>เข้าสู่ระบบ - CRA THE TUTOR 2026</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Thai:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
  <link href="https://cdn.jsdelivr.net/npm/@flaticon/flaticon-uicons@3.3.1/css/all/all.min.css" rel="stylesheet">
  
  <style>
    body { font-family: 'Noto Sans Thai', sans-serif; background: #0f172a; color: #0f172a; }
    
    .color-MD { background: #065f46; color: white; }
    .color-HDS { background: #a3e635; color: #1a2e05; }
    .color-BNS { background: #38bdf8; color: #082f49; }
    .color-RT { background: #a855f7; color: white; }
    .color-HKH { background: #f97316; color: white; }
    .color-PMD { background: #1e3a8a; color: white; }
    .color-INMS { background: #eab308; color: #422006; }
    .color-BME { background: #9f1239; color: white; }
    .color-MHFT { background: #ec4899; color: white; }
  </style>
</head>
<body class="min-h-screen flex items-center justify-center p-4">

  <div class="w-full max-w-md bg-white rounded-3xl overflow-hidden shadow-2xl relative p-6 md:p-8">
    <a href="index.html" class="inline-flex items-center gap-2 text-sm text-slate-500 hover:text-slate-800 font-bold mb-6 no-underline bg-slate-100 px-4 py-2 rounded-full">
      <i class="fi fi-sr-arrow-small-left mt-0.5"></i> กลับหน้าหลัก
    </a>

    <div class="text-center mb-8">
      <div class="w-16 h-16 bg-orange-100 text-orange-500 rounded-2xl flex items-center justify-center mx-auto mb-3 text-2xl">
        <i class="fi fi-sr-sign-in-alt mt-1"></i>
      </div>
      <h1 class="text-2xl font-black text-slate-900">เข้าสู่ระบบ</h1>
      <p class="text-sm text-slate-500">กรอกเบอร์โทรศัพท์ที่ใช้ลงทะเบียนเพื่อเรียกดูบัตรประจำตัว</p>
    </div>

    <!-- Login Form -->
    <div id="loginFormSection">
      <div class="mb-6">
        <label class="block text-sm font-bold text-slate-700 mb-2">เบอร์โทรศัพท์มือถือ</label>
        <input type="tel" id="loginPhone" maxlength="12" placeholder="0XX-XXX-XXXX" oninput="formatPhone(this)" class="w-full p-4 rounded-2xl border border-slate-200 font-bold text-lg text-center outline-none focus:border-orange-500 focus:ring-4 ring-orange-100 transition-all">
      </div>

      <button onclick="doLogin()" id="loginBtn" class="w-full bg-slate-900 text-white py-4 rounded-2xl font-black text-lg shadow-lg hover:bg-orange-500 transition-colors flex justify-center items-center gap-2">
        ตรวจสอบข้อมูล <i class="fi fi-sr-search mt-1"></i>
      </button>
    </div>

    <div id="userCardSection" class="hidden text-center">
      <div class="bg-slate-900 text-white p-6 rounded-3xl shadow-xl">
        <div id="badgeCourse" class="inline-block px-3 py-1 rounded-full text-xs font-black mb-3">--</div>
        <h2 class="text-xl font-bold mb-1" id="userName">--</h2>
        <div class="text-4xl font-black tracking-wider text-orange-400 mb-6" id="userId">--</div>
        
        <div class="bg-white p-3 rounded-2xl inline-block shadow-inner">
           <img id="userQr" src="" alt="QR Code" class="w-48 h-48 object-contain">
        </div>
        
        <p class="text-xs text-slate-400 mt-4">แสดง QR Code นี้แก่เจ้าหน้าที่เพื่อสแกนเข้างาน</p>
      </div>

      <button onclick="resetLogin()" class="mt-6 w-full bg-slate-100 text-slate-600 py-3 rounded-xl font-bold hover:bg-slate-200 transition-colors">
        ค้นหาเบอร์อื่น
      </button>
    </div>
  </div>

  <script>
    const SCRIPT_URL = "https://script.google.com/macros/s/AKfycbyCTpTOTqdytjmsEoBX8a88y3toayWDXBR6G6KzgGka6YhbnvmLNLOF1MuUtlGJnmv9/exec"; 

    const prefixMap = {
      "แพทยศาสตร์": "MD", "วิทยาศาสตร์ข้อมูลสุขภาพ": "HDS", "พยาบาลศาสตร์(4 ปี/หลักสูตรนานาชาติ 4 ปี)": "BNS",
      "รังสีเทคนิค": "RT", "วิทยาศาสตร์การเคลื่อนไหวและสุขภาพ": "HKH", "ฉุกเฉินการแพทย์": "PMD",
      "นวัตกรรมวิทยาศาสตร์การแพทย์": "INMS", "วิศวกรรมชีวการแพทย์": "BME", "เทคโนโลยีอาหารทางการแพทย์และสุขภาพ": "MHFT"
    };

    function formatPhone(el) {
      let v = el.value.replace(/\D/g,'');
      if(v.length > 10) v = v.substring(0,10);
      if(v.length > 6) el.value = v.substring(0,3)+'-'+v.substring(3,6)+'-'+v.substring(6);
      else if(v.length > 3) el.value = v.substring(0,3)+'-'+v.substring(3);
      else el.value = v;
    }

    function doLogin() {
      const phone = document.getElementById('loginPhone').value.trim();
      if(phone.length !== 12) return Swal.fire({icon:'warning', title:'เบอร์โทรไม่ถูกต้อง', text:'กรุณากรอกเบอร์โทรศัพท์ให้ครบ 10 หลัก'});

      const btn = document.getElementById('loginBtn');
      btn.disabled = true; btn.innerHTML = '<i class="fi fi-sr-spinner animate-spin"></i> กำลังค้นหา...';

      fetch(SCRIPT_URL, {
        method: 'POST',
        body: JSON.stringify({ action: 'login', phone: phone })
      })
      .then(r => r.json())
      .then(res => {
        btn.disabled = false; btn.innerHTML = 'ตรวจสอบข้อมูล <i class="fi fi-sr-search mt-1"></i>';
        if(res.status === 'success') {
          document.getElementById('loginFormSection').classList.add('hidden');
          document.getElementById('userCardSection').classList.remove('hidden');

          document.getElementById('userName').innerText = res.name;
          document.getElementById('userId').innerText = res.id;
          document.getElementById('userQr').src = res.qrUrl;

          const pKey = prefixMap[res.course] || "MD";
          const badge = document.getElementById('badgeCourse');
          badge.innerText = res.course;
          badge.className = `inline-block px-3 py-1 rounded-full text-xs font-black mb-3 color-${pKey}`;
        } else {
          Swal.fire({icon:'error', title:'ไม่พบข้อมูล', text: res.message});
        }
      })
      .catch(err => {
        btn.disabled = false; btn.innerHTML = 'ตรวจสอบข้อมูล <i class="fi fi-sr-search mt-1"></i>';
        Swal.fire({icon:'error', title:'ข้อผิดพลาด', text: 'เชื่อมต่อเซิร์ฟเวอร์ไม่ได้'});
      });
    }

    function resetLogin() {
      document.getElementById('loginPhone').value = '';
      document.getElementById('userCardSection').classList.add('hidden');
      document.getElementById('loginFormSection').classList.remove('hidden');
    }
  </script>
</body>
</html>
