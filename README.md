<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 300" width="100%" height="100%">
  <!-- Definitions of gradients, filters and patterns -->
  <defs>
    <!-- Background Gradient -->
    <linearGradient id="bg-gradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#05070f" />
      <stop offset="50%" stop-color="#0a0f1d" />
      <stop offset="100%" stop-color="#03050a" />
    </linearGradient>
    
    <!-- Accent Gradients -->
    <linearGradient id="primary-glow" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00f2fe" />
      <stop offset="100%" stop-color="#4facfe" />
    </linearGradient>
    
    <linearGradient id="secondary-glow" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#7f00ff" />
      <stop offset="100%" stop-color="#e100ff" />
    </linearGradient>

    <linearGradient id="text-gradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00f2fe" />
      <stop offset="50%" stop-color="#7f00ff" />
      <stop offset="100%" stop-color="#ec4899" />
    </linearGradient>

    <!-- Radial glows for futuristic atmosphere -->
    <radialGradient id="radial-glow-1" cx="20%" cy="30%" r="50%">
      <stop offset="0%" stop-color="#00f2fe" stop-opacity="0.15" />
      <stop offset="100%" stop-color="#000000" stop-opacity="0" />
    </radialGradient>
    
    <radialGradient id="radial-glow-2" cx="80%" cy="70%" r="60%">
      <stop offset="0%" stop-color="#7f00ff" stop-opacity="0.12" />
      <stop offset="100%" stop-color="#000000" stop-opacity="0" />
    </radialGradient>
    
    <!-- Cyberpunk grid pattern -->
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#ffffff" stroke-opacity="0.03" stroke-width="1" />
    </pattern>

    <!-- Text shadows & glows -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="6" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
    
    <filter id="subtle-glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="3" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
  </defs>

  <!-- Background Base -->
  <rect width="1200" height="300" fill="url(#bg-gradient)" />
  
  <!-- Glowing Orbs in Background -->
  <circle cx="200" cy="100" r="250" fill="url(#radial-glow-1)" />
  <circle cx="950" cy="200" r="300" fill="url(#radial-glow-2)" />

  <!-- Grid overlay -->
  <rect width="1200" height="300" fill="url(#grid)" />
  
  <!-- Abstract Design Lines / Cyber circuit -->
  <!-- Left accent bar -->
  <path d="M 0 0 L 10 0 L 10 300 L 0 300 Z" fill="url(#text-gradient)" opacity="0.8" />
  
  <!-- Top and Bottom subtle borders -->
  <line x1="10" y1="1" x2="1190" y2="1" stroke="#ffffff" stroke-opacity="0.05" stroke-width="1" />
  <line x1="10" y1="299" x2="1190" y2="299" stroke="#ffffff" stroke-opacity="0.05" stroke-width="1" />

  <!-- Connecting Node Network (Right Side) -->
  <g opacity="0.25">
    <line x1="900" y1="80" x2="1050" y2="50" stroke="#00f2fe" stroke-width="1.5" />
    <line x1="1050" y1="50" x2="1120" y2="150" stroke="#00f2fe" stroke-width="1" />
    <line x1="900" y1="80" x2="980" y2="180" stroke="#7f00ff" stroke-width="1" />
    <line x1="980" y1="180" x2="1120" y2="150" stroke="#7f00ff" stroke-width="1.5" />
    <line x1="980" y1="180" x2="1020" y2="250" stroke="#ec4899" stroke-width="1" />
    <line x1="1120" y1="150" x2="1080" y2="230" stroke="#ec4899" stroke-width="1.5" />
    <line x1="1020" y1="250" x2="1080" y2="230" stroke="#00f2fe" stroke-width="1" />
    
    <!-- Nodes -->
    <circle cx="900" cy="80" r="5" fill="#00f2fe" filter="url(#subtle-glow)" />
    <circle cx="1050" cy="50" r="4" fill="#00f2fe" />
    <circle cx="980" cy="180" r="6" fill="#7f00ff" filter="url(#subtle-glow)" />
    <circle cx="1120" cy="150" r="5" fill="#ec4899" filter="url(#subtle-glow)" />
    <circle cx="1020" cy="250" r="4" fill="#00f2fe" />
    <circle cx="1080" cy="230" r="6" fill="#ec4899" filter="url(#subtle-glow)" />
  </g>
  
  <!-- Glowing Tech Rings (Right Side) -->
  <g transform="translate(1000, 150)">
    <circle cx="0" cy="0" r="90" fill="none" stroke="#7f00ff" stroke-width="1.5" stroke-opacity="0.3" stroke-dasharray="10 15" />
    <circle cx="0" cy="0" r="70" fill="none" stroke="#00f2fe" stroke-width="1" stroke-opacity="0.4" stroke-dasharray="40 8" />
    <circle cx="0" cy="0" r="50" fill="none" stroke="#ec4899" stroke-width="2" stroke-opacity="0.2" stroke-dasharray="5 5" />
    <circle cx="0" cy="0" r="12" fill="none" stroke="#ffffff" stroke-width="2" stroke-opacity="0.7" />
    <circle cx="0" cy="0" r="4" fill="#ffffff" filter="url(#subtle-glow)" />
  </g>

  <!-- Title / Typography (Left/Center Side) -->
  <!-- Floating Code Decorative Text -->
  <text x="80" y="70" font-family="'Fira Code', 'Courier New', monospace" font-size="14" fill="#00f2fe" font-weight="600" letter-spacing="1.5" opacity="0.8">
    &lt;DEVELOPER_PORTFOLIO&gt;
  </text>
  
  <!-- Main Name Title -->
  <text x="80" y="150" font-family="system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif" font-size="62" fill="url(#text-gradient)" font-weight="900" letter-spacing="-1.5" filter="url(#glow)">
   A Y E S H A   H A S H M I 
  </text>

  <!-- Subtitle -->
  <text x="80" y="200" font-family="system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif" font-size="22" fill="#e2e8f0" font-weight="600" letter-spacing="0.5">
    CS Student 
  </text>

  <!-- Small Bio / Focus -->
  <text x="80" y="235" font-family="system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif" font-size="15" fill="#94a3b8" font-weight="400" letter-spacing="0.5">
    ⚡ Constantly learning. Consistently building.
  </text>

  <!-- Floating particles / Sparkles -->
  <circle cx="450" cy="70" r="2" fill="#ffffff" opacity="0.6" />
  <circle cx="620" cy="220" r="3" fill="#00f2fe" opacity="0.5" filter="url(#subtle-glow)" />
  <circle cx="720" cy="110" r="1.5" fill="#ec4899" opacity="0.7" />
  <circle cx="350" cy="260" r="2" fill="#7f00ff" opacity="0.4" />
  <circle cx="150" cy="25" r="1" fill="#ffffff" opacity="0.3" />
  <circle cx="850" cy="270" r="2.5" fill="#00f2fe" opacity="0.4" />
</svg>
# 💫 About Me:
🔭 I’m currently working on: Building scalable full-stack web applications with .NET and Next.<br><br>👯 I’m looking to collaborate on: Open-source web tools, backend APIs, and creative UI/UX projects.<br><br>🤝 I’m looking for help with: Advanced Docker containerization and microservices orchestration.<br><br>🌱 I’m currently learning: Docker, microservices architecture, and cloud networking with Cisco.<br><br>💬 Ask me about: Full-stack web development, C#/.NET, SQL Server database design, and UI design in Figma.


# 💻 Tech Stack:
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) ![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white) ![Framework7](https://img.shields.io/badge/framework7-%23EE350F.svg?style=for-the-badge&logo=framework7&logoColor=white) ![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white) ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) ![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white) ![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white) ![Sketch](https://img.shields.io/badge/Sketch-FFB387?style=for-the-badge&logo=sketch&logoColor=black) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) ![GitLab CI](https://img.shields.io/badge/gitlab%20CI-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.shion.dev/api?username=Ayesha-T-Hashmi&theme=onedark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://streak-stats.demolab.com/?user=Ayesha-T-Hashmi&theme=onedark&hide_border=false)<br/>
![](https://github-readme-stats.shion.dev/api/top-langs/?username=Ayesha-T-Hashmi&theme=onedark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
