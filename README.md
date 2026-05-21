# 🌌 Shantanu Sarkar Portfolio

A modern dark-themed developer portfolio website built using **HTML & CSS** with glassmorphism UI, responsive layout, animations, and professional sections.

---

# 🚀 Features

- Modern Dark UI
- Fully Responsive Design
- Sticky Sidebar
- Hero Section
- About Me Section
- Tech Stack Section
- Featured Projects
- Stats Cards
- Contact Section
- Smooth Hover Effects
- Modern Gradient Design

---

# 🛠️ Technologies Used

- HTML5
- CSS3
- Google Fonts
- Flexbox
- CSS Grid
- Responsive Design

---

# 📂 Project Structure

```bash
portfolio/
│
├── index.html
├── style.css
└── images/
```

---

# 📸 Preview

![Portfolio Preview](https://i.imgur.com/8Km9tLL.jpg)

---

# 📜 Full HTML Code

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

    .container{
      width:95%;
      max-width:1500px;
      margin:auto;
      display:grid;
      grid-template-columns:320px 1fr;
      gap:25px;
      padding:30px 0;
    }

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

    .card{
      background:linear-gradient(180deg,#0b1020,#070b16);
      border-radius:25px;
      padding:35px;
      border:1px solid rgba(255,255,255,0.08);
    }

    .section-title{
      font-size:28px;
      margin-bottom:25px;
      color:white;
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
    }

    .projects{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:25px;
    }

    .project{
      background:#111827;
      border-radius:20px;
      padding:25px;
    }

    footer{
      text-align:center;
      padding:40px 0;
      color:#94a3b8;
      font-size:14px;
    }

    @media(max-width:1000px){

      .container{
        grid-template-columns:1fr;
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

    }

  </style>
</head>

<body>

  <div class="container">

    <aside class="sidebar">

      <div class="profile-img">
        <img src="https://i.imgur.com/8Km9tLL.jpg">
      </div>

      <h2>Shantanu Sarkar</h2>

      <div class="role">
        Full Stack Developer
      </div>

      <div class="desc">
        Building modern web applications using MERN Stack.
      </div>

    </aside>

    <main class="main">

      <section class="hero">

        <small>WELCOME TO MY PORTFOLIO</small>

        <h1>Shantanu Sarkar</h1>

        <h3>Full Stack Developer</h3>

        <p>Building Real-World Projects</p>

      </section>

    </main>

  </div>

</body>
</html>
```

---

# ▶️ How To Run

1. Create a folder
2. Create a file named `index.html`
3. Paste the code
4. Save the file
5. Open in browser

---

# ⭐ Future Improvements

- Add Dark/Light Toggle
- Add Animations with JavaScript
- Add Backend Contact Form
- Add React Version
- Add Real GitHub API Stats

---

# 👨‍💻 Developer

**Shantanu Sarkar**

Full Stack Developer  
Building Real-World Projects 🚀

---
