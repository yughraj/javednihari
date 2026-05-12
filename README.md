<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Javed Nihari — Karachi's Legendary Nihari Since 1985</title>
<meta name="description" content="Karachi's most legendary nihari — slow-cooked tradition served for generations at Javed Nihari, FB Area and Bahadurabad.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300..700;1,300..700&family=Manrope:wght@300;400;500;600;700&family=Noto+Nastaliq+Urdu:wght@400..700&display=swap" rel="stylesheet">
<style>
/* ============================================
   ROOT & RESET
   ============================================ */
* { margin: 0; padding: 0; box-sizing: border-box; }

:root {
  --bg: #0a0604;
  --bg-rich: #14090480;
  --surface: #1c100780;
  --surface-solid: #1c1007;
  --gold: #d4a04f;
  --gold-light: #f0c970;
  --gold-dark: #a07a35;
  --saffron: #e8893c;
  --ember: #ff6b35;
  --cream: #faf4e6;
  --text: #f4e9d4;
  --text-soft: #b8a585;
  --text-muted: #7a6a4f;
  --border: rgba(212, 160, 79, 0.15);
  --border-bright: rgba(212, 160, 79, 0.4);
}

html { scroll-behavior: smooth; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'Manrope', sans-serif;
  font-weight: 300;
  line-height: 1.6;
  -webkit-font-smoothing: antialiased;
  overflow-x: hidden;
}

a { color: inherit; text-decoration: none; }
button { font-family: inherit; cursor: pointer; border: none; background: none; color: inherit; }

.serif { font-family: 'Cormorant Garamond', serif; font-weight: 400; }
.urdu { font-family: 'Noto Nastaliq Urdu', serif; }
.gold { color: var(--gold); }

.container { max-width: 1280px; margin: 0 auto; padding: 0 2rem; }

/* Ambient texture overlay — film grain */
body::before {
  content: '';
  position: fixed;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='3' /%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.5'/%3E%3C/svg%3E");
  opacity: 0.04;
  pointer-events: none;
  z-index: 9999;
  mix-blend-mode: overlay;
}

/* ============================================
   NAVBAR
   ============================================ */
nav {
  position: fixed;
  top: 0; left: 0; right: 0;
  padding: 1.25rem 2.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 100;
  background: rgba(10, 6, 4, 0.7);
  backdrop-filter: blur(20px) saturate(180%);
  -webkit-backdrop-filter: blur(20px) saturate(180%);
  border-bottom: 1px solid var(--border);
  transition: all 0.3s;
}

.logo {
  display: flex;
  align-items: center;
  gap: 0.6rem;
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.6rem;
  font-weight: 500;
  letter-spacing: 0.02em;
}

.logo-mark {
  width: 36px; height: 36px;
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Cormorant Garamond', serif;
  font-style: italic;
  font-weight: 700;
  font-size: 1.2rem;
  color: var(--bg);
  box-shadow: 0 0 20px rgba(212, 160, 79, 0.4);
}

.logo-text { color: var(--cream); }
.logo-text em { color: var(--gold); font-style: italic; }

.nav-links {
  display: flex;
  gap: 2.5rem;
  list-style: none;
}

.nav-links a {
  color: var(--text-soft);
  font-size: 0.85rem;
  font-weight: 500;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  transition: color 0.2s;
  position: relative;
}

.nav-links a::after {
  content: '';
  position: absolute;
  bottom: -6px;
  left: 0;
  width: 0;
  height: 1px;
  background: var(--gold);
  transition: width 0.3s;
}

.nav-links a:hover { color: var(--gold); }
.nav-links a:hover::after { width: 100%; }

.nav-cta {
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  padding: 0.7rem 1.5rem;
  border-radius: 100px;
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  transition: all 0.3s;
  box-shadow: 0 4px 20px rgba(212, 160, 79, 0.25);
}

.nav-cta:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(212, 160, 79, 0.4);
}

.menu-toggle { display: none; flex-direction: column; gap: 5px; cursor: pointer; padding: 8px; }
.menu-toggle span { display: block; width: 24px; height: 2px; background: var(--gold); transition: all 0.3s; }

/* ============================================
   HERO SECTION
   ============================================ */
.hero {
  min-height: 100vh;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  overflow: hidden;
  padding: 7rem 2rem 4rem;
}

.hero-bg {
  position: absolute;
  inset: 0;
  background-image: 
    linear-gradient(180deg, rgba(10, 6, 4, 0.6) 0%, rgba(10, 6, 4, 0.85) 60%, var(--bg) 100%),
    url('https://images.unsplash.com/photo-1601050690597-df0568f70950?w=2400&auto=format&fit=crop&q=85');
  background-size: cover;
  background-position: center;
  z-index: -2;
  animation: heroZoom 20s ease-in-out infinite alternate;
}

@keyframes heroZoom {
  from { transform: scale(1); }
  to { transform: scale(1.08); }
}

/* Steam particles */
.steam-container {
  position: absolute;
  inset: 0;
  z-index: -1;
  pointer-events: none;
}

.steam {
  position: absolute;
  bottom: -50px;
  width: 6px;
  height: 6px;
  background: radial-gradient(circle, rgba(244, 233, 212, 0.3) 0%, transparent 70%);
  border-radius: 50%;
  filter: blur(2px);
  animation: rise linear infinite;
}

@keyframes rise {
  0% { transform: translateY(0) translateX(0) scale(1); opacity: 0; }
  10% { opacity: 0.8; }
  100% { transform: translateY(-100vh) translateX(40px) scale(3); opacity: 0; }
}

/* Spice particles (floating dots) */
.particle {
  position: absolute;
  width: 3px; height: 3px;
  background: var(--gold);
  border-radius: 50%;
  opacity: 0;
  animation: float 8s ease-in-out infinite;
  box-shadow: 0 0 8px var(--gold);
}

@keyframes float {
  0%, 100% { transform: translateY(0) translateX(0); opacity: 0; }
  10% { opacity: 0.6; }
  50% { transform: translateY(-30px) translateX(15px); opacity: 1; }
  90% { opacity: 0.4; }
}

.hero-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 1rem;
  color: var(--gold);
  font-size: 0.85rem;
  font-weight: 500;
  letter-spacing: 0.4em;
  text-transform: uppercase;
  margin-bottom: 2rem;
  opacity: 0;
  animation: fadeUp 1s 0.2s ease-out forwards;
}

.hero-eyebrow::before, .hero-eyebrow::after {
  content: '';
  width: 50px;
  height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
}

.hero-urdu {
  font-family: 'Noto Nastaliq Urdu', serif;
  font-size: 1.4rem;
  color: var(--gold-light);
  margin-bottom: 1.5rem;
  opacity: 0;
  animation: fadeUp 1s 0.4s ease-out forwards;
}

.hero h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(3.5rem, 9vw, 7.5rem);
  line-height: 0.95;
  letter-spacing: -0.02em;
  font-weight: 400;
  margin-bottom: 1.5rem;
  max-width: 1100px;
  opacity: 0;
  animation: fadeUp 1.2s 0.6s ease-out forwards;
}

.hero h1 em {
  font-style: italic;
  background: linear-gradient(135deg, var(--gold-light) 0%, var(--saffron) 100%);
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}

.hero-subtitle {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(1.1rem, 1.8vw, 1.4rem);
  font-style: italic;
  color: var(--text-soft);
  max-width: 600px;
  margin: 0 auto 3rem;
  opacity: 0;
  animation: fadeUp 1s 0.8s ease-out forwards;
}

.hero-buttons {
  display: flex;
  gap: 1.25rem;
  justify-content: center;
  flex-wrap: wrap;
  opacity: 0;
  animation: fadeUp 1s 1s ease-out forwards;
}

.btn-primary {
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  padding: 1.15rem 2.5rem;
  border-radius: 100px;
  font-size: 0.85rem;
  font-weight: 700;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  transition: all 0.3s;
  display: inline-flex;
  align-items: center;
  gap: 0.6rem;
  box-shadow: 0 6px 30px rgba(212, 160, 79, 0.3);
  position: relative;
  overflow: hidden;
}

.btn-primary::before {
  content: '';
  position: absolute;
  top: 0; left: -100%;
  width: 100%; height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
  transition: left 0.6s;
}

.btn-primary:hover {
  transform: translateY(-3px);
  box-shadow: 0 12px 40px rgba(212, 160, 79, 0.5);
}

.btn-primary:hover::before { left: 100%; }

.btn-outline {
  border: 1px solid var(--gold);
  color: var(--gold);
  padding: 1.15rem 2.5rem;
  border-radius: 100px;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  transition: all 0.3s;
  display: inline-flex;
  align-items: center;
  gap: 0.6rem;
}

.btn-outline:hover {
  background: rgba(212, 160, 79, 0.1);
  border-color: var(--gold-light);
  color: var(--gold-light);
}

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(40px); }
  to { opacity: 1; transform: translateY(0); }
}

/* Floating stat cards */
.hero-stats {
  position: absolute;
  bottom: 3rem;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  gap: 2rem;
  flex-wrap: wrap;
  justify-content: center;
  opacity: 0;
  animation: fadeUp 1s 1.4s ease-out forwards;
}

.stat-pill {
  background: rgba(28, 16, 7, 0.6);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  border: 1px solid var(--border);
  padding: 0.85rem 1.5rem;
  border-radius: 100px;
  display: flex;
  align-items: center;
  gap: 0.75rem;
  font-size: 0.85rem;
  font-weight: 500;
  color: var(--cream);
}

.stat-pill .icon {
  color: var(--gold);
  font-size: 1.1rem;
}

/* ============================================
   SECTION BASE
   ============================================ */
section {
  padding: 7rem 0;
  position: relative;
}

.section-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 1rem;
  color: var(--gold);
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
}

.section-eyebrow::before {
  content: '';
  width: 40px;
  height: 1px;
  background: var(--gold);
}

.section-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  line-height: 1.05;
  letter-spacing: -0.02em;
  margin-bottom: 1.5rem;
  font-weight: 400;
  max-width: 800px;
}

.section-title em {
  font-style: italic;
  color: var(--gold);
}

.section-subtitle {
  font-size: 1.1rem;
  color: var(--text-soft);
  max-width: 600px;
  margin-bottom: 4rem;
  line-height: 1.7;
}

/* ============================================
   MENU SECTION
   ============================================ */
#menu {
  background:
    radial-gradient(circle at 20% 30%, rgba(212, 160, 79, 0.05) 0%, transparent 50%),
    radial-gradient(circle at 80% 70%, rgba(232, 137, 60, 0.04) 0%, transparent 50%),
    var(--bg);
}

.menu-header {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 5rem;
}

.menu-header .section-title { max-width: 900px; }
.menu-header .section-subtitle { margin-bottom: 0; }

.menu-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}

.menu-card {
  background: linear-gradient(180deg, var(--surface-solid) 0%, #14090a 100%);
  border: 1px solid var(--border);
  border-radius: 20px;
  overflow: hidden;
  transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
  position: relative;
  display: flex;
  flex-direction: column;
}

.menu-card:hover {
  transform: translateY(-8px);
  border-color: var(--border-bright);
  box-shadow: 0 20px 60px rgba(212, 160, 79, 0.15);
}

.menu-card-img {
  aspect-ratio: 4/3;
  background-size: cover;
  background-position: center;
  position: relative;
  overflow: hidden;
}

.menu-card-img::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(180deg, transparent 50%, rgba(10, 6, 4, 0.7) 100%);
}

.menu-card:hover .menu-card-img { transform: scale(1.05); }
.menu-card-img { transition: transform 0.6s; }

.badge {
  position: absolute;
  top: 1rem;
  left: 1rem;
  background: rgba(10, 6, 4, 0.85);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid var(--gold);
  color: var(--gold);
  padding: 0.4rem 0.9rem;
  border-radius: 100px;
  font-size: 0.7rem;
  font-weight: 700;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  z-index: 2;
}

.badge.signature {
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  border: none;
}

.menu-card-content {
  padding: 1.75rem;
  display: flex;
  flex-direction: column;
  flex: 1;
}

.menu-card-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.75rem;
  font-weight: 500;
  margin-bottom: 0.5rem;
  color: var(--cream);
}

.menu-card-desc {
  color: var(--text-soft);
  font-size: 0.9rem;
  margin-bottom: 1.25rem;
  line-height: 1.6;
  flex: 1;
}

.menu-card-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 1.25rem;
  border-top: 1px solid var(--border);
}

.spice-meter {
  display: flex;
  gap: 3px;
  align-items: center;
}

.chili {
  font-size: 0.85rem;
  filter: grayscale(1);
  opacity: 0.3;
}

.chili.active { filter: none; opacity: 1; }

.menu-card-price {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.6rem;
  font-weight: 500;
  color: var(--gold);
  font-style: italic;
}

/* ============================================
   ABOUT / STORY
   ============================================ */
#about {
  background:
    linear-gradient(180deg, var(--bg) 0%, #0d0805 100%);
}

.story-grid {
  display: grid;
  grid-template-columns: 5fr 6fr;
  gap: 5rem;
  align-items: center;
}

.story-images {
  position: relative;
  aspect-ratio: 4/5;
}

.story-img {
  position: absolute;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 30px 60px rgba(0,0,0,0.5);
  background-size: cover;
  background-position: center;
}

.story-img-1 {
  top: 0; left: 0;
  width: 70%; height: 60%;
  background-image: url('https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=800&auto=format&fit=crop&q=85');
}

.story-img-2 {
  bottom: 0; right: 0;
  width: 65%; height: 55%;
  background-image: url('https://images.unsplash.com/photo-1601050690597-df0568f70950?w=800&auto=format&fit=crop&q=85');
  border: 6px solid var(--bg);
}

.story-decoration {
  position: absolute;
  top: 50%; left: -2rem;
  font-family: 'Cormorant Garamond', serif;
  font-size: 10rem;
  font-style: italic;
  color: var(--gold);
  opacity: 0.06;
  line-height: 1;
  pointer-events: none;
}

.story-content h2 em { font-style: italic; color: var(--gold); }

.story-content p {
  color: var(--text-soft);
  font-size: 1.05rem;
  margin-bottom: 1.25rem;
  line-height: 1.8;
}

.story-quote {
  font-family: 'Cormorant Garamond', serif;
  font-style: italic;
  font-size: 1.4rem;
  color: var(--gold-light);
  border-left: 2px solid var(--gold);
  padding: 0.5rem 0 0.5rem 1.5rem;
  margin: 2rem 0;
  line-height: 1.5;
}

.counters {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 2rem;
  margin-top: 5rem;
  padding: 3rem 0;
  border-top: 1px solid var(--border);
  border-bottom: 1px solid var(--border);
}

.counter {
  text-align: center;
}

.counter-num {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(2.5rem, 4vw, 3.5rem);
  font-weight: 500;
  color: var(--gold);
  line-height: 1;
  margin-bottom: 0.5rem;
}

.counter-label {
  font-size: 0.85rem;
  color: var(--text-soft);
  text-transform: uppercase;
  letter-spacing: 0.15em;
}

/* ============================================
   REVIEWS
   ============================================ */
#reviews {
  background:
    radial-gradient(circle at 50% 50%, rgba(212, 160, 79, 0.04) 0%, transparent 60%),
    var(--bg);
  text-align: center;
}

#reviews .section-eyebrow,
#reviews .section-title,
#reviews .section-subtitle {
  margin-left: auto;
  margin-right: auto;
}

#reviews .section-eyebrow { display: inline-flex; }

.reviews-track {
  position: relative;
  max-width: 900px;
  margin: 0 auto;
  height: 280px;
}

.review-card {
  position: absolute;
  inset: 0;
  background: linear-gradient(180deg, var(--surface-solid) 0%, #14090a 100%);
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 3rem;
  opacity: 0;
  transition: all 0.6s cubic-bezier(0.16, 1, 0.3, 1);
  display: flex;
  flex-direction: column;
  justify-content: center;
  transform: scale(0.95);
}

.review-card.active {
  opacity: 1;
  transform: scale(1);
}

.review-stars {
  color: var(--gold);
  font-size: 1.2rem;
  letter-spacing: 0.2rem;
  margin-bottom: 1.5rem;
}

.review-text {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(1.2rem, 2vw, 1.6rem);
  font-style: italic;
  color: var(--cream);
  line-height: 1.5;
  margin-bottom: 2rem;
}

.review-author {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
}

.review-avatar {
  width: 48px; height: 48px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Cormorant Garamond', serif;
  font-weight: 700;
  color: var(--bg);
  font-size: 1.1rem;
}

.review-name {
  font-weight: 600;
  color: var(--cream);
  font-size: 0.95rem;
}

.review-meta {
  font-size: 0.8rem;
  color: var(--text-muted);
  margin-top: 2px;
}

.review-dots {
  display: flex;
  gap: 0.6rem;
  justify-content: center;
  margin-top: 2rem;
}

.review-dot {
  width: 8px; height: 8px;
  border-radius: 50%;
  background: var(--border);
  cursor: pointer;
  transition: all 0.3s;
}

.review-dot.active {
  background: var(--gold);
  width: 28px;
  border-radius: 100px;
}

/* ============================================
   GALLERY
   ============================================ */
#gallery {
  background: #0d0805;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: 180px;
  gap: 1rem;
}

.gallery-item {
  background-size: cover;
  background-position: center;
  border-radius: 8px;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: all 0.4s;
}

.gallery-item::after {
  content: '';
  position: absolute;
  inset: 0;
  background: rgba(10, 6, 4, 0.2);
  transition: background 0.3s;
}

.gallery-item:hover {
  transform: scale(1.02);
}

.gallery-item:hover::after {
  background: rgba(10, 6, 4, 0);
}

.gallery-item.tall { grid-row: span 2; }
.gallery-item.wide { grid-column: span 2; }

/* Lightbox */
.lightbox {
  position: fixed;
  inset: 0;
  background: rgba(10, 6, 4, 0.97);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  z-index: 1000;
  display: none;
  align-items: center;
  justify-content: center;
  padding: 2rem;
}

.lightbox.open { display: flex; }

.lightbox-img {
  max-width: 90%;
  max-height: 90%;
  border-radius: 8px;
  box-shadow: 0 30px 80px rgba(0,0,0,0.6);
}

.lightbox-close {
  position: absolute;
  top: 2rem; right: 2rem;
  font-size: 2rem;
  color: var(--gold);
  background: rgba(28, 16, 7, 0.8);
  width: 44px; height: 44px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* ============================================
   LOCATIONS
   ============================================ */
#locations {
  background: var(--bg);
}

.locations-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
}

.location-card {
  background: linear-gradient(180deg, var(--surface-solid) 0%, #14090a 100%);
  border: 1px solid var(--border);
  border-radius: 20px;
  overflow: hidden;
  transition: all 0.3s;
}

.location-card:hover {
  border-color: var(--border-bright);
  transform: translateY(-4px);
}

.location-map {
  aspect-ratio: 16/9;
  background: #1a0f08;
  position: relative;
  overflow: hidden;
}

.location-map iframe {
  width: 100%; height: 100%;
  border: 0;
  filter: invert(0.85) hue-rotate(180deg) saturate(0.5) brightness(0.7);
}

.location-content {
  padding: 2.5rem;
}

.location-badge {
  display: inline-block;
  background: rgba(212, 160, 79, 0.1);
  color: var(--gold);
  padding: 0.3rem 0.8rem;
  border-radius: 100px;
  font-size: 0.7rem;
  font-weight: 700;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  margin-bottom: 1rem;
}

.location-name {
  font-family: 'Cormorant Garamond', serif;
  font-size: 2rem;
  font-weight: 500;
  margin-bottom: 1rem;
  color: var(--cream);
}

.location-info {
  color: var(--text-soft);
  margin-bottom: 0.75rem;
  display: flex;
  align-items: flex-start;
  gap: 0.75rem;
  font-size: 0.95rem;
}

.location-info .icon {
  color: var(--gold);
  flex-shrink: 0;
  margin-top: 0.15rem;
}

.location-buttons {
  display: flex;
  gap: 0.75rem;
  margin-top: 2rem;
}

.btn-location {
  flex: 1;
  padding: 0.9rem;
  border-radius: 100px;
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  text-align: center;
  transition: all 0.2s;
}

.btn-location.primary {
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
}

.btn-location.secondary {
  border: 1px solid var(--gold);
  color: var(--gold);
}

.btn-location:hover { transform: translateY(-2px); }

/* ============================================
   FLOATING WHATSAPP
   ============================================ */
.whatsapp-float {
  position: fixed;
  bottom: 2rem;
  right: 2rem;
  z-index: 99;
  width: 60px;
  height: 60px;
  background: #25d366;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 8px 30px rgba(37, 211, 102, 0.4);
  animation: pulse-wa 2s infinite;
  transition: all 0.3s;
}

.whatsapp-float:hover { transform: scale(1.1); }

@keyframes pulse-wa {
  0%, 100% { box-shadow: 0 8px 30px rgba(37, 211, 102, 0.4); }
  50% { box-shadow: 0 8px 30px rgba(37, 211, 102, 0.4), 0 0 0 12px rgba(37, 211, 102, 0); }
}

.whatsapp-float svg { width: 32px; height: 32px; fill: white; }

/* ============================================
   FOOTER
   ============================================ */
footer {
  background:
    linear-gradient(180deg, var(--bg) 0%, #060402 100%);
  padding: 5rem 0 2rem;
  position: relative;
  overflow: hidden;
  border-top: 1px solid var(--border);
}

.skyline {
  position: absolute;
  bottom: 0; left: 0; right: 0;
  height: 80px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1200 80' preserveAspectRatio='none'%3E%3Cpath fill='%23d4a04f' fill-opacity='0.08' d='M0 80 L0 50 L40 50 L40 30 L60 30 L60 50 L100 50 L100 20 L120 20 L120 10 L140 10 L140 20 L160 20 L160 50 L200 50 L200 35 L220 35 L220 15 L240 15 L240 35 L260 35 L260 50 L300 50 L300 25 L340 25 L340 50 L380 50 L380 30 L400 30 L400 5 L420 5 L420 30 L440 30 L440 50 L480 50 L480 40 L520 40 L520 20 L540 20 L540 40 L580 40 L580 50 L620 50 L620 25 L640 25 L640 10 L660 10 L660 25 L680 25 L680 50 L720 50 L720 35 L760 35 L760 15 L780 15 L780 35 L800 35 L800 50 L840 50 L840 30 L860 30 L860 50 L900 50 L900 20 L940 20 L940 50 L980 50 L980 40 L1020 40 L1020 25 L1040 25 L1040 5 L1060 5 L1060 25 L1080 25 L1080 50 L1120 50 L1120 35 L1160 35 L1160 50 L1200 50 L1200 80 Z'/%3E%3C/svg%3E");
  background-size: 100% 100%;
  pointer-events: none;
}

.footer-content {
  position: relative;
  z-index: 2;
  display: grid;
  grid-template-columns: 1.5fr 1fr 1fr 1fr;
  gap: 3rem;
  margin-bottom: 4rem;
}

.footer-brand .logo { margin-bottom: 1.5rem; }

.footer-tagline {
  font-family: 'Cormorant Garamond', serif;
  font-style: italic;
  font-size: 1.2rem;
  color: var(--text-soft);
  margin-bottom: 1.5rem;
  line-height: 1.5;
}

.footer-urdu {
  font-family: 'Noto Nastaliq Urdu', serif;
  color: var(--gold);
  font-size: 1.3rem;
  margin-bottom: 1rem;
}

.footer-col h4 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.2rem;
  color: var(--cream);
  margin-bottom: 1.5rem;
  font-weight: 500;
}

.footer-col ul { list-style: none; }
.footer-col li { margin-bottom: 0.6rem; }

.footer-col a {
  color: var(--text-soft);
  font-size: 0.9rem;
  transition: color 0.2s;
}

.footer-col a:hover { color: var(--gold); }

.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 2rem;
  border-top: 1px solid var(--border);
  position: relative;
  z-index: 2;
  flex-wrap: wrap;
  gap: 1rem;
}

.footer-bottom-text {
  color: var(--text-muted);
  font-size: 0.85rem;
}

.social-row {
  display: flex;
  gap: 0.75rem;
}

.social-icon {
  width: 36px; height: 36px;
  border: 1px solid var(--border);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--text-soft);
  transition: all 0.3s;
  font-size: 0.95rem;
}

.social-icon:hover {
  background: var(--gold);
  color: var(--bg);
  border-color: var(--gold);
}

.disclaimer {
  text-align: center;
  font-size: 0.75rem;
  color: var(--text-muted);
  margin-top: 2rem;
  font-style: italic;
  opacity: 0.7;
}

.disclaimer a { color: var(--gold); }

/* ============================================
   RESPONSIVE
   ============================================ */
@media (max-width: 968px) {
  .nav-links { display: none; }
  .menu-toggle { display: flex; }
  .nav-links.open {
    display: flex;
    flex-direction: column;
    position: fixed;
    top: 70px; left: 0; right: 0;
    background: rgba(10, 6, 4, 0.98);
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    padding: 2rem;
    gap: 1.5rem;
    border-bottom: 1px solid var(--border);
  }
  
  .hero-stats { display: none; }
  .menu-grid { grid-template-columns: 1fr 1fr; }
  .story-grid { grid-template-columns: 1fr; gap: 3rem; }
  .counters { grid-template-columns: repeat(2, 1fr); gap: 1.5rem; }
  .gallery-grid { grid-template-columns: repeat(2, 1fr); }
  .locations-grid { grid-template-columns: 1fr; }
  .footer-content { grid-template-columns: 1fr 1fr; }
  section { padding: 5rem 0; }
}

@media (max-width: 600px) {
  nav { padding: 1rem 1.25rem; }
  .container { padding: 0 1.25rem; }
  .menu-grid { grid-template-columns: 1fr; }
  .footer-content { grid-template-columns: 1fr; }
  .footer-bottom { flex-direction: column; text-align: center; }
  .whatsapp-float { bottom: 1.25rem; right: 1.25rem; width: 52px; height: 52px; }
  .whatsapp-float svg { width: 26px; height: 26px; }
  .reviews-track { height: 340px; }
  .review-card { padding: 2rem 1.5rem; }
  .story-decoration { display: none; }
}
</style>
</head>
<body>

<!-- NAVBAR -->
<nav>
  <div class="logo">
    <div class="logo-mark">J</div>
    <div class="logo-text">Javed <em>Nihari</em></div>
  </div>
  <ul class="nav-links" id="navLinks">
    <li><a href="#hero">Home</a></li>
    <li><a href="#menu">Menu</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#reviews">Reviews</a></li>
    <li><a href="#gallery">Gallery</a></li>
    <li><a href="#locations">Locations</a></li>
  </ul>
  <a href="#locations" class="nav-cta">Order Now</a>
  <div class="menu-toggle" onclick="document.getElementById('navLinks').classList.toggle('open')">
    <span></span><span></span><span></span>
  </div>
</nav>

<!-- HERO -->
<section class="hero" id="hero">
  <div class="hero-bg"></div>
  <div class="steam-container" id="steamContainer"></div>
  
  <div class="container">
    <div class="hero-eyebrow">Est. 1985 · Karachi</div>
    <div class="hero-urdu">لذتِ روایت</div>
    <h1>Karachi's Most<br><em>Legendary</em> Nihari</h1>
    <p class="hero-subtitle">Slow-cooked tradition served for generations. Every plate tells a story that began on the streets of old Karachi.</p>
    <div class="hero-buttons">
      <a href="#menu" class="btn-primary">Explore Menu →</a>
      <a href="#locations" class="btn-outline">Find a Branch</a>
    </div>
  </div>
  
  <div class="hero-stats">
    <div class="stat-pill"><span class="icon">★</span> 40+ Years Legacy</div>
    <div class="stat-pill"><span class="icon">◆</span> 10,000+ Reviews</div>
    <div class="stat-pill"><span class="icon">♛</span> Karachi Icon</div>
    <div class="stat-pill"><span class="icon">✦</span> Authentic Specialists</div>
  </div>
</section>

<!-- MENU -->
<section id="menu">
  <div class="container">
    <div class="menu-header">
      <div class="section-eyebrow">The Menu</div>
      <h2 class="section-title">Recipes <em>slow-cooked</em> through generations.</h2>
      <p class="section-subtitle">Every dish on our menu has been perfected over four decades — from the spice blend to the slow simmer that lasts through the night.</p>
    </div>
    
    <div class="menu-grid">
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=800&auto=format&fit=crop&q=85');">
          <div class="badge signature">Signature</div>
        </div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Special Nihari</h3>
          <p class="menu-card-desc">Our flagship dish. Tender beef shank slow-cooked for 8 hours in a saffron-rich gravy with 18 hand-ground spices. Also available as double.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 1,150</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=800&auto=format&fit=crop&q=85');">
          <div class="badge">Most Loved</div>
        </div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Nalli Nihari</h3>
          <p class="menu-card-desc">Bone marrow nihari — rich, indulgent, and deeply flavorful. The bone-in cuts release a velvety depth into the gravy.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 800</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1574484284002-952d92456975?w=800&auto=format&fit=crop&q=85');"></div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Maghaz Nihari</h3>
          <p class="menu-card-desc">Brain masala served alongside our signature gravy — a delicacy beloved by purists and adventurous eaters alike.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span>
            </div>
            <div class="menu-card-price">PKR 900</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1546833999-b9f581a1996d?w=800&auto=format&fit=crop&q=85');">
          <div class="badge">Premium</div>
        </div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Boti Nihari</h3>
          <p class="menu-card-desc">Premium boneless cuts in a rich gravy. Available half (Rs. 1,800) or full plate — the ultimate Javed Nihari experience.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 3,000</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1567337710282-00832b415979?w=800&auto=format&fit=crop&q=85');">
          <div class="badge">Sunday Only</div>
        </div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Paya</h3>
          <p class="menu-card-desc">Sunday morning ritual. Slow-cooked goat trotters in a hearty, collagen-rich gravy. Special Paya with daal also available at Rs. 650.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 500</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1565557623262-b51c2513a641?w=800&auto=format&fit=crop&q=85');"></div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Tandoori Roti</h3>
          <p class="menu-card-desc">Fresh from the clay tandoor — crispy edges, pillowy center. Sheermal (Rs. 80) and Taftan (Rs. 80) also available.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 30</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1606502281004-f4ed1456ce3c?w=800&auto=format&fit=crop&q=85');"></div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Sheermal</h3>
          <p class="menu-card-desc">Sweet saffron-infused flatbread, baked golden. A traditional pairing dating back to Mughal-era kitchens.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 80</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1605197181344-d34b5e4d4147?w=800&auto=format&fit=crop&q=85');"></div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Kheer</h3>
          <p class="menu-card-desc">Creamy rice pudding with cardamom and pistachios — the dessert that closes every Javed Nihari meal perfectly.</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 130</div>
          </div>
        </div>
      </div>
      
      <div class="menu-card">
        <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1612102060327-1b7f7e9f5e0f?w=800&auto=format&fit=crop&q=85');"></div>
        <div class="menu-card-content">
          <h3 class="menu-card-title">Rabri</h3>
          <p class="menu-card-desc">Slow-reduced sweetened milk — a celebratory desi dessert. Available by the pyala or by the kilo (Rs. 1,400/kg).</p>
          <div class="menu-card-footer">
            <div class="spice-meter">
              <span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span>
            </div>
            <div class="menu-card-price">PKR 180</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <div class="container">
    <div class="story-grid">
      <div class="story-images">
        <div class="story-decoration">"</div>
        <div class="story-img story-img-1"></div>
        <div class="story-img story-img-2"></div>
      </div>
      <div class="story-content">
        <div class="section-eyebrow">Our Story</div>
        <h2 class="section-title">Four decades of <em>tradition</em>, served in every bowl.</h2>
        <p>Javed Nihari began at Dastagir, Block 15, FB Area — one pot, one recipe, one promise: to serve nihari the way it was meant to be served. Slow-cooked through the night, layered with depth, finished with a generous tarka of fried onions and saffron oil.</p>
        <p>Today, we are a Karachi institution — beloved by locals, sought out by tourists, and remembered fondly by overseas Pakistanis who return home just to taste it again.</p>
        <div class="story-quote">"In a city that never stops moving, our nihari has been worth slowing down for."</div>
        <p>From morning naashta to late-night cravings, our doors stay open for those who understand that real flavor cannot be rushed.</p>
      </div>
    </div>
    
    <div class="counters">
      <div class="counter">
        <div class="counter-num" data-target="50000">0</div>
        <div class="counter-label">Happy Customers</div>
      </div>
      <div class="counter">
        <div class="counter-num" data-target="40">0</div>
        <div class="counter-label">Years of Legacy</div>
      </div>
      <div class="counter">
        <div class="counter-num" data-target="800">0</div>
        <div class="counter-label">Daily Visitors</div>
      </div>
      <div class="counter">
        <div class="counter-num" data-target="15">0</div>
        <div class="counter-label">Signature Dishes</div>
      </div>
    </div>
  </div>
</section>

<!-- REVIEWS -->
<section id="reviews">
  <div class="container">
    <div class="section-eyebrow">What people say</div>
    <h2 class="section-title">Praised across <em>Karachi</em> and beyond.</h2>
    <p class="section-subtitle">From food critics to families, from first-timers to lifelong regulars.</p>
    
    <div class="reviews-track" id="reviewsTrack">
      <div class="review-card active">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Best nihari in Karachi. Hands down. The gravy is rich, the meat falls apart, and the naan is straight from the tandoor. Worth every minute of the wait."</p>
        <div class="review-author">
          <div class="review-avatar">AR</div>
          <div>
            <div class="review-name">Ahmed Raza</div>
            <div class="review-meta">Local Guide · 47 reviews</div>
          </div>
        </div>
      </div>
      
      <div class="review-card">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Authentic old-school desi experience. The spices are perfectly balanced — not too overpowering, deeply flavorful. My family's go-to for over 20 years."</p>
        <div class="review-author">
          <div class="review-avatar">FA</div>
          <div>
            <div class="review-name">Fatima Aslam</div>
            <div class="review-meta">Verified visitor</div>
          </div>
        </div>
      </div>
      
      <div class="review-card">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Crowded but completely worth it. I fly in from Dubai twice a year and Javed Nihari is the first place I visit before I even reach home. Legendary."</p>
        <div class="review-author">
          <div class="review-avatar">UK</div>
          <div>
            <div class="review-name">Usman Khan</div>
            <div class="review-meta">Overseas customer · UAE</div>
          </div>
        </div>
      </div>
      
      <div class="review-card">
        <div class="review-stars">★★★★☆</div>
        <p class="review-text">"Phenomenal food, no question. The nalli nihari was unforgettable. Parking can be tricky during peak hours so go a bit early — but the experience is worth it."</p>
        <div class="review-author">
          <div class="review-avatar">SM</div>
          <div>
            <div class="review-name">Sara Malik</div>
            <div class="review-meta">First-time visitor</div>
          </div>
        </div>
      </div>
      
      <div class="review-card">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Hot naan, spicy nihari, and the kheer at the end — this is what Karachi food culture looks like at its finest. A true institution."</p>
        <div class="review-author">
          <div class="review-avatar">BH</div>
          <div>
            <div class="review-name">Bilal Hussain</div>
            <div class="review-meta">Food blogger</div>
          </div>
        </div>
      </div>
    </div>
    
    <div class="review-dots" id="reviewDots"></div>
  </div>
</section>

<!-- GALLERY -->
<section id="gallery">
  <div class="container">
    <div class="section-eyebrow">Gallery</div>
    <h2 class="section-title">Inside <em>our kitchen</em>.</h2>
    <p class="section-subtitle">Steam-rising bowls, fresh-baked naans, busy evenings — moments from our restaurants captured in motion.</p>
    
    <div class="gallery-grid">
      <div class="gallery-item wide" style="background-image: url('https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=1200&auto=format&fit=crop&q=85');" data-img="https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=1600&auto=format&fit=crop&q=85"></div>
      <div class="gallery-item" style="background-image: url('https://images.unsplash.com/photo-1565557623262-b51c2513a641?w=800&auto=format&fit=crop&q=85');" data-img="https://images.unsplash.com/photo-1565557623262-b51c2513a641?w=1600&auto=format&fit=crop&q=85"></div>
      <div class="gallery-item tall" style="background-image: url('https://images.unsplash.com/photo-1546833999-b9f581a1996d?w=800&auto=format&fit=crop&q=85');" data-img="https://images.unsplash.com/photo-1546833999-b9f581a1996d?w=1600&auto=format&fit=crop&q=85"></div>
      <div class="gallery-item" style="background-image: url('https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=800&auto=format&fit=crop&q=85');" data-img="https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=1600&auto=format&fit=crop&q=85"></div>
      <div class="gallery-item" style="background-image: url('https://images.unsplash.com/photo-1574484284002-952d92456975?w=800&auto=format&fit=crop&q=85');" data-img="https://images.unsplash.com/photo-1574484284002-952d92456975?w=1600&auto=format&fit=crop&q=85"></div>
      <div class="gallery-item wide" style="background-image: url('https://images.unsplash.com/photo-1601050690597-df0568f70950?w=1200&auto=format&fit=crop&q=85');" data-img="https://images.unsplash.com/photo-1601050690597-df0568f70950?w=1600&auto=format&fit=crop&q=85"></div>
      <div class="gallery-item" style="background-image: url('https://images.unsplash.com/photo-1606502281004-f4ed1456ce3c?w=800&auto=format&fit=crop&q=85');" data-img="https://images.unsplash.com/photo-1606502281004-f4ed1456ce3c?w=1600&auto=format&fit=crop&q=85"></div>
    </div>
  </div>
</section>

<!-- LIGHTBOX -->
<div class="lightbox" id="lightbox" onclick="closeLightbox()">
  <div class="lightbox-close">✕</div>
  <img class="lightbox-img" id="lightboxImg" src="" alt="">
</div>

<!-- LOCATIONS -->
<section id="locations">
  <div class="container">
    <div class="section-eyebrow">Visit Us</div>
    <h2 class="section-title">Two branches, <em>one tradition</em>.</h2>
    <p class="section-subtitle">Find your nearest Javed Nihari. Open seven days a week, from morning to late night.</p>
    
    <div class="locations-grid">
      <div class="location-card">
        <div class="location-map">
          <iframe src="https://maps.google.com/maps?q=Dastagir+Block+15+Federal+B+Area+Karachi&t=&z=15&ie=UTF8&iwloc=&output=embed" allowfullscreen></iframe>
        </div>
        <div class="location-content">
          <div class="location-badge">Original Branch</div>
          <h3 class="location-name">FB Area</h3>
          <p class="location-info"><span class="icon">⌖</span> Dastagir, Block No. 15, Federal B Area, Karachi</p>
          <p class="location-info"><span class="icon">◷</span> Daily · 8:00 AM – 12:00 AM · Sunday from 6:00 AM</p>
          <p class="location-info"><span class="icon">☎</span> 0311-4422786 · 0324-7860881 · 021-36372111</p>
          <div class="location-buttons">
            <a href="tel:+923247860881" class="btn-location primary">Call Now</a>
            <a href="https://maps.google.com/?q=Dastagir+Block+15+Federal+B+Area+Karachi" target="_blank" class="btn-location secondary">Directions</a>
          </div>
        </div>
      </div>
      
      <div class="location-card">
        <div class="location-map">
          <iframe src="https://maps.google.com/maps?q=Bahadurabad+Karachi&t=&z=14&ie=UTF8&iwloc=&output=embed" allowfullscreen></iframe>
        </div>
        <div class="location-content">
          <div class="location-badge">Bahadurabad Branch</div>
          <h3 class="location-name">Bahadurabad</h3>
          <p class="location-info"><span class="icon">⌖</span> Main Bahadurabad Chowk, Karachi</p>
          <p class="location-info"><span class="icon">◷</span> Daily · 8:00 AM – 12:00 AM</p>
          <p class="location-info"><span class="icon">☎</span> 021-34933111</p>
          <div class="location-buttons">
            <a href="tel:+922134933111" class="btn-location primary">Call Now</a>
            <a href="https://maps.google.com/?q=Bahadurabad+Karachi" target="_blank" class="btn-location secondary">Directions</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- WHATSAPP FLOAT -->
<a href="https://wa.me/923247860881?text=Salaam!%20I%20would%20like%20to%20place%20an%20order" target="_blank" class="whatsapp-float" aria-label="Order on WhatsApp">
  <svg viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946.003-6.556 5.338-11.891 11.893-11.891 3.181.001 6.167 1.24 8.413 3.488 2.245 2.248 3.481 5.236 3.48 8.414-.003 6.557-5.338 11.892-11.893 11.892-1.99-.001-3.951-.5-5.688-1.448l-6.305 1.654zm6.597-3.807c1.676.995 3.276 1.591 5.392 1.592 5.448 0 9.886-4.434 9.889-9.885.002-5.462-4.415-9.89-9.881-9.892-5.452 0-9.887 4.434-9.889 9.884-.001 2.225.651 3.891 1.746 5.634l-.999 3.648 3.742-.981zm11.387-5.464c-.074-.124-.272-.198-.57-.347-.297-.149-1.758-.868-2.031-.967-.272-.099-.47-.149-.669.149-.198.297-.768.967-.941 1.165-.173.198-.347.223-.644.074-.297-.149-1.255-.462-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.521.151-.172.2-.296.3-.495.099-.198.05-.372-.025-.521-.075-.148-.669-1.611-.916-2.206-.242-.579-.487-.501-.669-.51l-.57-.01c-.198 0-.52.074-.792.372s-1.04 1.016-1.04 2.479 1.065 2.876 1.213 3.074c.149.198 2.095 3.2 5.076 4.487.709.306 1.263.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.695.248-1.29.173-1.414z"/></svg>
</a>

<!-- FOOTER -->
<footer>
  <div class="skyline"></div>
  <div class="container">
    <div class="footer-content">
      <div class="footer-brand">
        <div class="logo">
          <div class="logo-mark">J</div>
          <div class="logo-text">Javed <em>Nihari</em></div>
        </div>
        <div class="footer-urdu">جاوید نہاری</div>
        <p class="footer-tagline">"Serving Karachi's legendary nihari experience for generations."</p>
      </div>
      
      <div class="footer-col">
        <h4>Menu</h4>
        <ul>
          <li><a href="#menu">Special Nihari</a></li>
          <li><a href="#menu">Nalli Nihari</a></li>
          <li><a href="#menu">Paya (Sunday)</a></li>
          <li><a href="#menu">Tandoori Roti</a></li>
        </ul>
      </div>
      
      <div class="footer-col">
        <h4>Visit</h4>
        <ul>
          <li><a href="#locations">FB Area Branch</a></li>
          <li><a href="#locations">Bahadurabad Branch</a></li>
          <li><a href="#locations">Opening Hours</a></li>
          <li><a href="#locations">Get Directions</a></li>
        </ul>
      </div>
      
      <div class="footer-col">
        <h4>Connect</h4>
        <ul>
          <li><a href="#">WhatsApp Order</a></li>
          <li><a href="#">Catering</a></li>
          <li><a href="#">Reservations</a></li>
          <li><a href="#">Reviews</a></li>
        </ul>
      </div>
    </div>
    
    <div class="footer-bottom">
      <div class="footer-bottom-text">© 2026 Javed Nihari. All rights reserved.</div>
      <div class="social-row">
        <a href="#" class="social-icon" aria-label="Facebook">f</a>
        <a href="#" class="social-icon" aria-label="Instagram">⊡</a>
        <a href="#" class="social-icon" aria-label="YouTube">▶</a>
        <a href="#" class="social-icon" aria-label="WhatsApp">✆</a>
      </div>
    </div>
    
    <p class="disclaimer">
      Concept design · Not affiliated with any existing restaurant. Designed by <a href="#" target="_blank">Yugh Studio</a>.
    </p>
  </div>
</footer>

<script>
  // ===== STEAM PARTICLES =====
  const steamContainer = document.getElementById('steamContainer');
  function createSteam() {
    const s = document.createElement('div');
    s.className = 'steam';
    s.style.left = Math.random() * 100 + '%';
    s.style.animationDuration = (6 + Math.random() * 6) + 's';
    s.style.opacity = 0.3 + Math.random() * 0.4;
    steamContainer.appendChild(s);
    setTimeout(() => s.remove(), 12000);
  }
  setInterval(createSteam, 400);
  
  // Spice particles
  for (let i = 0; i < 12; i++) {
    const p = document.createElement('div');
    p.className = 'particle';
    p.style.left = Math.random() * 100 + '%';
    p.style.top = Math.random() * 100 + '%';
    p.style.animationDelay = Math.random() * 8 + 's';
    p.style.animationDuration = (6 + Math.random() * 4) + 's';
    steamContainer.appendChild(p);
  }
  
  // ===== ANIMATED COUNTERS =====
  const counters = document.querySelectorAll('.counter-num');
  const counterObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting && !entry.target.dataset.animated) {
        entry.target.dataset.animated = 'true';
        const target = parseInt(entry.target.dataset.target);
        let current = 0;
        const increment = target / 60;
        const update = () => {
          current += increment;
          if (current < target) {
            entry.target.textContent = Math.floor(current).toLocaleString() + (target >= 1000 ? '' : '');
            requestAnimationFrame(update);
          } else {
            entry.target.textContent = target.toLocaleString() + (target >= 10000 ? '+' : '');
          }
        };
        update();
      }
    });
  }, { threshold: 0.5 });
  counters.forEach(c => counterObserver.observe(c));
  
  // ===== REVIEWS CAROUSEL =====
  const reviewCards = document.querySelectorAll('.review-card');
  const dotsContainer = document.getElementById('reviewDots');
  let currentReview = 0;
  
  reviewCards.forEach((_, i) => {
    const dot = document.createElement('div');
    dot.className = 'review-dot' + (i === 0 ? ' active' : '');
    dot.onclick = () => showReview(i);
    dotsContainer.appendChild(dot);
  });
  const dots = document.querySelectorAll('.review-dot');
  
  function showReview(i) {
    reviewCards[currentReview].classList.remove('active');
    dots[currentReview].classList.remove('active');
    currentReview = i;
    reviewCards[currentReview].classList.add('active');
    dots[currentReview].classList.add('active');
  }
  
  setInterval(() => {
    showReview((currentReview + 1) % reviewCards.length);
  }, 5500);
  
  // ===== LIGHTBOX =====
  const lightbox = document.getElementById('lightbox');
  const lightboxImg = document.getElementById('lightboxImg');
  document.querySelectorAll('.gallery-item').forEach(item => {
    item.addEventListener('click', () => {
      lightboxImg.src = item.dataset.img;
      lightbox.classList.add('open');
    });
  });
  
  function closeLightbox() {
    lightbox.classList.remove('open');
  }
  document.addEventListener('keydown', e => {
    if (e.key === 'Escape') closeLightbox();
  });
  
  // ===== SCROLL REVEAL =====
  const revealObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.style.opacity = '1';
        entry.target.style.transform = 'translateY(0)';
      }
    });
  }, { threshold: 0.1, rootMargin: '0px 0px -50px 0px' });
  
  document.querySelectorAll('.menu-card, .counter, .location-card, .gallery-item').forEach((el, i) => {
    el.style.opacity = '0';
    el.style.transform = 'translateY(30px)';
    el.style.transition = `all 0.7s cubic-bezier(0.16, 1, 0.3, 1) ${i * 0.05}s`;
    revealObserver.observe(el);
  });
  
  // ===== SMOOTH NAV SCROLL =====
  document.querySelectorAll('a[href^="#"]').forEach(a => {
    a.addEventListener('click', (e) => {
      const target = document.querySelector(a.getAttribute('href'));
      if (target) {
        e.preventDefault();
        target.scrollIntoView({ behavior: 'smooth' });
        document.getElementById('navLinks').classList.remove('open');
      }
    });
  });
</script>

</body>
</html>
