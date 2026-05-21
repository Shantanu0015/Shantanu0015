````md
# 🌌 Shantanu Sarkar Portfolio

A modern dark-themed Full Stack Developer portfolio website built using **HTML & CSS** with a professional UI design, responsive layout, smooth hover effects, animated cards, and glassmorphism styling.

---

# 🚀 Live Features

✅ Modern Dark Theme  
✅ Fully Responsive Layout  
✅ Sticky Sidebar  
✅ Hero Section  
✅ About Me Section  
✅ Tech Stack Section  
✅ Featured Projects  
✅ Stats Cards  
✅ Contact Section  
✅ Hover Effects  
✅ Gradient UI  
✅ Smooth Animations  
✅ Mobile Responsive  

---

# 🛠️ Technologies Used

- HTML5
- CSS3
- Google Fonts
- Flexbox
- CSS Grid
- Media Queries
- Responsive Design

---

# 📂 Folder Structure

```bash
portfolio/
│
├── index.html
├── README.md
└── images/
```

---

# 📸 Preview

![Portfolio Preview](https://i.imgur.com/8Km9tLL.jpg)

---

# 📜 Full Source Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Shantanu Sarkar Portfolio</title>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      font-family:'Poppins',sans-serif;
      background:#050816;
      color:white;
      overflow-x:hidden;
    }

    body::-webkit-scrollbar{
      width:8px;
    }

    body::-webkit-scrollbar-thumb{
      background:#7c3aed;
      border-radius:20px;
    }

    .container{
      width:95%;
      max-width:1500px;
      margin:auto;
      display:grid;
      grid-template-columns:320px 1fr;
      gap:25px;
      padding:30px 0;
    }

    /* SIDEBAR */

    .sidebar{
      position:sticky;
      top:20px;
      height:fit-content;
      background:linear-gradient(180deg,#0b1020,#070b16);
      border:1px solid rgba(255,255,255,0.08);
      border-radius:25px;
      padding:30px;
      box-shadow:0 0 30px rgba(0,0,0,0.5);
    }

    .profile-img{
      width:170px;
      height:170px;
      border-radius:50%;
      overflow:hidden;
      margin:auto;
      border:4px solid #7c3aed;
      box-shadow:0 0 30px #7c3aed;
    }

    .profile-img img{
      width:100%;
      height:100%;
      object-fit:cover;
    }

    .sidebar h2{
      text-align:center;
      margin-top:20px;
      font-size:32px;
    }

    .role{
      text-align:center;
      color:#8b5cf6;
      margin-top:10px;
      font-size:18px;
    }

    .desc{
      margin-top:25px;
      color:#cbd5e1;
      line-height:1.8;
      text-align:center;
      font-size:15px;
    }

    .info{
      margin-top:25px;
    }

    .info div{
      margin-bottom:16px;
      color:#d1d5db;
      font-size:15px;
    }

    .resume-btn{
      display:block;
      width:100%;
      margin-top:25px;
      padding:14px;
      border:none;
      border-radius:15px;
      background:linear-gradient(90deg,#7c3aed,#3b82f6);
      color:white;
      font-size:16px;
      font-weight:600;
      cursor:pointer;
      transition:0.4s;
    }

    .resume-btn:hover{
      transform:translateY(-3px);
      box-shadow:0 10px 25px rgba(124,58,237,0.5);
    }

    .socials{
      margin-top:30px;
      display:flex;
      justify-content:center;
      gap:15px;
    }

    .socials a{
      width:50px;
      height:50px;
      border-radius:50%;
      background:#111827;
      display:flex;
      align-items:center;
      justify-content:center;
      text-decoration:none;
      color:white;
      font-size:20px;
      transition:0.4s;
      border:1px solid rgba(255,255,255,0.08);
    }

    .socials a:hover{
      transform:translateY(-5px);
      background:#7c3aed;
    }

    /* MAIN CONTENT */

    .main{
      display:flex;
      flex-direction:column;
      gap:25px;
    }

    .hero{
      background:linear-gradient(135deg,#111827,#1e1b4b);
      border-radius:25px;
      padding:50px;
      border:1px solid rgba(255,255,255,0.08);
      position:relative;
      overflow:hidden;
    }

    .hero::before{
      content:'';
      position:absolute;
      width:300px;
      height:300px;
      background:#7c3aed;
      filter:blur(120px);
      top:-100px;
      right:-100px;
      opacity:0.3;
    }

    .hero small{
      color:#cbd5e1;
      letter-spacing:2px;
    }

    .hero h1{
      font-size:70px;
      margin-top:10px;
      line-height:1.1;
      background:linear-gradient(to right,#ffffff,#8b5cf6);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
    }

    .hero h3{
      margin-top:15px;
      font-size:30px;
      color:#e2e8f0;
    }

    .hero p{
      margin-top:15px;
      color:#38bdf8;
      font-size:30px;
      font-weight:600;
    }

    /* CARD */

    .card{
      background:linear-gradient(180deg,#0b1020,#070b16);
      border-radius:25px;
      padding:35px;
      border:1px solid rgba(255,255,255,0.08);
      transition:0.4s;
    }

    .card:hover{
      transform:translateY(-5px);
      box-shadow:0 15px 30px rgba(0,0,0,0.4);
    }

    .section-title{
      font-size:28px;
      margin-bottom:25px;
      color:white;
    }

    .about p{
      color:#cbd5e1;
      line-height:1.9;
      font-size:16px;
    }

    .skills{
      display:flex;
      flex-wrap:wrap;
      gap:15px;
    }

    .skill{
      padding:12px 20px;
      background:#111827;
      border-radius:12px;
      border:1px solid rgba(255,255,255,0.08);
      transition:0.3s;
    }

    .skill:hover{
      background:#7c3aed;
      transform:scale(1.05);
    }

    /* PROJECTS */

    .projects{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:25px;
    }

    .project{
      background:#111827;
      border-radius:20px;
      padding:25px;
      border:1px solid rgba(255,255,255,0.08);
      transition:0.4s;
    }

    .project:hover{
      transform:translateY(-8px);
      border-color:#7c3aed;
      box-shadow:0 15px 30px rgba(124,58,237,0.25);
    }

    .project h3{
      margin-bottom:12px;
      font-size:24px;
    }

    .project p{
      color:#cbd5e1;
      line-height:1.7;
      font-size:15px;
    }

    .tags{
      margin-top:18px;
      display:flex;
      gap:10px;
      flex-wrap:wrap;
    }

    .tag{
      background:#1f2937;
      padding:8px 14px;
      border-radius:10px;
      font-size:13px;
    }

    /* STATS */

    .stats{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:20px;
    }

    .stat{
      background:#111827;
      padding:30px;
      border-radius:20px;
      border:1px solid rgba(255,255,255,0.08);
      text-align:center;
    }

    .stat h2{
      font-size:45px;
      margin-top:10px;
      color:#8b5cf6;
    }

    .stat p{
      color:#cbd5e1;
    }

    /* CONTACT */

    .contact{
      text-align:center;
    }

    .contact h2{
      margin-bottom:20px;
    }

    .contact-btn{
      padding:15px 35px;
      border:none;
      border-radius:15px;
      background:linear-gradient(90deg,#7c3aed,#3b82f6);
      color:white;
      font-size:17px;
      font-weight:600;
      cursor:pointer;
      transition:0.4s;
    }

    .contact-btn:hover{
      transform:scale(1.05);
      box-shadow:0 15px 30px rgba(124,58,237,0.4);
    }

    footer{
      text-align:center;
      padding:40px 0;
      color:#94a3b8;
      font-size:14px;
    }

    /* RESPONSIVE */

    @media(max-width:1000px){

      .container{
        grid-template-columns:1fr;
      }

      .sidebar{
        position:relative;
      }

      .hero h1{
        font-size:50px;
      }

    }

    @media(max-width:600px){

      .hero{
        padding:30px;
      }

      .hero h1{
        font-size:38px;
      }

      .hero h3{
        font-size:24px;
      }

      .hero p{
        font-size:20px;
      }

      .card{
        padding:25px;
      }

    }

  </style>
</head>
<body>

  <div class="container">

    <!-- SIDEBAR -->

    <aside class="sidebar">

      <div class="profile-img">
        <img src="https://i.imgur.com/8Km9tLL.jpg">
      </div>

      <h2>Shantanu Sarkar</h2>

      <div class="role">
        Full Stack Developer
      </div>

      <div class="desc">
        Building modern web applications using MERN Stack with beautiful UI/UX and powerful backend systems.
      </div>

      <div class="info">
        <div>📍 Kolkata, India</div>
        <div>📧 shantanu@gmail.com</div>
        <div>📞 +91 9876543210</div>
        <div>💻 shantanu.dev</div>
      </div>

      <button class="resume-btn">
        Download Resume
      </button>

      <div class="socials">
        <a href="#">🌐</a>
        <a href="#">💼</a>
        <a href="#">📷</a>
        <a href="#">🐦</a>
      </div>

    </aside>

    <!-- MAIN -->

    <main class="main">

      <section class="hero">

        <small>WELCOME TO MY PORTFOLIO</small>

        <h1>Shantanu Sarkar</h1>

        <h3>Full Stack Developer</h3>

        <p>Building Real-World Projects</p>

      </section>

      <section class="card about">

        <h2 class="section-title">👨‍💻 About Me</h2>

        <p>
          I am a passionate Full Stack Developer focused on creating responsive,
          modern and user-friendly websites using HTML, CSS, JavaScript, React,
          Node.js and MongoDB.
        </p>

      </section>

      <section class="card">

        <h2 class="section-title">⚡ Tech Stack</h2>

        <div class="skills">

          <div class="skill">HTML</div>
          <div class="skill">CSS</div>
          <div class="skill">JavaScript</div>
          <div class="skill">React</div>
          <div class="skill">Node.js</div>
          <div class="skill">MongoDB</div>

        </div>

      </section>

      <section class="card">

        <h2 class="section-title">🚀 Featured Projects</h2>

        <div class="projects">

          <div class="project">
            <h3>Portfolio Website</h3>
            <p>Modern responsive developer portfolio website.</p>
          </div>

          <div class="project">
            <h3>StudyPedia AI</h3>
            <p>AI powered study platform for students.</p>
          </div>

        </div>

      </section>

      <footer>
        © 2026 Shantanu Sarkar | All Rights Reserved
      </footer>

    </main>

  </div>

</body>
</html>
```

---

# ▶️ How To Run

```bash
1. Create a folder
2. Create index.html
3. Paste the code
4. Save the file
5. Open in browser
```

---

# ⭐ Future Improvements

- Add JavaScript Animations
- Add GitHub API
- Add Dark/Light Mode
- Add Contact Backend
- Convert into React.js

---

# 👨‍💻 Developer

## Shantanu Sarkar

Full Stack Developer  
Building Real-World Projects 🚀

---
````
