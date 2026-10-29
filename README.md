<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 60" width="100%" height="60">
  <defs>
    <!-- ไล่เฉดสีนีออนหลากสี -->
    <linearGradient id="gradientName" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#38BDF8" />
      <stop offset="100%" stop-color="#A855F7" />
    </linearGradient>
    <linearGradient id="gradientDev" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#FB923C" />
      <stop offset="100%" stop-color="#F43F5E" />
    </linearGradient>
  </defs>

  <style>
    .font {
      font-family: 'Fira Code', Consolas, Monaco, monospace;
      font-size: 24px;
      font-weight: bold;
    }
    
    .cursor {
      animation: blink 0.8s infinite;
      fill: #38BDF8;
    }
    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    .line1 {
      animation: type1 8s infinite;
    }
    .line2 {
      animation: type2 8s infinite;
    }

    @keyframes type1 {
      0% { opacity: 0; clip-path: inset(0 100% 0 0); }
      5% { opacity: 1; clip-path: inset(0 100% 0 0); }
      30%, 65% { opacity: 1; clip-path: inset(0 0 0 0); } /* รอ 3 วินาที */
      70% { opacity: 0; clip-path: inset(0 100% 0 0); }
      100% { opacity: 0; }
    }

    @keyframes type2 {
      0%, 45% { opacity: 0; clip-path: inset(0 100% 0 0); }
      50% { opacity: 1; clip-path: inset(0 100% 0 0); }
      75%, 95% { opacity: 1; clip-path: inset(0 0 0 0); } /* รอ 3 วินาที */
      100% { opacity: 0; clip-path: inset(0 100% 0 0); }
    }
  </style>

  <g class="font">
    <!-- ข้อความที่ 1: My name is (สีขาว) Tavanh (สีฟ้าไล่ม่วง) -->
    <g class="line1" transform="translate(100, 38)">
      <text fill="#FFFFFF">My name is </text>
      <text x="165" fill="url(#gradientName)">Tavanh</text>
    </g>

    <!-- ข้อความที่ 2: I'm (สีขาว) Mobile Developer (สีส้มไล่ชมพู) -->
    <g class="line2" transform="translate(90, 38)">
      <text fill="#FFFFFF">I'm </text>
      <text x="55" fill="url(#gradientDev)">Mobile Developer</text>
    </g>

    <!-- เคอร์เซอร์ขีดกะพริบ -->
    <rect class="cursor" x="500" y="16" width="10" height="26" rx="2" />
  </g>
</svg>
