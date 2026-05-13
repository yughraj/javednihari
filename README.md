<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Javed Nihari — Karachi's Legendary Nihari Since 1985</title>
<meta name="description" content="Karachi's most legendary nihari — slow-cooked tradition served for generations.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300..700;1,300..700&family=Manrope:wght@300;400;500;600;700&family=Noto+Nastaliq+Urdu:wght@400..700&display=swap" rel="stylesheet">
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }
:root {
  --bg: #0a0604; --surface-solid: #1c1007;
  --gold: #d4a04f; --gold-light: #f0c970; --saffron: #e8893c;
  --cream: #faf4e6; --text: #f4e9d4;
  --text-soft: #b8a585; --text-muted: #7a6a4f;
  --border: rgba(212, 160, 79, 0.15);
  --border-bright: rgba(212, 160, 79, 0.4);
}
html { scroll-behavior: smooth; }
body { background: var(--bg); color: var(--text); font-family: 'Manrope', sans-serif; font-weight: 300; line-height: 1.6; -webkit-font-smoothing: antialiased; overflow-x: hidden; }
a { color: inherit; text-decoration: none; }
button { font-family: inherit; cursor: pointer; border: none; background: none; color: inherit; }
.container { max-width: 1280px; margin: 0 auto; padding: 0 2rem; }
body::before { content: ''; position: fixed; inset: 0; background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='3' /%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.5'/%3E%3C/svg%3E"); opacity: 0.04; pointer-events: none; z-index: 9999; mix-blend-mode: overlay; }

nav { position: fixed; top: 0; left: 0; right: 0; padding: 1.25rem 2.5rem; display: flex; justify-content: space-between; align-items: center; z-index: 100; background: rgba(10, 6, 4, 0.7); backdrop-filter: blur(20px) saturate(180%); -webkit-backdrop-filter: blur(20px) saturate(180%); border-bottom: 1px solid var(--border); transition: all 0.3s; }
.logo { display: flex; align-items: center; gap: 0.6rem; font-family: 'Cormorant Garamond', serif; font-size: 1.6rem; font-weight: 500; letter-spacing: 0.02em; }
.logo-mark { width: 36px; height: 36px; background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-family: 'Cormorant Garamond', serif; font-style: italic; font-weight: 700; font-size: 1.2rem; color: var(--bg); box-shadow: 0 0 20px rgba(212, 160, 79, 0.4); }
.logo-text { color: var(--cream); }
.logo-text em { color: var(--gold); font-style: italic; }
.nav-links { display: flex; gap: 2.2rem; list-style: none; align-items: center; }
.nav-links li { display: flex; align-items: center; }
.nav-links a { color: var(--text-soft); font-size: 0.85rem; font-weight: 500; letter-spacing: 0.05em; text-transform: uppercase; transition: color 0.2s; position: relative; line-height: 1; }
.nav-links a::after { content: ''; position: absolute; bottom: -6px; left: 0; width: 0; height: 1px; background: var(--gold); transition: width 0.3s; }
.nav-links a:hover { color: var(--gold); }
.nav-links a:hover::after { width: 100%; }
.nav-cta { background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%); color: var(--bg); padding: 0.7rem 1.5rem; border-radius: 100px; font-size: 0.8rem; font-weight: 700; letter-spacing: 0.05em; text-transform: uppercase; transition: all 0.3s; box-shadow: 0 4px 20px rgba(212, 160, 79, 0.25); }
.nav-cta:hover { transform: translateY(-2px); box-shadow: 0 8px 30px rgba(212, 160, 79, 0.4); }
.menu-toggle { display: none; flex-direction: column; gap: 5px; cursor: pointer; padding: 8px; }
.menu-toggle span { display: block; width: 24px; height: 2px; background: var(--gold); transition: all 0.3s; }

.hero { min-height: 100vh; position: relative; display: flex; align-items: center; justify-content: center; text-align: center; overflow: hidden; padding: 7rem 2rem 4rem; }
.hero-slides { position: absolute; inset: 0; z-index: -2; }
.hero-slide { position: absolute; inset: 0; background-size: cover; background-position: center; opacity: 0; transition: opacity 1.2s ease-in-out; }
.hero-slide.active { opacity: 1; }
.hero-slide::after { content: ''; position: absolute; inset: 0; background: linear-gradient(180deg, rgba(10, 6, 4, 0.65) 0%, rgba(10, 6, 4, 0.88) 60%, var(--bg) 100%); }
.hero-slide-1 { background-image: url('https://images.unsplash.com/photo-1601050690597-df0568f70950?w=2400&auto=format&fit=crop&q=85'); }
.hero-slide-2 { background-image: url('https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=2400&auto=format&fit=crop&q=85'); }
.hero-slide-3 { background-image: url('https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=2400&auto=format&fit=crop&q=85'); }
.steam-container { position: absolute; inset: 0; z-index: -1; pointer-events: none; }
.steam { position: absolute; bottom: -50px; width: 6px; height: 6px; background: radial-gradient(circle, rgba(244, 233, 212, 0.3) 0%, transparent 70%); border-radius: 50%; filter: blur(2px); animation: rise linear infinite; }
@keyframes rise { 0% { transform: translateY(0) translateX(0) scale(1); opacity: 0; } 10% { opacity: 0.8; } 100% { transform: translateY(-100vh) translateX(40px) scale(3); opacity: 0; } }
.particle { position: absolute; width: 3px; height: 3px; background: var(--gold); border-radius: 50%; opacity: 0; animation: float 8s ease-in-out infinite; box-shadow: 0 0 8px var(--gold); }
@keyframes float { 0%, 100% { transform: translateY(0) translateX(0); opacity: 0; } 10% { opacity: 0.6; } 50% { transform: translateY(-30px) translateX(15px); opacity: 1; } 90% { opacity: 0.4; } }

.hero-content { position: relative; z-index: 1; }
.hero-eyebrow { display: inline-flex; align-items: center; gap: 1rem; color: var(--gold); font-size: 0.85rem; font-weight: 500; letter-spacing: 0.4em; text-transform: uppercase; margin-bottom: 2rem; }
.hero-eyebrow::before, .hero-eyebrow::after { content: ''; width: 50px; height: 1px; background: linear-gradient(90deg, transparent, var(--gold), transparent); }
.hero-urdu { font-family: 'Noto Nastaliq Urdu', serif; font-size: 1.4rem; color: var(--gold-light); margin-bottom: 1.5rem; }
.hero-text-track { position: relative; min-height: 18rem; margin-bottom: 1rem; }
.hero-text-slide { position: absolute; inset: 0; opacity: 0; transform: translateY(20px); transition: all 0.8s cubic-bezier(0.16, 1, 0.3, 1); pointer-events: none; }
.hero-text-slide.active { opacity: 1; transform: translateY(0); pointer-events: auto; }
.hero h1 { font-family: 'Cormorant Garamond', serif; font-size: clamp(3rem, 8vw, 6.5rem); line-height: 1; letter-spacing: -0.02em; font-weight: 400; margin-bottom: 1.25rem; max-width: 1100px; margin-left: auto; margin-right: auto; }
.hero h1 em { font-style: italic; background: linear-gradient(135deg, var(--gold-light) 0%, var(--saffron) 100%); -webkit-background-clip: text; background-clip: text; -webkit-text-fill-color: transparent; }
.hero-subtitle { font-family: 'Cormorant Garamond', serif; font-size: clamp(1.05rem, 1.6vw, 1.3rem); font-style: italic; color: var(--text-soft); max-width: 600px; margin: 0 auto 2rem; }
.hero-buttons { display: flex; gap: 1.25rem; justify-content: center; flex-wrap: wrap; position: relative; z-index: 2; }
.btn-primary { background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%); color: var(--bg); padding: 1.15rem 2.5rem; border-radius: 100px; font-size: 0.85rem; font-weight: 700; letter-spacing: 0.15em; text-transform: uppercase; transition: all 0.3s; display: inline-flex; align-items: center; gap: 0.6rem; box-shadow: 0 6px 30px rgba(212, 160, 79, 0.3); position: relative; overflow: hidden; }
.btn-primary::before { content: ''; position: absolute; top: 0; left: -100%; width: 100%; height: 100%; background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent); transition: left 0.6s; }
.btn-primary:hover { transform: translateY(-3px); box-shadow: 0 12px 40px rgba(212, 160, 79, 0.5); }
.btn-primary:hover::before { left: 100%; }
.btn-outline { border: 1px solid var(--gold); color: var(--gold); padding: 1.15rem 2.5rem; border-radius: 100px; font-size: 0.85rem; font-weight: 600; letter-spacing: 0.15em; text-transform: uppercase; transition: all 0.3s; display: inline-flex; align-items: center; gap: 0.6rem; }
.btn-outline:hover { background: rgba(212, 160, 79, 0.1); border-color: var(--gold-light); color: var(--gold-light); }
.carousel-dots { display: flex; gap: 0.6rem; justify-content: center; margin-top: 2.5rem; position: relative; z-index: 2; }
.carousel-dot { width: 8px; height: 8px; border-radius: 50%; background: rgba(212, 160, 79, 0.3); cursor: pointer; transition: all 0.3s; }
.carousel-dot.active { background: var(--gold); width: 32px; border-radius: 100px; }
.hero-stats { position: absolute; bottom: 2.5rem; left: 50%; transform: translateX(-50%); display: flex; gap: 1.25rem; flex-wrap: wrap; justify-content: center; z-index: 2; }
.stat-pill { background: rgba(28, 16, 7, 0.6); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); border: 1px solid var(--border); padding: 0.7rem 1.3rem; border-radius: 100px; display: flex; align-items: center; gap: 0.6rem; font-size: 0.8rem; font-weight: 500; color: var(--cream); }
.stat-pill .icon { color: var(--gold); font-size: 1rem; }

section { padding: 6rem 0; position: relative; }
.section-eyebrow { display: inline-flex; align-items: center; gap: 1rem; color: var(--gold); font-size: 0.8rem; font-weight: 600; letter-spacing: 0.3em; text-transform: uppercase; margin-bottom: 1.5rem; }
.section-eyebrow::before { content: ''; width: 40px; height: 1px; background: var(--gold); }
.section-title { font-family: 'Cormorant Garamond', serif; font-size: clamp(2.5rem, 5vw, 4.5rem); line-height: 1.05; letter-spacing: -0.02em; margin-bottom: 1.5rem; font-weight: 400; max-width: 800px; }
.section-title em { font-style: italic; color: var(--gold); }
.section-subtitle { font-size: 1.1rem; color: var(--text-soft); max-width: 600px; margin-bottom: 4rem; line-height: 1.7; }

#menu { background: radial-gradient(circle at 20% 30%, rgba(212, 160, 79, 0.05) 0%, transparent 50%), radial-gradient(circle at 80% 70%, rgba(232, 137, 60, 0.04) 0%, transparent 50%), var(--bg); }
.menu-header { text-align: center; display: flex; flex-direction: column; align-items: center; margin-bottom: 3rem; }
.menu-header .section-title { max-width: 900px; }
.category-tabs { display: flex; gap: 0.6rem; justify-content: center; flex-wrap: wrap; margin-bottom: 4rem; }
.category-tab { padding: 0.75rem 1.5rem; background: var(--surface-solid); border: 1px solid var(--border); border-radius: 100px; color: var(--text-soft); font-size: 0.85rem; font-weight: 600; letter-spacing: 0.05em; text-transform: uppercase; cursor: pointer; transition: all 0.3s; }
.category-tab:hover { border-color: var(--border-bright); color: var(--cream); }
.category-tab.active { background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%); color: var(--bg); border-color: var(--gold); }
.category-banner { background: linear-gradient(90deg, var(--surface-solid) 0%, rgba(28, 16, 7, 0.5) 100%); border-left: 3px solid var(--gold); padding: 1.25rem 2rem; margin-bottom: 2.5rem; border-radius: 0 12px 12px 0; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 1rem; }
.category-banner h3 { font-family: 'Cormorant Garamond', serif; font-size: 2rem; font-weight: 500; color: var(--cream); }
.category-banner h3 em { font-style: italic; color: var(--gold); }
.category-banner-sub { color: var(--text-soft); font-size: 0.95rem; font-style: italic; }
.category-section { margin-bottom: 4rem; }
.menu-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 2rem; }
.menu-card { background: linear-gradient(180deg, var(--surface-solid) 0%, #14090a 100%); border: 1px solid var(--border); border-radius: 20px; overflow: hidden; transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1); position: relative; display: flex; flex-direction: column; }
.menu-card:hover { transform: translateY(-8px); border-color: var(--border-bright); box-shadow: 0 20px 60px rgba(212, 160, 79, 0.15); }
.menu-card-img { aspect-ratio: 4/3; background-size: cover; background-position: center; position: relative; overflow: hidden; transition: transform 0.6s; }
.menu-card-img::after { content: ''; position: absolute; inset: 0; background: linear-gradient(180deg, transparent 50%, rgba(10, 6, 4, 0.7) 100%); }
.menu-card:hover .menu-card-img { transform: scale(1.05); }
.badge { position: absolute; top: 1rem; left: 1rem; background: rgba(10, 6, 4, 0.85); backdrop-filter: blur(10px); -webkit-backdrop-filter: blur(10px); border: 1px solid var(--gold); color: var(--gold); padding: 0.4rem 0.9rem; border-radius: 100px; font-size: 0.7rem; font-weight: 700; letter-spacing: 0.15em; text-transform: uppercase; z-index: 2; }
.badge.signature { background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%); color: var(--bg); border: none; }
.badge.oos { background: rgba(120, 50, 50, 0.85); border-color: #c97070; color: #ffb3b3; }
.menu-card-content { padding: 1.75rem; display: flex; flex-direction: column; flex: 1; }
.menu-card-title { font-family: 'Cormorant Garamond', serif; font-size: 1.6rem; font-weight: 500; margin-bottom: 0.5rem; color: var(--cream); }
.menu-card-desc { color: var(--text-soft); font-size: 0.9rem; margin-bottom: 1.25rem; line-height: 1.6; flex: 1; }
.menu-card-footer { display: flex; justify-content: space-between; align-items: center; padding-top: 1.25rem; border-top: 1px solid var(--border); flex-wrap: wrap; gap: 0.75rem; }
.menu-card-footer .add-to-cart { margin-left: auto; }
.spice-meter { display: flex; gap: 3px; align-items: center; }
.chili { font-size: 0.85rem; filter: grayscale(1); opacity: 0.3; }
.chili.active { filter: none; opacity: 1; }
.menu-card-price { font-family: 'Cormorant Garamond', serif; font-size: 1.5rem; font-weight: 500; color: var(--gold); font-style: italic; }

#about { background: linear-gradient(180deg, var(--bg) 0%, #0d0805 100%); }
.story-grid { display: grid; grid-template-columns: 5fr 6fr; gap: 5rem; align-items: center; }
.story-images { position: relative; aspect-ratio: 4/5; }
.story-img { position: absolute; border-radius: 12px; overflow: hidden; box-shadow: 0 30px 60px rgba(0,0,0,0.5); background-size: cover; background-position: center; }
.story-img-1 { top: 0; left: 0; width: 70%; height: 60%; background-image: url('https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=800&auto=format&fit=crop&q=85'); }
.story-img-2 { bottom: 0; right: 0; width: 65%; height: 55%; background-image: url('https://images.unsplash.com/photo-1601050690597-df0568f70950?w=800&auto=format&fit=crop&q=85'); border: 6px solid var(--bg); }
.story-decoration { position: absolute; top: 50%; left: -2rem; font-family: 'Cormorant Garamond', serif; font-size: 10rem; font-style: italic; color: var(--gold); opacity: 0.06; line-height: 1; pointer-events: none; }
.story-content h2 em { font-style: italic; color: var(--gold); }
.story-content p { color: var(--text-soft); font-size: 1.05rem; margin-bottom: 1.25rem; line-height: 1.8; }
.story-quote { font-family: 'Cormorant Garamond', serif; font-style: italic; font-size: 1.4rem; color: var(--gold-light); border-left: 2px solid var(--gold); padding: 0.5rem 0 0.5rem 1.5rem; margin: 2rem 0; line-height: 1.5; }
.counters { display: grid; grid-template-columns: repeat(4, 1fr); gap: 2rem; margin-top: 5rem; padding: 3rem 0; border-top: 1px solid var(--border); border-bottom: 1px solid var(--border); }
.counter { text-align: center; }
.counter-num { font-family: 'Cormorant Garamond', serif; font-size: clamp(2.5rem, 4vw, 3.5rem); font-weight: 500; color: var(--gold); line-height: 1; margin-bottom: 0.5rem; }
.counter-label { font-size: 0.85rem; color: var(--text-soft); text-transform: uppercase; letter-spacing: 0.15em; }

#reviews { background: radial-gradient(circle at 50% 50%, rgba(212, 160, 79, 0.04) 0%, transparent 60%), var(--bg); text-align: center; }
#reviews .section-eyebrow, #reviews .section-title, #reviews .section-subtitle { margin-left: auto; margin-right: auto; }
#reviews .section-eyebrow { display: inline-flex; }
.reviews-track { position: relative; max-width: 900px; margin: 0 auto; height: 280px; }
.review-card { position: absolute; inset: 0; background: linear-gradient(180deg, var(--surface-solid) 0%, #14090a 100%); border: 1px solid var(--border); border-radius: 20px; padding: 3rem; opacity: 0; transition: all 0.6s cubic-bezier(0.16, 1, 0.3, 1); display: flex; flex-direction: column; justify-content: center; transform: scale(0.95); }
.review-card.active { opacity: 1; transform: scale(1); }
.review-stars { color: var(--gold); font-size: 1.2rem; letter-spacing: 0.2rem; margin-bottom: 1.5rem; }
.review-text { font-family: 'Cormorant Garamond', serif; font-size: clamp(1.2rem, 2vw, 1.6rem); font-style: italic; color: var(--cream); line-height: 1.5; margin-bottom: 2rem; }
.review-author { display: flex; align-items: center; justify-content: center; gap: 1rem; }
.review-avatar { width: 48px; height: 48px; border-radius: 50%; background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%); display: flex; align-items: center; justify-content: center; font-family: 'Cormorant Garamond', serif; font-weight: 700; color: var(--bg); font-size: 1.1rem; }
.review-name { font-weight: 600; color: var(--cream); font-size: 0.95rem; }
.review-meta { font-size: 0.8rem; color: var(--text-muted); margin-top: 2px; }
.review-dots { display: flex; gap: 0.6rem; justify-content: center; margin-top: 2rem; }
.review-dot { width: 8px; height: 8px; border-radius: 50%; background: var(--border); cursor: pointer; transition: all 0.3s; }
.review-dot.active { background: var(--gold); width: 28px; border-radius: 100px; }

/* LEAVE REVIEW FORM */
.review-form-wrap {
  max-width: 700px; margin: 5rem auto 0;
  background: linear-gradient(180deg, var(--surface-solid) 0%, #14090a 100%);
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 3rem;
  text-align: left;
}
.review-form-wrap h3 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 2rem; font-weight: 500;
  margin-bottom: 0.5rem; color: var(--cream);
  text-align: center;
}
.review-form-wrap h3 em { font-style: italic; color: var(--gold); }
.review-form-wrap .form-sub {
  text-align: center; color: var(--text-soft);
  margin-bottom: 2rem; font-size: 0.95rem;
}
.review-form { display: grid; gap: 1.25rem; }
.form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; }
.form-field { display: flex; flex-direction: column; gap: 0.5rem; }
.form-field label {
  font-size: 0.75rem; color: var(--gold);
  text-transform: uppercase; letter-spacing: 0.15em; font-weight: 600;
}
.form-field input, .form-field textarea {
  background: rgba(10, 6, 4, 0.6);
  border: 1px solid var(--border);
  border-radius: 10px;
  padding: 0.85rem 1rem;
  color: var(--cream);
  font-family: 'Manrope', sans-serif;
  font-size: 0.95rem;
  transition: border-color 0.2s;
}
.form-field input:focus, .form-field textarea:focus {
  outline: none; border-color: var(--gold);
}
.form-field textarea { resize: vertical; min-height: 100px; }
.star-rating {
  display: flex; gap: 0.4rem; align-items: center;
}
.star-rating .star {
  font-size: 1.6rem; color: var(--text-muted);
  cursor: pointer; transition: color 0.2s;
}
.star-rating .star.active, .star-rating .star:hover { color: var(--gold); }
.review-form button {
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg); padding: 1rem 2rem; border-radius: 100px;
  font-size: 0.85rem; font-weight: 700;
  letter-spacing: 0.15em; text-transform: uppercase;
  cursor: pointer; transition: all 0.3s;
  margin-top: 0.5rem;
}
.review-form button:hover { transform: translateY(-2px); box-shadow: 0 8px 30px rgba(212, 160, 79, 0.4); }
.review-success {
  display: none;
  background: rgba(40, 100, 50, 0.15);
  border: 1px solid rgba(80, 180, 100, 0.3);
  color: #b3e8c0;
  padding: 1.5rem; border-radius: 12px;
  text-align: center; margin-top: 1rem;
  font-style: italic;
}
.review-success.show { display: block; }

/* ============================================
   ORDERING SYSTEM — CART, CHECKOUT, SUCCESS
   ============================================ */

/* Add to Cart button on menu cards */
.add-to-cart {
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  padding: 0.5rem 1rem;
  border-radius: 100px;
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.2s;
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
}
.add-to-cart:hover { transform: translateY(-2px); box-shadow: 0 6px 20px rgba(212, 160, 79, 0.4); }
.add-to-cart.added { background: rgba(80, 180, 100, 0.9); color: white; }

/* Floating Cart Button */
.cart-fab {
  position: fixed;
  bottom: 2rem;
  left: 2rem;
  z-index: 99;
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  border-radius: 100px;
  padding: 0.9rem 1.5rem;
  display: flex;
  align-items: center;
  gap: 0.6rem;
  font-weight: 700;
  font-size: 0.85rem;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  cursor: pointer;
  box-shadow: 0 8px 30px rgba(212, 160, 79, 0.4);
  transition: all 0.3s;
  opacity: 0;
  transform: translateY(20px);
  pointer-events: none;
}
.cart-fab.visible { opacity: 1; transform: translateY(0); pointer-events: auto; }
.cart-fab:hover { transform: translateY(-3px) scale(1.02); }
.cart-count-badge {
  background: var(--bg);
  color: var(--gold);
  border-radius: 100px;
  padding: 0.15rem 0.55rem;
  font-size: 0.75rem;
  font-weight: 700;
}
.cart-fab svg { width: 18px; height: 18px; fill: var(--bg); }

/* Cart Drawer */
.cart-overlay {
  position: fixed; inset: 0;
  background: rgba(10, 6, 4, 0.7);
  backdrop-filter: blur(6px);
  -webkit-backdrop-filter: blur(6px);
  z-index: 1000;
  opacity: 0;
  pointer-events: none;
  transition: opacity 0.3s;
}
.cart-overlay.open { opacity: 1; pointer-events: auto; }

.cart-drawer {
  position: fixed;
  top: 0; right: 0; bottom: 0;
  width: 440px; max-width: 100vw;
  background: linear-gradient(180deg, #14090a 0%, #0a0604 100%);
  border-left: 1px solid var(--border);
  z-index: 1001;
  display: flex; flex-direction: column;
  transform: translateX(100%);
  transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1);
}
.cart-drawer.open { transform: translateX(0); }

.cart-header {
  padding: 1.5rem 2rem;
  border-bottom: 1px solid var(--border);
  display: flex; justify-content: space-between; align-items: center;
}
.cart-header h3 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.6rem; font-weight: 500;
  color: var(--cream);
}
.cart-header h3 em { font-style: italic; color: var(--gold); }
.cart-close {
  background: rgba(212, 160, 79, 0.1);
  color: var(--gold);
  border-radius: 50%;
  width: 36px; height: 36px;
  display: flex; align-items: center; justify-content: center;
  font-size: 1.2rem; cursor: pointer;
  transition: all 0.2s;
}
.cart-close:hover { background: rgba(212, 160, 79, 0.2); }

.cart-items {
  flex: 1; overflow-y: auto;
  padding: 1.5rem 2rem;
}
.cart-empty {
  text-align: center;
  padding: 4rem 1rem;
  color: var(--text-soft);
}
.cart-empty .icon { font-size: 3rem; opacity: 0.3; margin-bottom: 1rem; }
.cart-empty h4 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.3rem; color: var(--cream); margin-bottom: 0.5rem;
}

.cart-item {
  display: flex; gap: 1rem;
  padding: 1rem 0;
  border-bottom: 1px solid var(--border);
}
.cart-item-img {
  width: 70px; height: 70px;
  border-radius: 10px;
  background-size: cover; background-position: center;
  flex-shrink: 0;
}
.cart-item-content { flex: 1; display: flex; flex-direction: column; gap: 0.35rem; }
.cart-item-name {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.1rem; color: var(--cream);
  font-weight: 500;
}
.cart-item-price {
  color: var(--gold); font-size: 0.9rem;
  font-style: italic;
}
.cart-item-controls {
  display: flex; align-items: center; gap: 0.75rem; margin-top: 0.4rem;
}
.qty-btn {
  width: 26px; height: 26px;
  background: rgba(212, 160, 79, 0.1);
  border: 1px solid var(--border);
  color: var(--gold);
  border-radius: 50%;
  font-size: 0.95rem; cursor: pointer;
  display: flex; align-items: center; justify-content: center;
  transition: all 0.2s;
}
.qty-btn:hover { background: rgba(212, 160, 79, 0.25); }
.qty-value {
  font-size: 0.9rem; color: var(--cream);
  min-width: 20px; text-align: center;
}
.cart-item-remove {
  background: none; color: var(--text-muted);
  font-size: 0.75rem; cursor: pointer;
  margin-left: auto; text-decoration: underline;
  transition: color 0.2s;
}
.cart-item-remove:hover { color: #c97070; }

.cart-footer {
  padding: 1.5rem 2rem;
  border-top: 1px solid var(--border);
  background: rgba(10, 6, 4, 0.5);
}
.cart-totals { margin-bottom: 1.25rem; }
.cart-row {
  display: flex; justify-content: space-between;
  margin-bottom: 0.6rem;
  font-size: 0.9rem;
  color: var(--text-soft);
}
.cart-row.total {
  font-size: 1.1rem;
  font-weight: 600;
  color: var(--cream);
  border-top: 1px solid var(--border);
  padding-top: 0.75rem;
  margin-top: 0.75rem;
  margin-bottom: 0;
}
.cart-row.total .amount {
  color: var(--gold);
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.4rem;
  font-style: italic;
}
.checkout-btn {
  width: 100%;
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  padding: 1.1rem;
  border-radius: 100px;
  font-size: 0.85rem; font-weight: 700;
  letter-spacing: 0.15em; text-transform: uppercase;
  cursor: pointer; transition: all 0.3s;
}
.checkout-btn:hover { transform: translateY(-2px); box-shadow: 0 8px 25px rgba(212, 160, 79, 0.4); }
.checkout-btn:disabled { opacity: 0.5; cursor: not-allowed; transform: none; box-shadow: none; }

/* Demo Banner inside cart */
.demo-banner {
  background: rgba(232, 137, 60, 0.1);
  border: 1px solid rgba(232, 137, 60, 0.3);
  border-radius: 10px;
  padding: 0.85rem 1rem;
  color: var(--gold-light);
  font-size: 0.78rem;
  margin: 1rem 2rem;
  font-style: italic;
  text-align: center;
}

/* Checkout Modal */
.checkout-modal {
  position: fixed; inset: 0;
  background: rgba(10, 6, 4, 0.85);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  z-index: 1100;
  display: none;
  align-items: flex-start;
  justify-content: center;
  padding: 2rem 1rem;
  overflow-y: auto;
}
.checkout-modal.open { display: flex; }
.checkout-box {
  background: linear-gradient(180deg, #14090a 0%, #0a0604 100%);
  border: 1px solid var(--border);
  border-radius: 20px;
  max-width: 600px; width: 100%;
  padding: 2.5rem;
  margin: auto;
}
.checkout-box h3 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.8rem; color: var(--cream);
  margin-bottom: 0.5rem;
  font-weight: 500;
}
.checkout-box h3 em { font-style: italic; color: var(--gold); }
.checkout-box .form-sub { color: var(--text-soft); margin-bottom: 2rem; font-size: 0.9rem; }

.order-type-grid {
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 0.75rem; margin-bottom: 0.5rem;
}
.order-type-btn {
  padding: 1rem;
  background: rgba(10, 6, 4, 0.6);
  border: 1px solid var(--border);
  border-radius: 12px;
  color: var(--text-soft);
  font-size: 0.85rem; font-weight: 600;
  letter-spacing: 0.05em; text-transform: uppercase;
  cursor: pointer; transition: all 0.2s;
  display: flex; flex-direction: column; align-items: center; gap: 0.4rem;
}
.order-type-btn .icon { font-size: 1.4rem; color: var(--gold); }
.order-type-btn.active { border-color: var(--gold); background: rgba(212, 160, 79, 0.1); color: var(--cream); }

.delivery-fields { display: none; }
.delivery-fields.show { display: grid; gap: 1rem; }

.checkout-actions { display: flex; gap: 0.75rem; margin-top: 1.5rem; }
.btn-back {
  flex: 1;
  background: transparent;
  border: 1px solid var(--border);
  color: var(--text-soft);
  padding: 1rem;
  border-radius: 100px;
  font-size: 0.8rem; font-weight: 600;
  letter-spacing: 0.1em; text-transform: uppercase;
  cursor: pointer; transition: all 0.2s;
}
.btn-back:hover { border-color: var(--gold); color: var(--gold); }
.btn-confirm {
  flex: 2;
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  padding: 1rem;
  border-radius: 100px;
  font-size: 0.85rem; font-weight: 700;
  letter-spacing: 0.15em; text-transform: uppercase;
  cursor: pointer; transition: all 0.3s;
}
.btn-confirm:hover { transform: translateY(-2px); box-shadow: 0 8px 25px rgba(212, 160, 79, 0.4); }

/* Order Success Screen */
.success-modal {
  position: fixed; inset: 0;
  background: rgba(10, 6, 4, 0.95);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  z-index: 1200;
  display: none;
  align-items: center;
  justify-content: center;
  padding: 2rem;
  overflow-y: auto;
}
.success-modal.open { display: flex; }
.success-box {
  background: linear-gradient(180deg, #14090a 0%, #0a0604 100%);
  border: 1px solid var(--gold);
  border-radius: 20px;
  max-width: 520px; width: 100%;
  padding: 3rem 2.5rem;
  text-align: center;
  box-shadow: 0 20px 80px rgba(212, 160, 79, 0.2);
  margin: auto;
}
.success-check {
  width: 80px; height: 80px;
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  margin: 0 auto 1.5rem;
  font-size: 2.5rem; color: var(--bg);
  font-weight: 700;
  box-shadow: 0 8px 30px rgba(212, 160, 79, 0.4);
}
.success-box h3 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 2rem; color: var(--cream);
  margin-bottom: 0.5rem; font-weight: 500;
}
.success-box h3 em { font-style: italic; color: var(--gold); }
.success-box .order-no {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.6rem; color: var(--gold);
  font-style: italic; margin: 1rem 0;
  letter-spacing: 0.05em;
}
.success-box .summary {
  background: rgba(10, 6, 4, 0.5);
  border-radius: 12px;
  padding: 1.25rem;
  margin: 1.5rem 0;
  text-align: left;
  font-size: 0.9rem;
}
.success-box .summary-row {
  display: flex; justify-content: space-between;
  margin-bottom: 0.5rem; color: var(--text-soft);
}
.success-box .summary-row strong { color: var(--cream); }
.success-eta {
  color: var(--gold-light);
  font-style: italic;
  font-size: 0.95rem;
  margin: 1rem 0 1.5rem;
}
.demo-warning {
  background: rgba(232, 137, 60, 0.12);
  border: 1px solid rgba(232, 137, 60, 0.4);
  border-radius: 12px;
  padding: 1rem 1.25rem;
  color: var(--gold-light);
  font-size: 0.85rem;
  margin: 1.5rem 0;
  font-style: italic;
  line-height: 1.5;
  text-align: left;
}
.demo-warning strong { display: block; color: var(--cream); font-style: normal; margin-bottom: 0.4rem; letter-spacing: 0.1em; text-transform: uppercase; font-size: 0.75rem; }
.success-close {
  background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%);
  color: var(--bg);
  padding: 0.9rem 2rem;
  border-radius: 100px;
  font-size: 0.85rem; font-weight: 700;
  letter-spacing: 0.15em; text-transform: uppercase;
  cursor: pointer; transition: all 0.3s;
}
.success-close:hover { transform: translateY(-2px); }

@media (max-width: 600px) {
  .cart-drawer { width: 100%; }
  .cart-header, .cart-items, .cart-footer { padding-left: 1.25rem; padding-right: 1.25rem; }
  .demo-banner { margin: 1rem 1.25rem; }
  .checkout-box { padding: 2rem 1.5rem; }
  .success-box { padding: 2.5rem 1.5rem; }
  .order-type-grid { grid-template-columns: 1fr; }
  .cart-fab { bottom: 1.25rem; left: 1.25rem; padding: 0.75rem 1.1rem; font-size: 0.78rem; }
}

#locations { background: var(--bg); }
.locations-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; }
.location-card { background: linear-gradient(180deg, var(--surface-solid) 0%, #14090a 100%); border: 1px solid var(--border); border-radius: 20px; overflow: hidden; transition: all 0.3s; }
.location-card:hover { border-color: var(--border-bright); transform: translateY(-4px); }
.location-map { aspect-ratio: 16/9; background: #1a0f08; position: relative; overflow: hidden; }
.location-map iframe { width: 100%; height: 100%; border: 0; filter: invert(0.85) hue-rotate(180deg) saturate(0.5) brightness(0.7); }
.location-content { padding: 2.5rem; }
.location-badge { display: inline-block; background: rgba(212, 160, 79, 0.1); color: var(--gold); padding: 0.3rem 0.8rem; border-radius: 100px; font-size: 0.7rem; font-weight: 700; letter-spacing: 0.2em; text-transform: uppercase; margin-bottom: 1rem; }
.location-name { font-family: 'Cormorant Garamond', serif; font-size: 2rem; font-weight: 500; margin-bottom: 1rem; color: var(--cream); }
.location-info { color: var(--text-soft); margin-bottom: 0.75rem; display: flex; align-items: flex-start; gap: 0.75rem; font-size: 0.95rem; }
.location-info .icon { color: var(--gold); flex-shrink: 0; margin-top: 0.15rem; }
.location-buttons { display: flex; gap: 0.75rem; margin-top: 2rem; }
.btn-location { flex: 1; padding: 0.9rem; border-radius: 100px; font-size: 0.8rem; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; text-align: center; transition: all 0.2s; }
.btn-location.primary { background: linear-gradient(135deg, var(--gold) 0%, var(--saffron) 100%); color: var(--bg); }
.btn-location.secondary { border: 1px solid var(--gold); color: var(--gold); }
.btn-location:hover { transform: translateY(-2px); }

.whatsapp-float { position: fixed; bottom: 2rem; right: 2rem; z-index: 99; width: 60px; height: 60px; background: #25d366; border-radius: 50%; display: flex; align-items: center; justify-content: center; box-shadow: 0 8px 30px rgba(37, 211, 102, 0.4); animation: pulse-wa 2s infinite; transition: all 0.3s; }
.whatsapp-float:hover { transform: scale(1.1); }
@keyframes pulse-wa { 0%, 100% { box-shadow: 0 8px 30px rgba(37, 211, 102, 0.4); } 50% { box-shadow: 0 8px 30px rgba(37, 211, 102, 0.4), 0 0 0 12px rgba(37, 211, 102, 0); } }
.whatsapp-float svg { width: 32px; height: 32px; fill: white; }

footer { background: linear-gradient(180deg, var(--bg) 0%, #060402 100%); padding: 5rem 0 2rem; position: relative; overflow: hidden; border-top: 1px solid var(--border); }
.skyline { position: absolute; bottom: 0; left: 0; right: 0; height: 80px; background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1200 80' preserveAspectRatio='none'%3E%3Cpath fill='%23d4a04f' fill-opacity='0.08' d='M0 80 L0 50 L40 50 L40 30 L60 30 L60 50 L100 50 L100 20 L120 20 L120 10 L140 10 L140 20 L160 20 L160 50 L200 50 L200 35 L220 35 L220 15 L240 15 L240 35 L260 35 L260 50 L300 50 L300 25 L340 25 L340 50 L380 50 L380 30 L400 30 L400 5 L420 5 L420 30 L440 30 L440 50 L480 50 L480 40 L520 40 L520 20 L540 20 L540 40 L580 40 L580 50 L620 50 L620 25 L640 25 L640 10 L660 10 L660 25 L680 25 L680 50 L720 50 L720 35 L760 35 L760 15 L780 15 L780 35 L800 35 L800 50 L840 50 L840 30 L860 30 L860 50 L900 50 L900 20 L940 20 L940 50 L980 50 L980 40 L1020 40 L1020 25 L1040 25 L1040 5 L1060 5 L1060 25 L1080 25 L1080 50 L1120 50 L1120 35 L1160 35 L1160 50 L1200 50 L1200 80 Z'/%3E%3C/svg%3E"); background-size: 100% 100%; pointer-events: none; }
.footer-content { position: relative; z-index: 2; display: grid; grid-template-columns: 1.5fr 1fr 1fr 1fr; gap: 3rem; margin-bottom: 4rem; }
.footer-brand .logo { margin-bottom: 1.5rem; }
.footer-tagline { font-family: 'Cormorant Garamond', serif; font-style: italic; font-size: 1.2rem; color: var(--text-soft); margin-bottom: 1.5rem; line-height: 1.5; }
.footer-urdu { font-family: 'Noto Nastaliq Urdu', serif; color: var(--gold); font-size: 1.3rem; margin-bottom: 1rem; }
.footer-col h4 { font-family: 'Cormorant Garamond', serif; font-size: 1.2rem; color: var(--cream); margin-bottom: 1.5rem; font-weight: 500; }
.footer-col ul { list-style: none; }
.footer-col li { margin-bottom: 0.6rem; }
.footer-col a { color: var(--text-soft); font-size: 0.9rem; transition: color 0.2s; }
.footer-col a:hover { color: var(--gold); }
.footer-bottom { display: flex; justify-content: space-between; align-items: center; padding-top: 2rem; border-top: 1px solid var(--border); position: relative; z-index: 2; flex-wrap: wrap; gap: 1rem; }
.footer-bottom-text { color: var(--text-muted); font-size: 0.85rem; }
.social-row { display: flex; gap: 0.75rem; }
.social-icon { width: 36px; height: 36px; border: 1px solid var(--border); border-radius: 50%; display: flex; align-items: center; justify-content: center; color: var(--text-soft); transition: all 0.3s; font-size: 0.95rem; }
.social-icon:hover { background: var(--gold); color: var(--bg); border-color: var(--gold); }
.disclaimer { text-align: center; font-size: 0.75rem; color: var(--text-muted); margin-top: 2rem; font-style: italic; opacity: 0.7; }
.disclaimer a { color: var(--gold); }

@media (max-width: 968px) {
  .nav-links { display: none; }
  .menu-toggle { display: flex; }
  .nav-links.open { display: flex; flex-direction: column; position: fixed; top: 70px; left: 0; right: 0; background: rgba(10, 6, 4, 0.98); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); padding: 2rem; gap: 1.5rem; border-bottom: 1px solid var(--border); }
  .hero-stats { position: relative; bottom: auto; transform: none; margin-top: 2rem; }
  .menu-grid { grid-template-columns: 1fr 1fr; }
  .story-grid { grid-template-columns: 1fr; gap: 3rem; }
  .counters { grid-template-columns: repeat(2, 1fr); gap: 1.5rem; }
  .locations-grid { grid-template-columns: 1fr; }
  .footer-content { grid-template-columns: 1fr 1fr; }
  section { padding: 4rem 0; }
}
@media (max-width: 600px) {
  nav { padding: 1rem 1.25rem; }
  .container { padding: 0 1.25rem; }
  .menu-grid { grid-template-columns: 1fr; }
  .footer-content { grid-template-columns: 1fr; }
  .footer-bottom { flex-direction: column; text-align: center; }
  .whatsapp-float { bottom: 1.25rem; right: 1.25rem; width: 52px; height: 52px; }
  .whatsapp-float svg { width: 26px; height: 26px; }
  .reviews-track { height: 360px; }
  .review-card { padding: 2rem 1.5rem; }
  .story-decoration { display: none; }
  .category-banner { padding: 1rem 1.25rem; }
  .category-banner h3 { font-size: 1.5rem; }
  .review-form-wrap { padding: 2rem 1.5rem; }
  .form-row { grid-template-columns: 1fr; }
}
</style>
</head>
<body>

<nav>
  <div class="logo">
    <div class="logo-mark">J</div>
    <div class="logo-text">Javed <em>Nihari</em></div>
  </div>
  <ul class="nav-links" id="navLinks">
    <li><a href="#hero">Home</a></li>
    <li><a href="#menu">Menu</a></li>
    <li><a href="#about">Story</a></li>
    <li><a href="#reviews">Reviews</a></li>
    <li><a href="#locations">Locations</a></li>
  </ul>
  <a href="#menu" class="nav-cta">Order Now</a>
  <div class="menu-toggle" onclick="document.getElementById('navLinks').classList.toggle('open')">
    <span></span><span></span><span></span>
  </div>
</nav>

<section class="hero" id="hero">
  <div class="hero-slides">
    <div class="hero-slide hero-slide-1 active"></div>
    <div class="hero-slide hero-slide-2"></div>
    <div class="hero-slide hero-slide-3"></div>
  </div>
  <div class="steam-container" id="steamContainer"></div>
  <div class="container">
    <div class="hero-content">
      <div class="hero-eyebrow">Est. 1985 · Karachi</div>
      <div class="hero-urdu">لذتِ روایت</div>
      <div class="hero-text-track">
        <div class="hero-text-slide active">
          <h1>Karachi's Most<br><em>Legendary</em> Nihari</h1>
          <p class="hero-subtitle">Slow-cooked tradition served for generations. Every plate tells a story that began on the streets of old Karachi.</p>
        </div>
        <div class="hero-text-slide">
          <h1>Forty Years of<br><em>Tradition</em></h1>
          <p class="hero-subtitle">Hand-ground spices. Eight-hour simmer. The original recipe, unchanged since 1985.</p>
        </div>
        <div class="hero-text-slide">
          <h1>Order Online,<br><em>Delivered Hot</em></h1>
          <p class="hero-subtitle">Home delivery across Karachi. From our kitchen to your table in 45 minutes.</p>
        </div>
      </div>
      <div class="hero-buttons">
        <a href="#menu" class="btn-primary">Explore Menu →</a>
        <a href="#locations" class="btn-outline">Find a Branch</a>
      </div>
      <div class="carousel-dots" id="carouselDots">
        <div class="carousel-dot active" data-slide="0"></div>
        <div class="carousel-dot" data-slide="1"></div>
        <div class="carousel-dot" data-slide="2"></div>
      </div>
    </div>
  </div>
  <div class="hero-stats">
    <div class="stat-pill"><span class="icon">★</span> 40+ Years Legacy</div>
    <div class="stat-pill"><span class="icon">◆</span> 10,000+ Reviews</div>
    <div class="stat-pill"><span class="icon">♛</span> Karachi Icon</div>
    <div class="stat-pill"><span class="icon">✦</span> Authentic Specialists</div>
  </div>
</section>

<section id="menu">
  <div class="container">
    <div class="menu-header">
      <div class="section-eyebrow">The Menu</div>
      <h2 class="section-title">Recipes <em>slow-cooked</em> through generations.</h2>
      <p class="section-subtitle" style="text-align: center; margin: 0 auto 0;">Every dish on our menu has been perfected over four decades. Browse by category.</p>
    </div>
    <div class="category-tabs">
      <button class="category-tab active" data-cat="all">All</button>
      <button class="category-tab" data-cat="nihari">Nihari</button>
      <button class="category-tab" data-cat="haleem">Haleem</button>
      <button class="category-tab" data-cat="biryani">Biryani &amp; Pulao</button>
      <button class="category-tab" data-cat="tandoor">Tandoor</button>
      <button class="category-tab" data-cat="drinks">Soft Drinks</button>
      <button class="category-tab" data-cat="tin">Tin Pack</button>
      <button class="category-tab" data-cat="desserts">Desserts</button>
    </div>

    <div class="category-section" data-cat="nihari">
      <div class="category-banner"><h3>Our <em>Signature</em> Nihari</h3><span class="category-banner-sub">Slow-cooked overnight. Seven cuts, one tradition.</span></div>
      <div class="menu-grid">
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=800&auto=format&fit=crop&q=85');"><div class="badge signature">Most Popular</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Nihari</h3><p class="menu-card-desc">The classic. Tender beef in slow-simmered gravy with our signature 18-spice blend. Single Rs. 500 · Double Rs. 1,000.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 500</div>
              <button class="add-to-cart" onclick="addToCart('Nihari', 500, 'https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=800&auto=format&fit=crop&q=85');"><div class="badge">Bone Marrow</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Nalli Nihari</h3><p class="menu-card-desc">Bone-in cuts release a velvety depth — rich, indulgent, deeply flavorful. Single Rs. 800 · Double Rs. 1,400.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 800</div>
              <button class="add-to-cart" onclick="addToCart('Nalli Nihari', 800, 'https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1574484284002-952d92456975?w=800&auto=format&fit=crop&q=85');"><div class="badge">Connoisseur</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Maghaz Nihari</h3><p class="menu-card-desc">Brain masala served alongside our signature gravy — a delicacy for purists. Single Rs. 900 · Double Rs. 1,400.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span></div><div class="menu-card-price">From PKR 900</div>
              <button class="add-to-cart" onclick="addToCart('Maghaz Nihari', 900, 'https://images.unsplash.com/photo-1574484284002-952d92456975?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1546833999-b9f581a1996d?w=800&auto=format&fit=crop&q=85');"><div class="badge signature">Chef's Special</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Special Nihari</h3><p class="menu-card-desc">Our premium house special — selected cuts in a deeper, more luxurious gravy. Single Rs. 1,150 · Double Rs. 1,750.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 1,150</div>
              <button class="add-to-cart" onclick="addToCart('Special Nihari', 1150, 'https://images.unsplash.com/photo-1546833999-b9f581a1996d?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1599487488170-d11ec9c172f0?w=800&auto=format&fit=crop&q=85');"><div class="badge">Premium Fry</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Special Nihari Fry</h3><p class="menu-card-desc">Our special nihari with the meat lightly fried for added char and texture. Single Rs. 1,250 · Double Rs. 1,950.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span></div><div class="menu-card-price">From PKR 1,250</div>
              <button class="add-to-cart" onclick="addToCart('Special Nihari Fry', 1250, 'https://images.unsplash.com/photo-1599487488170-d11ec9c172f0?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1567337710282-00832b415979?w=800&auto=format&fit=crop&q=85');"><div class="badge">Boneless</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Boti Nihari</h3><p class="menu-card-desc">Premium boneless cuts only — pure tender beef in rich gravy. Half Rs. 1,800 · Full Rs. 3,000.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 1,800</div>
              <button class="add-to-cart" onclick="addToCart('Boti Nihari', 1800, 'https://images.unsplash.com/photo-1567337710282-00832b415979?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1626777552726-4a6b54c97e46?w=800&auto=format&fit=crop&q=85');"><div class="badge">Big Bone</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Nihari Bong</h3><p class="menu-card-desc">Whole bone-in piece with rich marrow — the most generous serving on our menu. Half Rs. 1,800 · Full Rs. 3,000.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 1,800</div>
              <button class="add-to-cart" onclick="addToCart('Nihari Bong', 1800, 'https://images.unsplash.com/photo-1626777552726-4a6b54c97e46?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
      </div>
    </div>

    <div class="category-section" data-cat="haleem">
      <div class="category-banner"><h3>Slow-cooked <em>Haleem</em></h3><span class="category-banner-sub">Lentils, wheat, and tender meat — simmered for hours.</span></div>
      <div class="menu-grid">
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Beef Haleem</h3><p class="menu-card-desc">Slow-cooked wheat, lentils, and beef — finished with fried onions, mint, and lemon.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 250</div>
              <button class="add-to-cart" onclick="addToCart('Beef Haleem', 250, 'https://images.unsplash.com/photo-1606491956689-2ea866880c84?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1631292784640-2b24be784d5d?w=800&auto=format&fit=crop&q=85');"><div class="badge oos">Out of Stock</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Chicken Haleem</h3><p class="menu-card-desc">A lighter haleem made with shredded chicken — same depth, gentler richness.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 200</div></div></div>
        </div>
      </div>
    </div>

    <div class="category-section" data-cat="biryani">
      <div class="category-banner"><h3>Biryani &amp; <em>Pulao</em></h3><span class="category-banner-sub">Aromatic basmati layered with our family's spice blend.</span></div>
      <div class="menu-grid">
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1631452180519-c014fe946bc7?w=800&auto=format&fit=crop&q=85');"><div class="badge">Most Popular</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Chicken Biryani</h3><p class="menu-card-desc">Layered basmati with marinated chicken, potatoes, and our 23-spice blend. Served with raita.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 320</div>
              <button class="add-to-cart" onclick="addToCart('Chicken Biryani', 320, 'https://images.unsplash.com/photo-1631452180519-c014fe946bc7?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1589302168068-964664d93dc0?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Chicken Pulao</h3><p class="menu-card-desc">A milder, more delicate rice dish — chicken cooked into the rice with whole spices.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 320</div>
              <button class="add-to-cart" onclick="addToCart('Chicken Pulao', 320, 'https://images.unsplash.com/photo-1589302168068-964664d93dc0?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1563379091339-03b21ab4a4f8?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Beef Pulao</h3><p class="menu-card-desc">Slow-cooked beef yakhni-style — basmati rice steeped in deep meaty broth.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 400</div>
              <button class="add-to-cart" onclick="addToCart('Beef Pulao', 400, 'https://images.unsplash.com/photo-1563379091339-03b21ab4a4f8?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
      </div>
    </div>

    <div class="category-section" data-cat="tandoor">
      <div class="category-banner"><h3>From the <em>Tandoor</em></h3><span class="category-banner-sub">Fresh-baked breads from our clay oven.</span></div>
      <div class="menu-grid">
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1565557623262-b51c2513a641?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Roti</h3><p class="menu-card-desc">Classic tandoori roti — crispy edges, pillowy center. The essential pairing for nihari.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 30</div>
              <button class="add-to-cart" onclick="addToCart('Roti', 30, 'https://images.unsplash.com/photo-1565557623262-b51c2513a641?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1573821663912-6df460f9c684?w=800&auto=format&fit=crop&q=85');"><div class="badge">Specialty</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Dhoot Wali Roti</h3><p class="menu-card-desc">A thicker, milk-enriched tandoori roti — heartier than the standard naan.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 50</div>
              <button class="add-to-cart" onclick="addToCart('Dhoot Wali Roti', 50, 'https://images.unsplash.com/photo-1573821663912-6df460f9c684?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1568901346375-23c9450c58cd?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Sheermal</h3><p class="menu-card-desc">Sweet saffron-infused flatbread, baked golden. A traditional Mughal-era pairing.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 80</div>
              <button class="add-to-cart" onclick="addToCart('Sheermal', 80, 'https://images.unsplash.com/photo-1568901346375-23c9450c58cd?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1612809076216-69a44f9bba14?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Taftan</h3><p class="menu-card-desc">A puffy, slightly sweet leavened bread — fragrant with cardamom and rose.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 80</div>
              <button class="add-to-cart" onclick="addToCart('Taftan', 80, 'https://images.unsplash.com/photo-1612809076216-69a44f9bba14?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
      </div>
    </div>

    <div class="category-section" data-cat="drinks">
      <div class="category-banner"><h3>Soft <em>Drinks</em></h3><span class="category-banner-sub">The perfect cool finish after a spicy meal.</span></div>
      <div class="menu-grid">
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1622483767028-3f66f32aef97?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Soft Drink Can</h3><p class="menu-card-desc">Chilled 345ml can — Pepsi, 7Up, or Mirinda.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 80</div>
              <button class="add-to-cart" onclick="addToCart('Soft Drink Can', 80, 'https://images.unsplash.com/photo-1622483767028-3f66f32aef97?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1543253687-c931c8e01820?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Small Bottle</h3><p class="menu-card-desc">500ml soft drink bottle, perfect for individual servings.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 50</div>
              <button class="add-to-cart" onclick="addToCart('Small Bottle', 50, 'https://images.unsplash.com/photo-1543253687-c931c8e01820?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1581636625402-29b2a704ef13?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">1.5L Bottle</h3><p class="menu-card-desc">Family-sized 1.5L soft drink for the whole table.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 100</div>
              <button class="add-to-cart" onclick="addToCart('1.5L Bottle', 100, 'https://images.unsplash.com/photo-1581636625402-29b2a704ef13?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1564419320461-6870880221ad?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Mineral Water</h3><p class="menu-card-desc">Chilled bottled drinking water. Available in 500ml and 1.5L sizes.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 60</div>
              <button class="add-to-cart" onclick="addToCart('Mineral Water', 60, 'https://images.unsplash.com/photo-1564419320461-6870880221ad?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
      </div>
    </div>

    <div class="category-section" data-cat="tin">
      <div class="category-banner"><h3>Tin <em>Pack</em></h3><span class="category-banner-sub">Take the legacy home. Perfect for travel and gifting.</span></div>
      <div class="menu-grid">
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1599909366516-6c1bba8e0d99?w=800&auto=format&fit=crop&q=85');"><div class="badge signature">Best Seller</div></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Nihari Tin Pack</h3><p class="menu-card-desc">900g sealed tin of our signature nihari — ready to heat, ready to enjoy. Loved by overseas Pakistanis.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 1,400</div>
              <button class="add-to-cart" onclick="addToCart('Nihari Tin Pack', 1400, 'https://images.unsplash.com/photo-1599909366516-6c1bba8e0d99?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1626777552726-4a6b54c97e46?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Beef Haleem Tin Pack</h3><p class="menu-card-desc">900g sealed tin of slow-cooked beef haleem. Travel-friendly. 12-month shelf life.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili active">🌶</span><span class="chili active">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 1,200</div>
              <button class="add-to-cart" onclick="addToCart('Beef Haleem Tin Pack', 1200, 'https://images.unsplash.com/photo-1626777552726-4a6b54c97e46?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
      </div>
    </div>

    <div class="category-section" data-cat="desserts">
      <div class="category-banner"><h3>Sweet <em>Endings</em></h3><span class="category-banner-sub">Traditional Pakistani desserts to close the meal.</span></div>
      <div class="menu-grid">
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1605197181344-d34b5e4d4147?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Kheer</h3><p class="menu-card-desc">Creamy rice pudding with cardamom and pistachios — by the pyala or in a larger portion.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 100</div>
              <button class="add-to-cart" onclick="addToCart('Kheer', 100, 'https://images.unsplash.com/photo-1605197181344-d34b5e4d4147?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1551024506-0bccd828d307?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Rabri</h3><p class="menu-card-desc">Slow-reduced sweetened milk, garnished with saffron. By the pyala or by the kilo (Rs. 1,400/kg).</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">From PKR 180</div>
              <button class="add-to-cart" onclick="addToCart('Rabri', 180, 'https://images.unsplash.com/photo-1551024506-0bccd828d307?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
        <div class="menu-card">
          <div class="menu-card-img" style="background-image: url('https://images.unsplash.com/photo-1626078299034-94288f0d1cd0?w=800&auto=format&fit=crop&q=85');"></div>
          <div class="menu-card-content"><h3 class="menu-card-title">Jorr Combo</h3><p class="menu-card-desc">Half kheer and half rabri served together — the traditional Karachi dessert duo.</p><div class="menu-card-footer"><div class="spice-meter"><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span><span class="chili">🌶</span></div><div class="menu-card-price">PKR 700</div>
              <button class="add-to-cart" onclick="addToCart('Jorr Combo', 700, 'https://images.unsplash.com/photo-1626078299034-94288f0d1cd0?w=400&auto=format&fit=crop&q=85', this)">Add +</button></div></div>
        </div>
      </div>
    </div>

  </div>
</section>

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
      <div class="counter"><div class="counter-num" data-target="50000">0</div><div class="counter-label">Happy Customers</div></div>
      <div class="counter"><div class="counter-num" data-target="40">0</div><div class="counter-label">Years of Legacy</div></div>
      <div class="counter"><div class="counter-num" data-target="800">0</div><div class="counter-label">Daily Visitors</div></div>
      <div class="counter"><div class="counter-num" data-target="25">0</div><div class="counter-label">Signature Dishes</div></div>
    </div>
  </div>
</section>

<section id="reviews">
  <div class="container">
    <div class="section-eyebrow">What people say</div>
    <h2 class="section-title">Praised across <em>Karachi</em> and beyond.</h2>
    <p class="section-subtitle">From food critics to families, from first-timers to lifelong regulars.</p>
    <div class="reviews-track" id="reviewsTrack">
      <div class="review-card active">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Best nihari in Karachi. Hands down. The gravy is rich, the meat falls apart, and the naan is straight from the tandoor. Worth every minute of the wait."</p>
        <div class="review-author"><div class="review-avatar">AR</div><div><div class="review-name">Ahmed Raza</div><div class="review-meta">Local Guide · 47 reviews</div></div></div>
      </div>
      <div class="review-card">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Authentic old-school desi experience. The spices are perfectly balanced — not too overpowering, deeply flavorful. My family's go-to for over 20 years."</p>
        <div class="review-author"><div class="review-avatar">FA</div><div><div class="review-name">Fatima Aslam</div><div class="review-meta">Verified visitor</div></div></div>
      </div>
      <div class="review-card">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Crowded but completely worth it. I fly in from Dubai twice a year and Javed Nihari is the first place I visit before I even reach home. Legendary."</p>
        <div class="review-author"><div class="review-avatar">UK</div><div><div class="review-name">Usman Khan</div><div class="review-meta">Overseas customer · UAE</div></div></div>
      </div>
      <div class="review-card">
        <div class="review-stars">★★★★☆</div>
        <p class="review-text">"Phenomenal food, no question. The nalli nihari was unforgettable. Parking can be tricky during peak hours so go a bit early — but the experience is worth it."</p>
        <div class="review-author"><div class="review-avatar">SM</div><div><div class="review-name">Sara Malik</div><div class="review-meta">First-time visitor</div></div></div>
      </div>
      <div class="review-card">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">"Hot naan, spicy nihari, and the kheer at the end — this is what Karachi food culture looks like at its finest. A true institution."</p>
        <div class="review-author"><div class="review-avatar">BH</div><div><div class="review-name">Bilal Hussain</div><div class="review-meta">Food blogger</div></div></div>
      </div>
    </div>
    <div class="review-dots" id="reviewDots"></div>

    <div class="review-form-wrap">
      <h3>Share <em>your experience</em></h3>
      <p class="form-sub">Tell us about your visit. Your feedback helps us serve you better.</p>
      <form class="review-form" id="reviewForm" onsubmit="submitReview(event)">
        <div class="form-row">
          <div class="form-field">
            <label for="rName">Your Name</label>
            <input type="text" id="rName" required placeholder="Ahmed Khan">
          </div>
          <div class="form-field">
            <label for="rEmail">Email (optional)</label>
            <input type="email" id="rEmail" placeholder="you@example.com">
          </div>
        </div>
        <div class="form-field">
          <label>Your Rating</label>
          <div class="star-rating" id="starRating">
            <span class="star" data-star="1">★</span>
            <span class="star" data-star="2">★</span>
            <span class="star" data-star="3">★</span>
            <span class="star" data-star="4">★</span>
            <span class="star" data-star="5">★</span>
          </div>
        </div>
        <div class="form-field">
          <label for="rReview">Your Review</label>
          <textarea id="rReview" required placeholder="Share your thoughts about the food and experience..."></textarea>
        </div>
        <button type="submit">Submit Review</button>
      </form>
      <div class="review-success" id="reviewSuccess">
        Shukriya! Your review has been received. We'll post it after a quick check.
      </div>
    </div>
  </div>
</section>

<section id="locations">
  <div class="container">
    <div class="section-eyebrow">Visit Us</div>
    <h2 class="section-title">Two branches, <em>one tradition</em>.</h2>
    <p class="section-subtitle">Find your nearest Javed Nihari. Open seven days a week, from morning to late night.</p>
    <div class="locations-grid">
      <div class="location-card">
        <div class="location-map"><iframe src="https://maps.google.com/maps?q=24.9282014,67.0750023&z=17&output=embed" allowfullscreen></iframe></div>
        <div class="location-content">
          <div class="location-badge">Original Branch</div>
          <h3 class="location-name">FB Area</h3>
          <p class="location-info"><span class="icon">⌖</span> Dastagir, Block No. 15, Federal B Area, Karachi</p>
          <p class="location-info"><span class="icon">◷</span> Daily · 8:00 AM – 12:00 AM · Sunday from 6:00 AM</p>
          <p class="location-info"><span class="icon">☎</span> 0311-4422786 · 0324-7860881 · 021-36372111</p>
          <div class="location-buttons">
            <a href="tel:+923247860881" class="btn-location primary">Call Now</a>
            <a href="https://www.google.com/maps/place/Javed+Nihari/@24.9282014,67.0750023,17z/data=!3m1!4b1!4m6!3m5!1s0x3eb33f4148864f51:0x11885c9e5b3eba2c!8m2!3d24.9282014!4d67.0750023" target="_blank" class="btn-location secondary">Directions</a>
          </div>
        </div>
      </div>
      <div class="location-card">
        <div class="location-map"><iframe src="https://maps.google.com/maps?q=24.8851941,67.0623272&z=17&output=embed" allowfullscreen></iframe></div>
        <div class="location-content">
          <div class="location-badge">Bahadurabad Branch</div>
          <h3 class="location-name">Bahadurabad</h3>
          <p class="location-info"><span class="icon">⌖</span> Main Bahadurabad Chowk, Karachi</p>
          <p class="location-info"><span class="icon">◷</span> Daily · 8:00 AM – 12:00 AM</p>
          <p class="location-info"><span class="icon">☎</span> 021-34933111</p>
          <div class="location-buttons">
            <a href="tel:+922134933111" class="btn-location primary">Call Now</a>
            <a href="https://www.google.com/maps/place/Javed+Nihari/@24.8851941,67.0623272,17z/data=!3m1!4b1!4m6!3m5!1s0x3eb33f36788a299b:0x236e9f3ba6fba8ef!8m2!3d24.8851941!4d67.0623272" target="_blank" class="btn-location secondary">Directions</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- FLOATING CART BUTTON -->
<button class="cart-fab" id="cartFab" onclick="openCart()">
  <svg viewBox="0 0 24 24"><path d="M7 18c-1.1 0-1.99.9-1.99 2S5.9 22 7 22s2-.9 2-2-.9-2-2-2zM1 2v2h2l3.6 7.59-1.35 2.45c-.16.28-.25.61-.25.96 0 1.1.9 2 2 2h12v-2H7.42c-.14 0-.25-.11-.25-.25l.03-.12L8.1 13h7.45c.75 0 1.41-.41 1.75-1.03L21.7 4H5.21l-.94-2H1zm16 16c-1.1 0-1.99.9-1.99 2s.89 2 1.99 2 2-.9 2-2-.9-2-2-2z"/></svg>
  <span>Cart</span>
  <span class="cart-count-badge" id="cartCount">0</span>
</button>

<!-- CART DRAWER -->
<div class="cart-overlay" id="cartOverlay" onclick="closeCart()"></div>
<aside class="cart-drawer" id="cartDrawer">
  <div class="cart-header">
    <h3>Your <em>Order</em></h3>
    <button class="cart-close" onclick="closeCart()">✕</button>
  </div>
  <div class="demo-banner">⚠ Concept design · Demo ordering only · No real orders placed</div>
  <div class="cart-items" id="cartItems">
    <div class="cart-empty" id="cartEmpty">
      <div class="icon">🍲</div>
      <h4>Your cart is empty</h4>
      <p>Add some delicious nihari to get started.</p>
    </div>
  </div>
  <div class="cart-footer">
    <div class="cart-totals">
      <div class="cart-row"><span>Subtotal</span><span id="cartSubtotal">Rs. 0</span></div>
      <div class="cart-row"><span>Delivery Fee</span><span id="cartDelivery">Rs. 150</span></div>
      <div class="cart-row total"><span>Total</span><span class="amount" id="cartTotal">Rs. 0</span></div>
    </div>
    <button class="checkout-btn" id="checkoutBtn" onclick="openCheckout()" disabled>Proceed to Checkout</button>
  </div>
</aside>

<!-- CHECKOUT MODAL -->
<div class="checkout-modal" id="checkoutModal">
  <div class="checkout-box">
    <h3>Complete <em>Your Order</em></h3>
    <p class="form-sub">Fill in your details below. Cash on delivery available.</p>
    <form id="checkoutForm" onsubmit="confirmOrder(event)">
      <div class="form-row">
        <div class="form-field">
          <label>Full Name *</label>
          <input type="text" id="coName" required placeholder="Ahmed Khan">
        </div>
        <div class="form-field">
          <label>Phone Number *</label>
          <input type="tel" id="coPhone" required placeholder="03XX-XXXXXXX">
        </div>
      </div>
      
      <div class="form-field" style="margin-top: 1rem;">
        <label>Order Type *</label>
        <div class="order-type-grid">
          <div class="order-type-btn active" data-type="delivery" onclick="selectOrderType('delivery', this)">
            <span class="icon">🛵</span>
            <span>Home Delivery</span>
          </div>
          <div class="order-type-btn" data-type="pickup" onclick="selectOrderType('pickup', this)">
            <span class="icon">🏪</span>
            <span>Branch Pickup</span>
          </div>
        </div>
      </div>
      
      <div class="delivery-fields show" id="deliveryFields" style="margin-top: 1rem;">
        <div class="form-field">
          <label>Delivery Address *</label>
          <textarea id="coAddress" placeholder="House #, Street, Block, Area..."></textarea>
        </div>
        <div class="form-field">
          <label>Area</label>
          <input type="text" id="coArea" placeholder="e.g. FB Area, Gulshan, DHA">
        </div>
        <div class="form-field">
          <label>Special Instructions (optional)</label>
          <input type="text" id="coNotes" placeholder="e.g. Less spicy, extra naan">
        </div>
      </div>
      
      <div class="form-field" style="margin-top: 1rem;">
        <label>Payment Method</label>
        <div class="order-type-btn active" style="cursor: default;">
          <span class="icon">💵</span>
          <span>Cash on Delivery</span>
        </div>
      </div>
      
      <div class="checkout-actions">
        <button type="button" class="btn-back" onclick="closeCheckout()">Back to Cart</button>
        <button type="submit" class="btn-confirm">Confirm Order</button>
      </div>
    </form>
  </div>
</div>

<!-- ORDER SUCCESS MODAL -->
<div class="success-modal" id="successModal">
  <div class="success-box">
    <div class="success-check">✓</div>
    <h3>Order <em>Received</em>!</h3>
    <div class="order-no" id="orderNumber">JN-10000</div>
    <p class="success-eta">Estimated arrival: 35–45 minutes</p>
    
    <div class="summary" id="orderSummary"></div>
    
    <div class="demo-warning">
      <strong>⚠ Concept Design Notice</strong>
      This website is not live to sell products. It is a speculative design concept created by Yugh Studio for portfolio purposes and is not officially affiliated with any restaurant. No real order has been placed, no payment has been collected, and no data has been transmitted or stored.
    </div>
    
    <button class="success-close" onclick="closeSuccess()">Got it</button>
  </div>
</div>

<a href="https://wa.me/923247860881?text=Salaam!%20I%20would%20like%20to%20place%20an%20order" target="_blank" class="whatsapp-float" aria-label="Order on WhatsApp">
  <svg viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946.003-6.556 5.338-11.891 11.893-11.891 3.181.001 6.167 1.24 8.413 3.488 2.245 2.248 3.481 5.236 3.48 8.414-.003 6.557-5.338 11.892-11.893 11.892-1.99-.001-3.951-.5-5.688-1.448l-6.305 1.654zm6.597-3.807c1.676.995 3.276 1.591 5.392 1.592 5.448 0 9.886-4.434 9.889-9.885.002-5.462-4.415-9.89-9.881-9.892-5.452 0-9.887 4.434-9.889 9.884-.001 2.225.651 3.891 1.746 5.634l-.999 3.648 3.742-.981zm11.387-5.464c-.074-.124-.272-.198-.57-.347-.297-.149-1.758-.868-2.031-.967-.272-.099-.47-.149-.669.149-.198.297-.768.967-.941 1.165-.173.198-.347.223-.644.074-.297-.149-1.255-.462-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.521.151-.172.2-.296.3-.495.099-.198.05-.372-.025-.521-.075-.148-.669-1.611-.916-2.206-.242-.579-.487-.501-.669-.51l-.57-.01c-.198 0-.52.074-.792.372s-1.04 1.016-1.04 2.479 1.065 2.876 1.213 3.074c.149.198 2.095 3.2 5.076 4.487.709.306 1.263.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.695.248-1.29.173-1.414z"/></svg>
</a>

<footer>
  <div class="skyline"></div>
  <div class="container">
    <div class="footer-content">
      <div class="footer-brand">
        <div class="logo"><div class="logo-mark">J</div><div class="logo-text">Javed <em>Nihari</em></div></div>
        <div class="footer-urdu">جاوید نہاری</div>
        <p class="footer-tagline">"Karachi's legendary nihari, served fresh for generations."</p>
      </div>
      <div class="footer-col">
        <h4>Menu</h4>
        <ul>
          <li><a href="#menu">Nihari</a></li>
          <li><a href="#menu">Haleem</a></li>
          <li><a href="#menu">Biryani &amp; Pulao</a></li>
          <li><a href="#menu">Tandoor</a></li>
          <li><a href="#menu">Tin Pack</a></li>
        </ul>
      </div>
      <div class="footer-col">
        <h4>Visit</h4>
        <ul>
          <li><a href="#locations">FB Area Branch</a></li>
          <li><a href="#locations">Bahadurabad Branch</a></li>
          <li><a href="#locations">Opening Hours</a></li>
          <li><a href="#locations">Home Delivery</a></li>
        </ul>
      </div>
      <div class="footer-col">
        <h4>Connect</h4>
        <ul>
          <li><a href="#">WhatsApp Order</a></li>
          <li><a href="#">Catering</a></li>
          <li><a href="#">Bulk Orders</a></li>
          <li><a href="#">Tin Pack Export</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="footer-bottom-text">Concept design · Not affiliated with any existing restaurant</div>
      <div class="social-row">
        <a href="#" class="social-icon" aria-label="Facebook">f</a>
        <a href="#" class="social-icon" aria-label="Instagram">⊡</a>
        <a href="#" class="social-icon" aria-label="YouTube">▶</a>
        <a href="#" class="social-icon" aria-label="WhatsApp">✆</a>
      </div>
    </div>
    <p class="disclaimer">
      This is a speculative design concept created for portfolio purposes. Not officially affiliated with any restaurant brand. Designed by <a href="#" target="_blank">Yugh Studio</a>.
    </p>
  </div>
</footer>

<script>
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
for (let i = 0; i < 12; i++) {
  const p = document.createElement('div');
  p.className = 'particle';
  p.style.left = Math.random() * 100 + '%';
  p.style.top = Math.random() * 100 + '%';
  p.style.animationDelay = Math.random() * 8 + 's';
  p.style.animationDuration = (6 + Math.random() * 4) + 's';
  steamContainer.appendChild(p);
}

const heroSlides = document.querySelectorAll('.hero-slide');
const heroTextSlides = document.querySelectorAll('.hero-text-slide');
const carouselDots = document.querySelectorAll('.carousel-dot');
let currentSlide = 0;
function showSlide(i) {
  heroSlides[currentSlide].classList.remove('active');
  heroTextSlides[currentSlide].classList.remove('active');
  carouselDots[currentSlide].classList.remove('active');
  currentSlide = i;
  heroSlides[currentSlide].classList.add('active');
  heroTextSlides[currentSlide].classList.add('active');
  carouselDots[currentSlide].classList.add('active');
}
carouselDots.forEach((dot, i) => dot.addEventListener('click', () => showSlide(i)));
setInterval(() => showSlide((currentSlide + 1) % heroSlides.length), 6000);

const tabs = document.querySelectorAll('.category-tab');
const sections = document.querySelectorAll('.category-section');
tabs.forEach(tab => {
  tab.addEventListener('click', () => {
    tabs.forEach(t => t.classList.remove('active'));
    tab.classList.add('active');
    const cat = tab.dataset.cat;
    sections.forEach(s => {
      s.style.display = (cat === 'all' || s.dataset.cat === cat) ? 'block' : 'none';
    });
  });
});

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
          entry.target.textContent = Math.floor(current).toLocaleString();
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

const reviewCards = document.querySelectorAll('.review-card');
const dotsContainer = document.getElementById('reviewDots');
let currentReview = 0;
reviewCards.forEach((_, i) => {
  const dot = document.createElement('div');
  dot.className = 'review-dot' + (i === 0 ? ' active' : '');
  dot.onclick = () => showReview(i);
  dotsContainer.appendChild(dot);
});
const reviewDots = document.querySelectorAll('.review-dot');
function showReview(i) {
  reviewCards[currentReview].classList.remove('active');
  reviewDots[currentReview].classList.remove('active');
  currentReview = i;
  reviewCards[currentReview].classList.add('active');
  reviewDots[currentReview].classList.add('active');
}
setInterval(() => showReview((currentReview + 1) % reviewCards.length), 5500);

// LEAVE REVIEW FORM
let selectedStars = 0;
const stars = document.querySelectorAll('#starRating .star');
stars.forEach(s => {
  s.addEventListener('click', () => {
    selectedStars = parseInt(s.dataset.star);
    stars.forEach((st, i) => {
      st.classList.toggle('active', i < selectedStars);
    });
  });
  s.addEventListener('mouseenter', () => {
    const n = parseInt(s.dataset.star);
    stars.forEach((st, i) => st.classList.toggle('active', i < n));
  });
});
document.getElementById('starRating').addEventListener('mouseleave', () => {
  stars.forEach((st, i) => st.classList.toggle('active', i < selectedStars));
});

function submitReview(e) {
  e.preventDefault();
  if (selectedStars === 0) {
    alert('Please select a star rating');
    return;
  }
  document.getElementById('reviewForm').style.display = 'none';
  document.getElementById('reviewSuccess').classList.add('show');
}

// ============================================
// ORDERING SYSTEM (DEMO ONLY — NO BACKEND)
// ============================================
const cart = [];
const DELIVERY_FEE = 150;
let orderType = 'delivery';

function addToCart(name, price, img, btn) {
  const existing = cart.find(i => i.name === name);
  if (existing) {
    existing.qty += 1;
  } else {
    cart.push({ name, price, img, qty: 1 });
  }
  renderCart();
  // Button feedback
  const original = btn.innerHTML;
  btn.classList.add('added');
  btn.innerHTML = '✓ Added';
  setTimeout(() => {
    btn.classList.remove('added');
    btn.innerHTML = original;
  }, 1200);
}

function updateQty(name, delta) {
  const item = cart.find(i => i.name === name);
  if (!item) return;
  item.qty += delta;
  if (item.qty <= 0) {
    const idx = cart.indexOf(item);
    cart.splice(idx, 1);
  }
  renderCart();
}

function removeItem(name) {
  const idx = cart.findIndex(i => i.name === name);
  if (idx > -1) cart.splice(idx, 1);
  renderCart();
}

function renderCart() {
  const itemsWrap = document.getElementById('cartItems');
  const countEl = document.getElementById('cartCount');
  const fab = document.getElementById('cartFab');
  const checkoutBtn = document.getElementById('checkoutBtn');
  
  const totalCount = cart.reduce((s, i) => s + i.qty, 0);
  countEl.textContent = totalCount;
  
  if (totalCount > 0) fab.classList.add('visible');
  else fab.classList.remove('visible');
  
  if (cart.length === 0) {
    itemsWrap.innerHTML = `
      <div class="cart-empty">
        <div class="icon">🍲</div>
        <h4>Your cart is empty</h4>
        <p>Add some delicious nihari to get started.</p>
      </div>`;
    checkoutBtn.disabled = true;
  } else {
    itemsWrap.innerHTML = cart.map(item => `
      <div class="cart-item">
        <div class="cart-item-img" style="background-image: url('${item.img}');"></div>
        <div class="cart-item-content">
          <div class="cart-item-name">${item.name}</div>
          <div class="cart-item-price">Rs. ${item.price.toLocaleString()} each</div>
          <div class="cart-item-controls">
            <button class="qty-btn" onclick="updateQty('${item.name}', -1)">−</button>
            <span class="qty-value">${item.qty}</span>
            <button class="qty-btn" onclick="updateQty('${item.name}', 1)">+</button>
            <button class="cart-item-remove" onclick="removeItem('${item.name}')">Remove</button>
          </div>
        </div>
      </div>`).join('');
    checkoutBtn.disabled = false;
  }
  
  const subtotal = cart.reduce((s, i) => s + i.price * i.qty, 0);
  const delivery = orderType === 'pickup' ? 0 : (cart.length > 0 ? DELIVERY_FEE : 0);
  const total = subtotal + delivery;
  
  document.getElementById('cartSubtotal').textContent = 'Rs. ' + subtotal.toLocaleString();
  document.getElementById('cartDelivery').textContent = delivery === 0 ? 'Free' : 'Rs. ' + delivery.toLocaleString();
  document.getElementById('cartTotal').textContent = 'Rs. ' + total.toLocaleString();
}

function openCart() {
  document.getElementById('cartDrawer').classList.add('open');
  document.getElementById('cartOverlay').classList.add('open');
  document.body.style.overflow = 'hidden';
}
function closeCart() {
  document.getElementById('cartDrawer').classList.remove('open');
  document.getElementById('cartOverlay').classList.remove('open');
  document.body.style.overflow = '';
}

function openCheckout() {
  closeCart();
  document.getElementById('checkoutModal').classList.add('open');
  document.body.style.overflow = 'hidden';
}
function closeCheckout() {
  document.getElementById('checkoutModal').classList.remove('open');
  document.body.style.overflow = '';
}

function selectOrderType(type, el) {
  orderType = type;
  document.querySelectorAll('.order-type-btn[data-type]').forEach(b => b.classList.remove('active'));
  el.classList.add('active');
  const deliveryFields = document.getElementById('deliveryFields');
  if (type === 'pickup') {
    deliveryFields.classList.remove('show');
    document.getElementById('coAddress').required = false;
  } else {
    deliveryFields.classList.add('show');
    document.getElementById('coAddress').required = true;
  }
  renderCart(); // update delivery fee display
}

function confirmOrder(e) {
  e.preventDefault();
  
  const name = document.getElementById('coName').value;
  const phone = document.getElementById('coPhone').value;
  
  if (orderType === 'delivery' && !document.getElementById('coAddress').value) {
    alert('Please enter your delivery address');
    return;
  }
  
  // Generate fake order number
  const orderNo = 'JN-' + Math.floor(10000 + Math.random() * 90000);
  
  // Build summary
  const subtotal = cart.reduce((s, i) => s + i.price * i.qty, 0);
  const delivery = orderType === 'pickup' ? 0 : DELIVERY_FEE;
  const total = subtotal + delivery;
  
  let summaryHTML = '';
  cart.forEach(item => {
    summaryHTML += `<div class="summary-row"><span>${item.qty}× ${item.name}</span><span>Rs. ${(item.price * item.qty).toLocaleString()}</span></div>`;
  });
  summaryHTML += `<div class="summary-row"><span>Subtotal</span><span>Rs. ${subtotal.toLocaleString()}</span></div>`;
  summaryHTML += `<div class="summary-row"><span>${orderType === 'pickup' ? 'Pickup' : 'Delivery Fee'}</span><span>${delivery === 0 ? 'Free' : 'Rs. ' + delivery.toLocaleString()}</span></div>`;
  summaryHTML += `<div class="summary-row"><strong>Total</strong><strong>Rs. ${total.toLocaleString()}</strong></div>`;
  summaryHTML += `<div class="summary-row" style="margin-top: 0.75rem; padding-top: 0.75rem; border-top: 1px solid var(--border);"><span>Customer</span><strong>${name}</strong></div>`;
  summaryHTML += `<div class="summary-row"><span>Phone</span><strong>${phone}</strong></div>`;
  summaryHTML += `<div class="summary-row"><span>Type</span><strong>${orderType === 'pickup' ? 'Branch Pickup' : 'Home Delivery'}</strong></div>`;
  
  document.getElementById('orderNumber').textContent = orderNo;
  document.getElementById('orderSummary').innerHTML = summaryHTML;
  
  closeCheckout();
  document.getElementById('successModal').classList.add('open');
}

function closeSuccess() {
  document.getElementById('successModal').classList.remove('open');
  document.body.style.overflow = '';
  // Clear cart
  cart.length = 0;
  document.getElementById('checkoutForm').reset();
  document.getElementById('coAddress').required = true;
  renderCart();
}

const revealObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.style.opacity = '1';
      entry.target.style.transform = 'translateY(0)';
    }
  });
}, { threshold: 0.1, rootMargin: '0px 0px -50px 0px' });
document.querySelectorAll('.menu-card, .counter, .location-card').forEach((el, i) => {
  el.style.opacity = '0';
  el.style.transform = 'translateY(30px)';
  el.style.transition = `all 0.7s cubic-bezier(0.16, 1, 0.3, 1) ${(i % 6) * 0.05}s`;
  revealObserver.observe(el);
});

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
