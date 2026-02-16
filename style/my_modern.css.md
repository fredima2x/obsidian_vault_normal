/* === Modern Obsidian Slides Theme === */

:root {
  --bg-main: #0f1226;
  --bg-card: rgba(255, 255, 255, 0.05);
  --accent: #7c5cff;
  --accent-2: #00d4ff;
  --text-main: #f5f7fa;
  --text-muted: #aab0c0;
  --border-glass: rgba(255, 255, 255, 0.1);
}

/* === Background === */
.reveal {
  background: radial-gradient(circle at top left, #1a1f4a, #0f1226 60%);
  color: var(--text-main);
  font-family: "Inter", "SF Pro Display", sans-serif;
}

/* === Slides === */
.reveal .slides section {
  padding: 2rem;
}

/* === Headings === */
.reveal h1, 
.reveal h2, 
.reveal h3 {
  font-weight: 700;
  background: linear-gradient(90deg, var(--accent), var(--accent-2));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-bottom: 1rem;
}

.reveal h1 {
  font-size: 3rem;
}

.reveal h2 {
  font-size: 2.2rem;
}

.reveal h3 {
  font-size: 1.6rem;
}

/* === Paragraphs === */
.reveal p {
  color: var(--text-muted);
  font-size: 1.2rem;
  line-height: 1.6;
}

/* === Cards / Glass Effect === */
.glass {
  background: var(--bg-card);
  backdrop-filter: blur(16px);
  border: 1px solid var(--border-glass);
  border-radius: 16px;
  padding: 1.5rem;
  box-shadow: 0 8px 32px rgba(0,0,0,0.4);
}

/* === Lists === */
.reveal ul {
  list-style: none;
  padding-left: 0;
}

.reveal ul li::before {
  content: "▹";
  color: var(--accent);
  margin-right: 0.6rem;
}

/* === Code Blocks === */
.reveal pre {
  background: #151932;
  border-radius: 12px;
  padding: 1rem;
  box-shadow: 0 6px 20px rgba(0,0,0,0.5);
}

.reveal code {
  color: var(--accent-2);
  font-family: "Fira Code", monospace;
}

/* === Tables === */
.reveal table {
  border-collapse: collapse;
  width: 100%;
  font-size: 1rem;
}

.reveal table th {
  background: rgba(124, 92, 255, 0.2);
  padding: 0.8rem;
}

.reveal table td {
  padding: 0.8rem;
  border-bottom: 1px solid rgba(255,255,255,0.08);
}

/* === Links === */
.reveal a {
  color: var(--accent);
  text-decoration: none;
}

.reveal a:hover {
  text-shadow: 0 0 8px var(--accent);
}

/* === Slide Transition Feel === */
.reveal .slides section {
  transition: all 0.6s ease;
}

/* === Center Title Slide === */
.title-slide {
  text-align: center;
}

.title-slide h1 {
  font-size: 3.5rem;
}

.title-slide p {
  font-size: 1.3rem;
  color: var(--text-muted);
}

/* === Subtle Animation === */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.reveal section.present {
  animation: fadeInUp 0.8s ease;
}
