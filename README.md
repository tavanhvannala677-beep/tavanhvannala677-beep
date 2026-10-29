<img src="image/4a2c637f229538bd0d27d6ba07e5da8c.jpg"  height="200" width="100%" />
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 70" width="100%" height="70">
  <defs>
    <!-- ไล่เฉดสีนีออนสวยๆ -->
    <linearGradient id="gradientName" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#38BDF8" />
      <stop offset="100%" stop-color="#818CF8" />
    </linearGradient>
    <linearGradient id="gradientDev" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#F43F5E" />
      <stop offset="100%" stop-color="#FB923C" />
    </linearGradient>
  </defs>

  <style>
    .font {
      font-family: 'Fira Code', Consolas, Monaco, monospace;
      font-size: 24px;
      font-weight: 600;
    }
    
    /* ควบคุมเคอร์เซอร์กระพริบ */
    .cursor {
      animation: blink 0.8s infinite;
      fill: #38BDF8;
    }
    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    /* ข้อความที่ 1: My name is Tavanh */
    .line1 {
      animation: typeLine1 8s infinite;
    }
    /* ข้อความที่ 2: I'm Mobile Developer */
    .line2 {
      animation: typeLine2 8s infinite;
    }

    /* การคำนวณเวลา: พิมพ์ -> ค้างไว้ 3 วินาที -> ลบออก -> สลับ */
    @keyframes typeLine1 {
      0% { opacity: 0; clip-path: inset(0 100% 0 0); }
      5% { opacity: 1; clip-path: inset(0 100% 0 0); }
      30% { opacity: 1; clip-path: inset(0 0 0 0); }
      67.5% { opacity: 1; clip-path: inset(0 0 0 0); } /* รอ 3 วิ */
      72.5% { opacity: 0; clip-path: inset(0 100% 0 0); }
      100% { opacity: 0; }
    }

    @keyframes typeLine2 {
      0%, 48% { opacity: 0; clip-path: inset(0 100% 0 0); }
      52% { opacity: 1; clip-path: inset(0 100% 0 0); }
      65% { opacity: 1; clip-path: inset(0 0 0 0); }
      95% { opacity: 1; clip-path: inset(0 0 0 0); } /* รอ 3 วิ */
      100% { opacity: 0; clip-path: inset(0 100% 0 0); }
    }
  </style>

  <g class="font">
    <!-- ข้อความที่ 1 (Tavanh จะเป็นสีฟ้า-ม่วง Gradient) -->
    <g class="line1" transform="translate(100, 42)">
      <text fill="#E2E8F0">My name is </text>
      <text x="160" fill="url(#gradientName)">Tavanh</text>
    </g>

    <!-- ข้อความที่ 2 (Mobile Developer จะเป็นสีส้ม-ชมพู Gradient) -->
    <g class="line2" transform="translate(90, 42)">
      <text fill="#E2E8F0">I'm </text>
      <text x="55" fill="url(#gradientDev)">Mobile Developer</text>
    </g>

    <!-- Cursor ขีดกระพริบ -->
    <rect class="cursor" x="500" y="22" width="10" height="24" rx="2" />
  </g>
</svg>
