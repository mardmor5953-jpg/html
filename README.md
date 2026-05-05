# html
portfolio
index.html 
s project1.jpg,
S, project2.jpg,
CSS VARIABLES — Edit colors here!
============================ */
  --color-primary: #0066cc;    /* Main color needs to be white   */
  --color-bg: #ffffff;          /* Page background white  */
  --color-text: #1a1a2e;        /* Main text words need to  be black  */
  --color-muted: #666680;       /* Subtle text */
  --color-card: #f4f6ff;        /* Card backgrounds  black*/
  --font-main: 'Segoe UI', Arial, sans-serif;
}

/* ============================
   GLOBAL RESET
============================ */
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  font-family: var(--font-main);                 
  background: var(--color-bg);
  color: var(--color-text);
  line-height: 1.6;
}

.container {
  max-width: 900px;
  margin: 0 auto;
  padding: 0 24px;
}

/* NAVIGATION */
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 16px 40px;
  background: var(--color-primary);
  position: sticky;
  top: 0;
}
nav .nav-name { color: white; font-weight: 700; font-size: 18px; }
nav ul { list-style: none; display: flex; gap: 24px; }
nav ul a { color: rgba(255,255,255,0.85); text-decoration: none; font-weight: 500; }
nav ul a:hover { color: white; }

/* SECTIONS */
section { padding: 80px 40px; }
section:nth-child(even) { background: var(--color-card); }
h2 {
  font-size: 32px;
  margin-bottom: 40px;
  color: var(--color-primary);
}

/* ABOUT SECTION */
#about { text-align: center; }
.avatar {
  width: 150px; height: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid var(--color-primary);
  margin-bottom: 20px;
}
#about h1 { font-size: 42px; margin-bottom: 8px; }
.highlight { color: var(--color-primary); }
.grade-label { color: var(--color-muted); margin-bottom: 16px; }
.bio { max-width: 600px; margin: 0 auto; font-size: 17px; }

/* SKILLS GRID */
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 16px;
}
.skill-card {
  background: white;
  border: 2px solid var(--color-primary);
  border-radius: 10px;
  padding: 16px;
  text-align: center;
  font-weight: 600;
  transition: transform 0.2s, background 0.2s;
}
.skill-card:hover {
  background: var(--colo_white);
  color: white;
  transform: translateY(-4px);
}

/* PROJECTS GRID */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
}
.project-card {
  background: white;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 20px rgba(0,0,0,0.08);
  transition: transform 0.2s;
}
.project-card:hover { transform: translateY(-6px); }
.project-card img { width: 100%; height: 200px; object-fit: cover; }
.project-info { padding: 20px; }
.project-info h3 { margin-bottom: 8px; font-size: 18px; }
.project-info p { color: var(--color-muted); font-size: 14px; margin-bottom: 12px; }
.tech-tags { display: flex; flex-wrap: wrap; gap: 6px; }
.tech-tags span {
  padding: 4px 10px;
  background: var(--color-card);
  border-radius: 20px;
  font-size: 12px;
  font-weight: 600;
  color: var(--color-primary);
}

/* CONTACT SECTION */
#contact { text-align: center; }
.email-link {
  display: inline-block;
  margin-top: 20px;
  padding: 14px 30px;
  background: var(--color-primary);
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-weight: 600;
  font-size: 16px;
  transition: opacity 0.2s;
}
.email-link:hover { opacity: 0.85; }

/* FOOTER */
footer {
  text-align: center;
  padding: 24px;
  background: var(--color-primary);
  color: rgba(255,255,255,0.8);
  font-size: 13px;
}
