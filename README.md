# hieunganhocmarketing.github.io
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Digital Marketing Masterclass | HAPAS Case Study</title>
<link href="https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:wght@300;400;500;600;700;800;900&family=Playfair+Display:ital,wght@0,700;0,900;1,700&display=swap" rel="stylesheet">
<style>
  :root {
    --black: #0a0a0a;
    --white: #fafaf8;
    --cream: #f5f0e8;
    --hapas-red: #c8392b;
    --hapas-gold: #d4a043;
    --hapas-warm: #e8d5b7;
    --accent: #2d6a4f;
    --accent2: #1a4a6b;
    --muted: #6b6460;
    --border: #e0d8cc;
    --section-bg: #fdf8f3;
    --nav-h: 56px;
    --tab-h: 52px;
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body { font-family: 'Be Vietnam Pro', sans-serif; background: var(--white); color: var(--black); line-height: 1.7; font-size: 16px; }
  .top-nav { position: fixed; top: 0; left: 0; right: 0; height: var(--nav-h); background: var(--black); display: flex; align-items: center; justify-content: space-between; padding: 0 32px; z-index: 200; border-bottom: 1px solid rgba(255,255,255,0.08); }
  .top-nav-brand { display: flex; align-items: center; gap: 10px; }
  .top-nav-brand .brand-mark { background: var(--hapas-red); color: white; font-weight: 900; font-size: 13px; padding: 4px 10px; border-radius: 3px; letter-spacing: 1px; }
  .top-nav-brand .brand-title { color: rgba(255,255,255,0.7); font-size: 13px; font-weight: 500; }
  .top-nav-sections { display: flex; gap: 4px; }
  .nav-section-btn { background: transparent; border: 1px solid rgba(255,255,255,0.15); color: rgba(255,255,255,0.6); font-family: inherit; font-size: 12px; font-weight: 600; letter-spacing: 0.5px; padding: 7px 16px; border-radius: 4px; cursor: pointer; transition: all 0.2s; white-space: nowrap; }
  .nav-section-btn:hover, .nav-section-btn.active { background: var(--hapas-red); border-color: var(--hapas-red); color: white; }
  .nav-section-btn span { display: inline-block; width: 18px; height: 18px; background: rgba(255,255,255,0.12); border-radius: 50%; font-size: 10px; text-align: center; line-height: 18px; margin-right: 6px; }
  .nav-section-btn.active span { background: rgba(255,255,255,0.2); }
  .section-tabs { position: fixed; top: var(--nav-h); left: 0; right: 0; height: var(--tab-h); background: var(--cream); border-bottom: 2px solid var(--border); display: flex; align-items: center; gap: 4px; padding: 0 24px; overflow-x: auto; z-index: 190; transition: all 0.3s; scrollbar-width: none; }
  .section-tabs::-webkit-scrollbar { display: none; }
  .tab-btn { background: transparent; border: none; font-family: inherit; font-size: 12px; font-weight: 600; color: var(--muted); padding: 6px 14px; border-radius: 20px; cursor: pointer; transition: all 0.2s; white-space: nowrap; flex-shrink: 0; }
  .tab-btn:hover { background: var(--border); color: var(--black); }
  .tab-btn.active { background: var(--black); color: white; }
  body { padding-top: calc(var(--nav-h) + var(--tab-h)); }
  .view-panel { display: none; }
  .view-panel.active { display: block; }
  .hero { background: var(--black); color: var(--white); padding: 80px 40px 60px; position: relative; overflow: hidden; }
  .hero::before { content: ''; position: absolute; top: -60px; right: -60px; width: 400px; height: 400px; background: radial-gradient(circle, rgba(200,57,43,0.3) 0%, transparent 70%); border-radius: 50%; }
  .hero::after { content: ''; position: absolute; bottom: -80px; left: 20%; width: 300px; height: 300px; background: radial-gradient(circle, rgba(212,160,67,0.2) 0%, transparent 70%); border-radius: 50%; }
  .hero-tag { display: inline-block; background: var(--hapas-red); color: white; font-size: 11px; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; padding: 6px 14px; border-radius: 2px; margin-bottom: 28px; }
  .hero h1 { font-family: 'Playfair Display', serif; font-size: clamp(36px, 5vw, 72px); font-weight: 900; line-height: 1.05; margin-bottom: 20px; position: relative; z-index: 1; }
  .hero h1 span { color: var(--hapas-gold); }
  .hero-sub { font-size: 18px; color: rgba(255,255,255,0.7); max-width: 600px; margin-bottom: 40px; position: relative; z-index: 1; }
  .hero-meta { display: flex; gap: 32px; flex-wrap: wrap; position: relative; z-index: 1; }
  .hero-meta-item { border-left: 2px solid var(--hapas-red); padding-left: 12px; }
  .hero-meta-item .label { font-size: 11px; letter-spacing: 1px; text-transform: uppercase; color: rgba(255,255,255,0.5); display: block; }
  .hero-meta-item .value { font-size: 15px; font-weight: 600; color: var(--white); }
  .container { max-width: 860px; margin: 0 auto; padding: 60px 40px; }
  .section-header { display: flex; align-items: flex-start; gap: 20px; margin-bottom: 40px; padding-bottom: 24px; border-bottom: 2px solid var(--black); }
  .section-number { font-family: 'Playfair Display', serif; font-size: 64px; font-weight: 900; color: var(--border); line-height: 1; flex-shrink: 0; width: 70px; }
  .section-title-block h2 { font-family: 'Playfair Display', serif; font-size: 32px; font-weight: 700; line-height: 1.2; margin-bottom: 6px; }
  .section-title-block .section-desc { font-size: 14px; color: var(--muted); font-style: italic; }
  .chapter-divider { background: var(--black); color: var(--white); padding: 60px 40px; text-align: center; }
  .chapter-divider .chapter-num { font-size: 11px; letter-spacing: 3px; text-transform: uppercase; color: var(--hapas-gold); margin-bottom: 12px; }
  .chapter-divider h2 { font-family: 'Playfair Display', serif; font-size: clamp(28px, 4vw, 48px); font-weight: 700; line-height: 1.2; }
  .chapter-divider p { font-size: 16px; color: rgba(255,255,255,0.6); max-width: 500px; margin: 16px auto 0; }
  p { margin-bottom: 18px; color: #2a2520; }
  h3 { font-size: 20px; font-weight: 700; margin: 32px 0 14px; color: var(--black); }
  h4 { font-size: 16px; font-weight: 700; margin: 24px 0 10px; color: var(--black); }
  .callout { border-left: 4px solid var(--hapas-red); background: #fff5f4; padding: 20px 24px; margin: 28px 0; border-radius: 0 8px 8px 0; }
  .callout.gold { border-color: var(--hapas-gold); background: #fdf8ee; }
  .callout.green { border-color: var(--accent); background: #f0f7f4; }
  .callout.blue { border-color: var(--accent2); background: #f0f4f8; }
  .callout .callout-label { font-size: 11px; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; color: var(--hapas-red); margin-bottom: 8px; display: block; }
  .callout.gold .callout-label { color: var(--hapas-gold); }
  .callout.green .callout-label { color: var(--accent); }
  .callout.blue .callout-label { color: var(--accent2); }
  .callout p { margin: 0; font-size: 15px; }
  .big-quote { font-family: 'Playfair Display', serif; font-size: clamp(22px, 3vw, 32px); font-style: italic; font-weight: 700; line-height: 1.35; color: var(--black); padding: 32px 0; border-top: 2px solid var(--black); border-bottom: 2px solid var(--black); margin: 40px 0; text-align: center; }
  .big-quote span { color: var(--hapas-red); }
  .framework { background: var(--section-bg); border: 1px solid var(--border); border-radius: 12px; padding: 32px; margin: 32px 0; }
  .framework-title { font-size: 13px; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; color: var(--muted); margin-bottom: 20px; }
  .framework-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 16px; }
  .framework-item { background: white; border: 1px solid var(--border); border-radius: 8px; padding: 16px 18px; }
  .framework-item .fi-label { font-size: 11px; font-weight: 700; letter-spacing: 1.5px; text-transform: uppercase; color: var(--muted); margin-bottom: 6px; display: block; }
  .framework-item .fi-value { font-size: 15px; font-weight: 600; color: var(--black); }
  .framework-item .fi-note { font-size: 13px; color: var(--muted); margin-top: 4px; font-style: italic; }
  .case-block { background: var(--black); color: var(--white); border-radius: 12px; padding: 32px; margin: 32px 0; position: relative; overflow: hidden; }
  .case-block::before { content: 'HAPAS CASE STUDY'; position: absolute; top: 16px; right: 20px; font-size: 10px; font-weight: 700; letter-spacing: 2px; color: var(--hapas-gold); }
  .case-block h4 { color: var(--hapas-gold); font-size: 17px; margin-top: 0; }
  .case-block p { color: rgba(255,255,255,0.8); font-size: 15px; }
  .case-block ul { padding-left: 20px; }
  .case-block li { color: rgba(255,255,255,0.8); font-size: 15px; margin-bottom: 8px; }
  .compare-table { width: 100%; border-collapse: collapse; margin: 24px 0; font-size: 14px; }
  .compare-table th { background: var(--black); color: var(--white); padding: 12px 16px; text-align: left; font-weight: 600; }
  .compare-table td { padding: 12px 16px; border-bottom: 1px solid var(--border); vertical-align: top; }
  .compare-table tr:nth-child(even) td { background: var(--section-bg); }
  .compare-table .good { color: #2d6a4f; font-weight: 600; }
  .compare-table .bad { color: var(--hapas-red); font-weight: 600; }
  .checklist { list-style: none; margin: 20px 0; }
  .checklist li { padding: 8px 0 8px 32px; position: relative; font-size: 15px; border-bottom: 1px solid var(--border); }
  .checklist li::before { content: '✓'; position: absolute; left: 0; color: var(--accent); font-weight: 700; font-size: 16px; }
  .checklist li.warn::before { content: '⚠'; color: var(--hapas-gold); }
  .checklist li.bad::before { content: '✗'; color: var(--hapas-red); }
  .badge { display: inline-block; padding: 3px 10px; border-radius: 20px; font-size: 12px; font-weight: 700; letter-spacing: 0.5px; }
  .badge-red { background: #fde8e6; color: var(--hapas-red); }
  .badge-green { background: #e6f4ed; color: var(--accent); }
  .badge-gold { background: #fdf5e6; color: #b8860b; }
  .num-list { counter-reset: item; list-style: none; margin: 20px 0; }
  .num-list li { counter-increment: item; padding: 12px 16px 12px 52px; position: relative; margin-bottom: 12px; background: var(--section-bg); border-radius: 8px; }
  .num-list li::before { content: counter(item); position: absolute; left: 16px; top: 50%; transform: translateY(-50%); width: 26px; height: 26px; background: var(--black); color: var(--white); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 12px; font-weight: 700; }
  .stats-row { display: grid; grid-template-columns: repeat(auto-fit, minmax(140px, 1fr)); gap: 16px; margin: 28px 0; }
  .stat-box { background: var(--section-bg); border: 1px solid var(--border); border-radius: 10px; padding: 20px 16px; text-align: center; }
  .stat-box .stat-num { font-family: 'Playfair Display', serif; font-size: 36px; font-weight: 900; color: var(--black); line-height: 1; margin-bottom: 6px; }
  .stat-box .stat-label { font-size: 12px; color: var(--muted); font-weight: 500; }
  .stat-box.highlight { background: var(--black); border-color: var(--black); }
  .stat-box.highlight .stat-num { color: var(--hapas-gold); }
  .stat-box.highlight .stat-label { color: rgba(255,255,255,0.7); }
  .funnel-step { display: flex; gap: 20px; align-items: flex-start; margin-bottom: 24px; padding: 20px; background: var(--section-bg); border-radius: 8px; border: 1px solid var(--border); }
  .funnel-icon { width: 44px; height: 44px; background: var(--black); color: var(--white); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 700; font-size: 16px; flex-shrink: 0; }
  .funnel-content h4 { margin: 0 0 6px; font-size: 16px; }
  .funnel-content p { margin: 0; font-size: 14px; color: var(--muted); }
  .action-week { border: 1px solid var(--border); border-radius: 10px; margin-bottom: 16px; overflow: hidden; }
  .action-week-header { background: var(--black); color: var(--white); padding: 14px 20px; font-weight: 700; font-size: 14px; display: flex; justify-content: space-between; align-items: center; }
  .action-week-header .week-tag { color: var(--hapas-gold); font-size: 12px; }
  .action-week-body { padding: 16px 20px; }
  .action-week-body li { font-size: 14px; margin-bottom: 8px; padding-left: 16px; position: relative; }
  .action-week-body li::before { content: '→'; position: absolute; left: 0; color: var(--muted); }
  .cs-card { border: 1px solid var(--border); border-radius: 14px; overflow: hidden; margin: 28px 0; transition: box-shadow 0.2s; }
  .cs-card:hover { box-shadow: 0 8px 32px rgba(0,0,0,0.1); }
  .cs-image-banner { position: relative; height: 220px; overflow: hidden; background: var(--black); }
  .cs-image-banner img { width: 100%; height: 100%; object-fit: cover; opacity: 0.85; transition: opacity 0.3s; }
  .cs-card:hover .cs-image-banner img { opacity: 1; }
  .cs-image-overlay { position: absolute; inset: 0; background: linear-gradient(to top, rgba(10,10,10,0.7) 0%, transparent 60%); }
  .cs-image-meta { position: absolute; bottom: 16px; left: 20px; right: 20px; display: flex; align-items: flex-end; justify-content: space-between; }
  .cs-brand-name { font-family: 'Playfair Display', serif; font-size: 28px; font-weight: 900; color: white; line-height: 1; }
  .cs-verdict { font-size: 11px; font-weight: 700; padding: 5px 12px; border-radius: 20px; letter-spacing: 0.5px; white-space: nowrap; }
  .verdict-good { background: rgba(45,106,79,0.9); color: white; }
  .verdict-bad { background: rgba(200,57,43,0.9); color: white; }
  .verdict-mixed { background: rgba(212,160,67,0.9); color: white; }
  .cs-links { display: flex; gap: 8px; padding: 14px 20px; background: var(--section-bg); border-bottom: 1px solid var(--border); flex-wrap: wrap; }
  .cs-link { display: inline-flex; align-items: center; gap: 5px; font-size: 11px; font-weight: 700; letter-spacing: 0.5px; color: var(--accent2); text-decoration: none; padding: 5px 12px; border: 1px solid var(--border); border-radius: 20px; background: white; transition: all 0.2s; }
  .cs-link:hover { background: var(--black); color: white; border-color: var(--black); }
  .cs-link svg { width: 12px; height: 12px; flex-shrink: 0; }
  .cs-body { display: grid; grid-template-columns: 1fr 1fr; gap: 0; }
  .cs-col { padding: 20px 24px; }
  .cs-col:first-child { border-right: 1px solid var(--border); }
  .cs-col h4 { font-size: 12px; text-transform: uppercase; letter-spacing: 1.5px; color: var(--muted); margin-bottom: 14px; }
  .cs-col ul { list-style: none; }
  .cs-col li { font-size: 14px; margin-bottom: 10px; padding-left: 16px; position: relative; line-height: 1.5; }
  .cs-col li::before { content: '•'; position: absolute; left: 0; color: var(--hapas-red); }
  .hook-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 16px; margin: 24px 0; }
  .hook-item { background: var(--section-bg); border: 1px solid var(--border); border-radius: 10px; padding: 16px; }
  .hook-type { font-size: 12px; font-weight: 700; letter-spacing: 1px; text-transform: uppercase; color: var(--hapas-red); margin-bottom: 8px; }
  .hook-example { font-size: 15px; font-style: italic; margin-bottom: 10px; padding: 10px; background: white; border-radius: 6px; border-left: 3px solid var(--hapas-red); }
  .hook-why { font-size: 12px; color: var(--muted); }
  .platform-guide { display: flex; flex-direction: column; gap: 16px; margin: 24px 0; }
  .platform-card { border: 1px solid var(--border); border-radius: 12px; overflow: hidden; }
  .platform-header { display: flex; align-items: center; gap: 12px; padding: 14px 20px; font-size: 15px; }
  .platform-icon { font-size: 20px; }
  .platform-tag { margin-left: auto; font-size: 11px; font-weight: 600; padding: 3px 10px; border-radius: 10px; background: rgba(255,255,255,0.2); color: white; }
  .platform-body { padding: 16px 20px; }
  .platform-body p { font-size: 14px; margin-bottom: 10px; }
  .platform-dont { background: #fff5f4; border-left: 3px solid var(--hapas-red); padding: 8px 12px; border-radius: 0 6px 6px 0; }
  .tiktok { background: linear-gradient(135deg, #010101, #69c9d0); color: white; }
  .instagram { background: linear-gradient(135deg, #833ab4, #fd1d1d, #fcb045); color: white; }
  .facebook { background: #1877f2; color: white; }
  .shopee { background: linear-gradient(135deg, #ee4d2d, #ff7337); color: white; }
  .story-arc { margin: 24px 0; }
  .arc-step { display: flex; gap: 16px; margin-bottom: 16px; align-items: flex-start; }
  .arc-num { width: 36px; height: 36px; background: var(--hapas-red); color: white; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 700; font-size: 14px; flex-shrink: 0; }
  .arc-content { flex: 1; background: var(--section-bg); border: 1px solid var(--border); border-radius: 8px; padding: 14px 16px; }
  .arc-content strong { display: block; margin-bottom: 6px; font-size: 15px; }
  .arc-content p { margin: 0; font-size: 14px; color: #3a3530; }
  .calendar-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 16px; margin: 24px 0; }
  .cal-month { background: var(--section-bg); border: 1px solid var(--border); border-radius: 10px; overflow: hidden; }
  .cal-month-header { background: var(--black); color: var(--white); padding: 10px 16px; font-weight: 700; font-size: 14px; }
  .cal-month-body { padding: 12px; }
  .cal-event { padding: 10px 0; border-bottom: 1px solid var(--border); }
  .cal-event:last-child { border-bottom: none; }
  .cal-date { display: inline-block; background: var(--hapas-red); color: white; font-size: 11px; font-weight: 700; padding: 2px 8px; border-radius: 10px; margin-bottom: 4px; }
  .cal-name { display: block; font-weight: 700; font-size: 14px; margin-bottom: 2px; }
  .cal-note { display: block; font-size: 12px; color: var(--muted); }
  .week-template { border: 1px solid var(--border); border-radius: 10px; overflow: hidden; margin: 24px 0; }
  .week-day { display: flex; gap: 16px; padding: 16px 20px; border-bottom: 1px solid var(--border); align-items: flex-start; }
  .week-day:last-child { border-bottom: none; }
  .week-day-label { font-weight: 700; font-size: 13px; width: 70px; flex-shrink: 0; padding-top: 4px; color: var(--muted); }
  .week-day-content { flex: 1; }
  .week-day-content p { margin: 4px 0 4px; font-size: 14px; }
  .week-day-content small { font-size: 12px; color: var(--muted); }
  .pillar-tag { display: inline-block; padding: 2px 10px; border-radius: 10px; font-size: 11px; font-weight: 700; letter-spacing: 0.5px; margin-bottom: 4px; }
  .pillar-edu { background: #e8f4f8; color: #1a6a8b; }
  .pillar-product { background: #fde8e6; color: var(--hapas-red); }
  .pillar-social { background: #e6f4ed; color: var(--accent); }
  .pillar-lifestyle { background: #fdf5e6; color: #b8860b; }
  .repurpose-flow { margin: 24px 0; }
  .repurpose-source { background: var(--black); color: var(--white); padding: 14px 20px; border-radius: 10px 10px 0 0; font-weight: 700; font-size: 15px; text-align: center; }
  .repurpose-arrow { text-align: center; padding: 8px; font-size: 18px; color: var(--muted); }
  .repurpose-items { display: grid; grid-template-columns: repeat(auto-fit, minmax(160px, 1fr)); gap: 8px; }
  .repurpose-item { background: var(--section-bg); border: 1px solid var(--border); border-radius: 8px; padding: 12px; font-size: 13px; text-align: center; }
  .perf-level { display: flex; gap: 16px; margin-bottom: 16px; align-items: flex-start; }
  .perf-num { width: 36px; height: 36px; border-radius: 8px; display: flex; align-items: center; justify-content: center; font-weight: 900; font-size: 12px; flex-shrink: 0; }
  .l1 { background: #e8f4f8; color: #1a6a8b; }
  .l2 { background: #e6f4ed; color: var(--accent); }
  .l3 { background: #fdf5e6; color: #b8860b; }
  .l4 { background: #fde8e6; color: var(--hapas-red); }
  .perf-content { flex: 1; padding: 14px 16px; background: var(--section-bg); border-radius: 8px; border: 1px solid var(--border); }
  .perf-content strong { display: block; margin-bottom: 6px; }
  .perf-content p { margin: 0 0 8px; font-size: 14px; }
  .perf-benchmark { font-size: 12px; background: white; padding: 6px 10px; border-radius: 4px; color: var(--muted); font-style: italic; }
  .process-flow { margin: 24px 0; }
  .process-step { display: flex; gap: 16px; margin-bottom: 16px; }
  .process-num { width: 36px; height: 36px; background: var(--black); color: var(--hapas-gold); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-weight: 700; font-size: 16px; flex-shrink: 0; }
  .process-body { flex: 1; padding: 14px 16px; background: var(--section-bg); border-radius: 8px; border: 1px solid var(--border); }
  .process-body strong { display: block; margin-bottom: 6px; font-size: 15px; }
  .process-body p { margin: 0; font-size: 14px; }
  .exercise-card { border: 1px solid var(--border); border-radius: 12px; overflow: hidden; margin-bottom: 24px; }
  .exercise-header { display: flex; align-items: center; gap: 12px; padding: 14px 20px; background: var(--section-bg); border-bottom: 1px solid var(--border); flex-wrap: wrap; }
  .exercise-num { background: var(--black); color: var(--hapas-gold); padding: 4px 12px; border-radius: 4px; font-weight: 700; font-size: 13px; }
  .exercise-title { font-weight: 700; font-size: 16px; flex: 1; }
  .exercise-level { font-size: 12px; font-weight: 700; padding: 3px 10px; border-radius: 20px; }
  .level-easy { background: #e6f4ed; color: var(--accent); }
  .level-mid { background: #fdf5e6; color: #b8860b; }
  .level-hard { background: #fde8e6; color: var(--hapas-red); }
  .exercise-body { padding: 20px 24px; }
  .exercise-body p { font-size: 15px; margin-bottom: 12px; }
  .exercise-body ol { padding-left: 20px; margin: 12px 0; }
  .exercise-body ol li { font-size: 14px; margin-bottom: 8px; }
  .submit-exercise-btn { margin-top: 16px; background: var(--black); color: var(--white); border: none; padding: 12px 24px; border-radius: 8px; font-size: 14px; font-weight: 700; cursor: pointer; font-family: inherit; transition: background 0.2s; }
  .submit-exercise-btn:hover { background: var(--hapas-red); }
  .chat-disclaimer { background: var(--section-bg); border: 1px solid var(--border); border-radius: 8px; padding: 16px 20px; margin-bottom: 20px; font-size: 14px; }
  .chat-container { border: 1px solid var(--border); border-radius: 12px; overflow: hidden; }
  .chat-messages { min-height: 300px; max-height: 600px; overflow-y: auto; padding: 20px; display: flex; flex-direction: column; gap: 16px; background: var(--section-bg); }
  .chat-msg { display: flex; gap: 12px; align-items: flex-start; }
  .chat-msg.user-msg { flex-direction: row-reverse; }
  .chat-avatar { width: 36px; height: 36px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 18px; flex-shrink: 0; background: var(--black); }
  .chat-bubble { max-width: 80%; background: white; border: 1px solid var(--border); border-radius: 12px; padding: 12px 16px; font-size: 14px; line-height: 1.6; }
  .chat-bubble p { margin-bottom: 8px; }
  .chat-bubble p:last-child { margin: 0; }
  .chat-bubble ul { padding-left: 20px; }
  .chat-bubble li { margin-bottom: 4px; }
  .chat-msg.user-msg .chat-bubble { background: var(--black); color: white; border-color: var(--black); }
  .chat-quick-prompts { padding: 12px 20px; background: white; border-top: 1px solid var(--border); display: flex; gap: 8px; flex-wrap: wrap; }
  .quick-prompt-label { font-size: 12px; color: var(--muted); margin-bottom: 8px; width: 100%; }
  .quick-prompt { background: var(--section-bg); border: 1px solid var(--border); padding: 6px 12px; border-radius: 20px; font-size: 12px; cursor: pointer; font-family: inherit; transition: all 0.2s; color: var(--black); white-space: nowrap; }
  .quick-prompt:hover { background: var(--black); color: white; border-color: var(--black); }
  .chat-input-area { display: flex; border-top: 1px solid var(--border); background: white; }
  #chatInput { flex: 1; border: none; padding: 16px 20px; font-size: 14px; font-family: inherit; resize: none; outline: none; background: transparent; }
  #chatSendBtn { background: var(--hapas-red); color: white; border: none; padding: 16px 24px; font-weight: 700; font-size: 14px; cursor: pointer; font-family: inherit; transition: background 0.2s; white-space: nowrap; }
  #chatSendBtn:hover { background: #a02d21; }
  #chatSendBtn:disabled { background: var(--muted); cursor: not-allowed; }
  .dot { width: 8px; height: 8px; background: var(--muted); border-radius: 50%; animation: bounce 1.2s infinite; display: inline-block; }
  .dot:nth-child(2) { animation-delay: 0.2s; }
  .dot:nth-child(3) { animation-delay: 0.4s; }
  @keyframes bounce { 0%,80%,100%{transform:translateY(0)}40%{transform:translateY(-8px)} }
  .chat-typing { display: flex; gap: 6px; align-items: center; padding: 10px 16px; }
  .doc-footer { background: var(--black); color: rgba(255,255,255,0.5); padding: 40px; text-align: center; font-size: 13px; }
  section { scroll-margin-top: calc(var(--nav-h) + var(--tab-h) + 16px); }
  @media (max-width: 640px) {
    .container { padding: 40px 20px; }
    .hero { padding: 60px 20px 40px; }
    .top-nav { padding: 0 16px; }
    .nav-section-btn span { display: none; }
    .cs-body { grid-template-columns: 1fr; }
    .cs-col:first-child { border-right: none; border-bottom: 1px solid var(--border); }
    .top-nav-brand .brand-title { display: none; }
  }
</style>
</head>
<body>

<nav class="top-nav">
  <div class="top-nav-brand">
    <span class="brand-mark">HAPAS</span>
    <span class="brand-title">Digital Marketing Masterclass</span>
  </div>
  <div class="top-nav-sections">
    <button class="nav-section-btn active" onclick="switchView('digital')" id="btn-digital"><span>1</span>Digital Marketing</button>
    <button class="nav-section-btn" onclick="switchView('content')" id="btn-content"><span>2</span>Content Strategy</button>
    <button class="nav-section-btn" onclick="switchView('practice')" id="btn-practice"><span>3</span>Bài Tập & AI Mentor</button>
  </div>
</nav>

<div class="section-tabs" id="tabs-digital">
  <button class="tab-btn active" onclick="scrollToId('intro',event)">Khởi đầu</button>
  <button class="tab-btn" onclick="scrollToId('hapas-story',event)">Câu chuyện HAPAS</button>
  <button class="tab-btn" onclick="scrollToId('foundation',event)">Nền tảng STP</button>
  <button class="tab-btn" onclick="scrollToId('channels',event)">Kênh Digital</button>
  <button class="tab-btn" onclick="scrollToId('case83',event)">Case 8/3</button>
  <button class="tab-btn" onclick="scrollToId('crisis',event)">Quản trị khủng hoảng</button>
  <button class="tab-btn" onclick="scrollToId('funnel',event)">Phễu bán hàng</button>
  <button class="tab-btn" onclick="scrollToId('measurement',event)">Đo lường</button>
  <button class="tab-btn" onclick="scrollToId('roadmap',event)">Lộ trình 90 ngày</button>
</div>
<div class="section-tabs" id="tabs-content" style="display:none">
  <button class="tab-btn active" onclick="scrollToId('content-planning',event)">Content Planning</button>
  <button class="tab-btn" onclick="scrollToId('content-pillar-deep',event)">Content Pillar</button>
  <button class="tab-btn" onclick="scrollToId('content-calendar',event)">Lịch nội dung</button>
  <button class="tab-btn" onclick="scrollToId('storytelling',event)">Storytelling</button>
  <button class="tab-btn" onclick="scrollToId('platform-deep',event)">Platform Strategy</button>
  <button class="tab-btn" onclick="scrollToId('content-performance',event)">Performance</button>
  <button class="tab-btn" onclick="scrollToId('creator-deep',event)">Creator Process</button>
  <button class="tab-btn" onclick="scrollToId('case-compare',event)">So sánh Brand</button>
</div>
<div class="section-tabs" id="tabs-practice" style="display:none">
  <button class="tab-btn active" onclick="scrollToId('exercises-section',event)">6 Bài tập</button>
  <button class="tab-btn" onclick="scrollToId('chat-interface',event)">AI Mentor Chat</button>
</div>

<!-- VIEW 1 -->
<div class="view-panel active" id="view-digital">
  <div class="hero">
    <div class="hero-tag">Bài giảng Digital Marketing</div>
    <h1>Marketing Thật Sự<br>Là <span>Gì?</span></h1>
    <p class="hero-sub">Từ câu chuyện của HAPAS — thương hiệu túi xách Việt từng bán hàng chợ, đổi tên và đạt Top 1 Shopee, Top 1 TikTok Shop — bạn sẽ học toàn bộ bản đồ Digital Marketing từ A tới Z.</p>
    <div class="hero-meta">
      <div class="hero-meta-item"><span class="label">Cấp độ</span><span class="value">Người mới → Thực chiến</span></div>
      <div class="hero-meta-item"><span class="label">Case Study</span><span class="value">HAPAS Việt Nam</span></div>
      <div class="hero-meta-item"><span class="label">Phân tích</span><span class="value">8/3/2026</span></div>
      <div class="hero-meta-item"><span class="label">Giảng viên</span><span class="value">15+ năm kinh nghiệm</span></div>
    </div>
  </div>

  <section id="intro">
  <div class="container">
    <div class="section-header">
      <div class="section-number">00</div>
      <div class="section-title-block"><h2>Trước Khi Bắt Đầu</h2><p class="section-desc">Hãy phá bỏ một quan niệm sai lầm phổ biến nhất</p></div>
    </div>
    <div class="big-quote">"Marketing <span>không phải</span> là đăng bài lên Facebook.<br>Marketing là khiến đúng người, thấy đúng thông điệp, vào đúng lúc — và hành động."</div>
    <p>Hầu hết người mới học marketing đều nhảy thẳng vào câu hỏi <em>"đăng bài gì?"</em> hay <em>"chạy ads thế nào?"</em> — mà bỏ qua phần quan trọng nhất: <strong>tại sao khách hàng phải quan tâm đến bạn?</strong></p>
    <p>Bài giảng này được thiết kế để dạy bạn <strong>tư duy trước, công cụ sau</strong>. Chúng ta sẽ dùng HAPAS — một thương hiệu túi xách Việt Nam đi từ không ai biết đến Top 1 thương mại điện tử — như một tấm gương thực tế để soi vào từng khái niệm.</p>
    <div class="callout gold"><span class="callout-label">Lưu ý từ giảng viên</span><p>Tôi có hơn 15 năm làm marketing thực chiến. Điều tôi thấy người mới thất bại nhiều nhất không phải vì thiếu kỹ năng — mà vì <strong>không hiểu tại sao họ làm thứ họ đang làm</strong>.</p></div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 1</div><h2>Câu Chuyện HAPAS:<br>Từ "Hà Túi" đến Top 1</h2><p>Bài học về Brand Repositioning — khi đổi tên đổi luôn số phận</p></div>

  <section id="hapas-story">
  <div class="container">
    <div class="section-header">
      <div class="section-number">01</div>
      <div class="section-title-block"><h2>Giải Phẫu HAPAS</h2><p class="section-desc">Tại sao một thương hiệu cần "chết đi" để được sinh ra lần nữa</p></div>
    </div>
    <div class="cs-card">
      <div class="cs-image-banner">
        <img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=900&q=80" alt="HAPAS túi xách Việt Nam">
        <div class="cs-image-overlay"></div>
        <div class="cs-image-meta"><span class="cs-brand-name">HAPAS</span><span class="cs-verdict verdict-good">✓ Câu chuyện thành công</span></div>
      </div>
      <div class="cs-links">
        <a class="cs-link" href="https://hapas.vn" target="_blank"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>hapas.vn</a>
        <a class="cs-link" href="https://www.tiktok.com/@hapas.vn" target="_blank"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>TikTok @hapas.vn</a>
        <a class="cs-link" href="https://shopee.vn/hapas_official" target="_blank"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>Shopee Official</a>
        <a class="cs-link" href="https://www.instagram.com/hapas.vn/" target="_blank"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>Instagram</a>
      </div>
      <div class="cs-body">
        <div class="cs-col"><h4>Vấn đề của Hà Túi (trước)</h4><ul><li>Tên gắn với hình ảnh hàng "chợ" — rẻ, đại trà, không phong cách</li><li>Không thể tăng giá vì brand image không phù hợp</li><li>Không thể hợp tác với influencer lớn</li><li>Margin mỏng, cạnh tranh giá với hàng Trung Quốc</li></ul></div>
        <div class="cs-col"><h4>Kết quả sau tái định vị</h4><ul><li>Tăng 147% doanh thu sau 6 tháng đổi thương hiệu</li><li>#1 Shopee ngành túi xách nội địa</li><li>#1 TikTok Shop ngành túi xách</li><li>Collab thành công với Hoa hậu Thùy Tiên</li></ul></div>
      </div>
    </div>
    <div class="stats-row">
      <div class="stat-box highlight"><div class="stat-num">147%</div><div class="stat-label">Tăng trưởng doanh thu sau 6 tháng</div></div>
      <div class="stat-box"><div class="stat-num">#1</div><div class="stat-label">Shopee ngành túi xách nội địa</div></div>
      <div class="stat-box"><div class="stat-num">#1</div><div class="stat-label">TikTok Shop ngành túi xách</div></div>
      <div class="stat-box"><div class="stat-num">15</div><div class="stat-label">Ngày sold out BST Pretty Normal x Thùy Tiên</div></div>
    </div>
    <div class="callout green"><span class="callout-label">Bài học Marketing #1 — Brand Repositioning</span><p><strong>Định vị thương hiệu</strong> là cách khách hàng nhớ đến bạn trong một "ngăn kéo" trong đầu họ. Nếu ngăn kéo đó là "rẻ và thường" — bạn không thể thoát ra bằng cách làm sản phẩm tốt hơn. Bạn cần <em>đập ngăn kéo đó đi và xây cái mới</em>.</p></div>
    <div class="framework">
      <div class="framework-title">4 trụ cột tái định vị của HAPAS</div>
      <div class="framework-grid">
        <div class="framework-item"><span class="fi-label">Sản phẩm</span><div class="fi-value">Da PU cao cấp</div><div class="fi-note">Chọn chất liệu, thiết kế theo concept, ra BST thay vì bán lẻ random</div></div>
        <div class="framework-item"><span class="fi-label">Hình ảnh</span><div class="fi-value">Dynamic Minimalism</div><div class="fi-note">Brand identity "tối giản có năng lượng"</div></div>
        <div class="framework-item"><span class="fi-label">KOL</span><div class="fi-value">Hoa hậu + KOL lifestyle</div><div class="fi-note">Thùy Tiên, Khánh Vân, Châu Bùi — người dùng mơ đến</div></div>
        <div class="framework-item"><span class="fi-label">Kênh bán</span><div class="fi-value">Omnichannel</div><div class="fi-note">Shopee, TikTok Shop, website, cửa hàng vật lý</div></div>
      </div>
    </div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 2</div><h2>Nền Tảng Digital Marketing</h2><p>Trước khi chạy, bạn cần biết mình chạy đi đâu</p></div>

  <section id="foundation">
  <div class="container">
    <div class="section-header">
      <div class="section-number">02</div>
      <div class="section-title-block"><h2>STP — Bộ Ba Vàng</h2><p class="section-desc">Segmentation, Targeting, Positioning</p></div>
    </div>
    <p>Mọi campaign marketing tốt đều bắt đầu từ việc trả lời 3 câu hỏi cơ bản: <strong>Thị trường gồm những ai? Ai là người mình nhắm tới? Mình muốn được nhớ là thương hiệu như thế nào?</strong></p>
    <div class="framework">
      <div class="framework-title">4 cách phân khúc thị trường</div>
      <div class="framework-grid">
        <div class="framework-item"><span class="fi-label">Nhân khẩu học</span><div class="fi-value">Ai?</div><div class="fi-note">Tuổi, giới tính, thu nhập, nghề nghiệp</div></div>
        <div class="framework-item"><span class="fi-label">Địa lý</span><div class="fi-value">Ở đâu?</div><div class="fi-note">Thành phố lớn, tỉnh thành, văn hóa vùng</div></div>
        <div class="framework-item"><span class="fi-label">Tâm lý học</span><div class="fi-value">Nghĩ gì?</div><div class="fi-note">Giá trị sống, lối sống, tính cách</div></div>
        <div class="framework-item"><span class="fi-label">Hành vi</span><div class="fi-value">Làm gì?</div><div class="fi-note">Mua khi nào, mua bao nhiêu, trung thành không</div></div>
      </div>
    </div>
    <div class="case-block"><h4>HAPAS phân khúc thị trường như thế nào?</h4><p>Nữ, 20–35 tuổi • Sinh viên năm 3–4 và nhân viên văn phòng 1–5 năm • Thu nhập 8–20 triệu/tháng, chi 500k–1.5tr cho túi • Sống ở đô thị loại 1–2 • Muốn đẹp và có phong cách nhưng chưa thể mua túi hiệu thật</p></div>
    <div class="callout"><span class="callout-label">Sai lầm phổ biến</span><p>"Target cho tất cả mọi người" = target không ai. Khi bạn nói chuyện với tất cả, bạn không nói chuyện với ai. Brand mạnh nhất là brand khiến một nhóm người cụ thể cảm thấy "thương hiệu này hiểu tôi".</p></div>
    <div class="callout blue"><span class="callout-label">Công thức Positioning Statement</span><p><strong>"Dành cho [target customer], [brand] là [category] duy nhất/tốt nhất [benefit] vì [reason to believe]."</strong><br><br>Của HAPAS: <em>"Dành cho phụ nữ Việt hiện đại muốn sở hữu phong cách cao cấp, HAPAS là thương hiệu túi xách nội địa duy nhất mang đến trải nghiệm mua sắm cao cấp với mức giá phù hợp — vì chúng tôi hiểu điều bình thường cũng có thể tươi đẹp."</em></p></div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 3</div><h2>Hệ Thống Kênh Digital</h2><p>Bạn không cần có mặt ở khắp nơi — bạn cần có mặt đúng chỗ</p></div>

  <section id="channels">
  <div class="container">
    <div class="section-header">
      <div class="section-number">03</div>
      <div class="section-title-block"><h2>Bản Đồ Kênh Digital</h2><p class="section-desc">Owned, Earned, Paid Media — và cách HAPAS dùng cả ba</p></div>
    </div>
    <table class="compare-table">
      <tr><th>Loại kênh</th><th>Là gì?</th><th>Chi phí</th><th>Ví dụ HAPAS</th></tr>
      <tr><td><strong>Owned Media</strong> <span class="badge badge-green">Tự sở hữu</span></td><td>Kênh bạn kiểm soát hoàn toàn</td><td class="good">Thấp</td><td>Website, fanpage, TikTok, email list</td></tr>
      <tr><td><strong>Earned Media</strong> <span class="badge badge-gold">Kiếm được</span></td><td>Người khác nói về bạn miễn phí</td><td class="good">Gần như miễn phí</td><td>Review KH, bài báo, UGC, viral content</td></tr>
      <tr><td><strong>Paid Media</strong> <span class="badge badge-red">Trả tiền</span></td><td>Mua lưu lượng truy cập/hiển thị</td><td class="bad">Chi phí cao</td><td>Facebook Ads, TikTok Ads, Shopee Ads, KOL</td></tr>
    </table>
    <div class="callout"><span class="callout-label">Nguyên tắc vàng</span><p>Doanh nghiệp mới nên xây <strong>Owned Media</strong> trước, dùng <strong>Paid Media</strong> để khuếch đại, và tập trung vào trải nghiệm để tạo ra <strong>Earned Media</strong>.</p></div>
    <div class="case-block"><h4>Bài học từ KOL strategy của HAPAS</h4><p>HAPAS dùng <strong>cả ba tầng KOL</strong>:</p><ul><li><strong>Mega KOL</strong> (Thùy Tiên, Khánh Vân): tạo brand credibility, truyền thông rộng</li><li><strong>Mid-tier KOL</strong> (lifestyle influencer 100k–500k follow): tạo relatability, review chi tiết</li><li><strong>Micro-creator</strong> (UGC từ khách hàng thật): tạo trust, social proof</li></ul></div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 4 — PHÂN TÍCH CHI TIẾT</div><h2>Case Study 8/3/2026<br>HAPAS Làm Gì Đúng?</h2><p>Khi đối thủ "tự bắn vào chân", kẻ đứng im cũng thắng — nếu biết tận dụng</p></div>

  <section id="case83">
  <div class="container">
    <div class="section-header">
      <div class="section-number">04</div>
      <div class="section-title-block"><h2>Giải Mã Mùa 8/3/2026</h2><p class="section-desc">Một bức tranh marketing hoàn chỉnh trong 7 ngày</p></div>
    </div>
    <p>Trước ngày 8/3/2026, thị trường túi xách Việt Nam chứng kiến một "sự cố" lớn: thương hiệu <strong>CHAUTFIFTH</strong> tung chiến dịch "Exploitation" — hình ảnh mang hàm ý bạo lực gia đình. Kết quả: làn sóng tẩy chay ào ạt. Đồng thời, chiến dịch 3CE x Tous les Jours cũng dính scandal tương tự.</p>
    <div class="callout"><span class="callout-label">Điều mà 15 năm marketing dạy tôi</span><p>Trong khủng hoảng của đối thủ, thương hiệu đứng im cũng lên. Nhưng thương hiệu <em>chủ động định vị mình là giải pháp thay thế</em> thì thắng lớn.</p></div>
    <div class="case-block"><h4>Sản phẩm chiến dịch: "Bộ Quà Tặng Hộp Thân Thương 2026"</h4><ul><li><strong>Tên sản phẩm:</strong> "Yêu Chiều" và "Thương Nhớ" — gợi cảm xúc tích cực, gần gũi người Việt</li><li><strong>Bao bì:</strong> Hộp quà cao cấp, tông pastel hoa cỏ, có thể tái sử dụng</li><li><strong>Giá:</strong> 1,683,000đ — đủ "premium" nhưng không quá đắt</li><li><strong>Thông điệp:</strong> "Đừng chỉ nói lời yêu thương — hãy trao đi"</li></ul></div>
    <ul class="checklist">
      <li class="warn">HAPAS chưa có campaign 8/3 đủ <em>viral</em> như chiến dịch 20/10</li>
      <li class="warn">Chưa tận dụng triệt để khoảnh khắc đối thủ sụp đổ để tạo PR wave</li>
      <li class="warn">Giá 1.68tr có thể hơi cao với segment học sinh/sinh viên</li>
    </ul>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 5</div><h2>Quản Trị Khủng Hoảng</h2><p>Khi thương hiệu "bắt lửa" — làm gì để không cháy hết?</p></div>

  <section id="crisis">
  <div class="container">
    <div class="section-header">
      <div class="section-number">05</div>
      <div class="section-title-block"><h2>Bài Học Từ Scandal 8/3</h2><p class="section-desc">CHAUTFIFTH và 3CE — hai case study về "marketing sai"</p></div>
    </div>
    <div class="cs-card">
      <div class="cs-image-banner">
        <img src="https://images.unsplash.com/photo-1553062407-98eeb64c6a62?w=900&q=80" alt="Brand crisis management">
        <div class="cs-image-overlay"></div>
        <div class="cs-image-meta"><span class="cs-brand-name">CHAUTFIFTH</span><span class="cs-verdict verdict-bad">✗ Case học từ sai lầm</span></div>
      </div>
      <div class="cs-links">
        <a class="cs-link" href="https://www.instagram.com/chautfifth/" target="_blank"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>Instagram @chautfifth</a>
      </div>
      <div class="cs-body">
        <div class="cs-col"><h4>Sai lầm chiến lược</h4><ul><li>Nhầm lẫn "gây sốc" là "sáng tạo" — hai thứ hoàn toàn khác nhau</li><li>Target audience (phụ nữ) bị miêu tả tiêu cực trong chính content của thương hiệu</li><li>Im lặng nhiều ngày sau scandal — làm vấn đề tệ hơn gấp đôi</li></ul></div>
        <div class="cs-col"><h4>Bài học rút ra</h4><ul><li>Luôn hỏi: "Content này khiến khách hàng cảm thấy thế nào về bản thân?" — nếu tệ → dừng</li><li>24h đầu quyết định 80% kết quả. Im lặng = đồng ý = tệ hơn</li><li>Reputation tốn năm để xây, một campaign sai có thể phá trong một ngày</li></ul></div>
      </div>
    </div>
    <h3>Quy trình xử lý khủng hoảng đúng</h3>
    <div class="funnel-step"><div class="funnel-icon">1</div><div class="funnel-content"><h4>Thừa nhận ngay — đừng im lặng</h4><p>Trong 24 giờ đầu, im lặng làm vấn đề tệ hơn gấp đôi. 3CE đăng xin lỗi và gỡ content — đúng hướng. CHAUTFIFTH im lặng nhiều ngày — sai nghiêm trọng.</p></div></div>
    <div class="funnel-step"><div class="funnel-icon">2</div><div class="funnel-content"><h4>Xin lỗi không bào chữa</h4><p>Câu xin lỗi tốt: "Chúng tôi đã sai. Content này không phản ánh giá trị của chúng tôi." Tệ nhất: "Xin lỗi nếu ai đó cảm thấy bị xúc phạm" — vẫn đang đổ lỗi cho cảm xúc của người xem.</p></div></div>
    <div class="funnel-step"><div class="funnel-icon">3</div><div class="funnel-content"><h4>Hành động cụ thể</h4><p>Gỡ content vi phạm. Cam kết quy trình duyệt content nghiêm ngặt hơn. Sau 3–6 tháng mới nên ra campaign "comeback".</p></div></div>
    <div class="callout green"><span class="callout-label">Checklist duyệt content</span><p>✓ Content này có tôn trọng đối tượng nó hướng đến không?<br>✓ Thông điệp có phù hợp với giá trị thương hiệu đã cam kết không?<br>✓ Đã test với ít nhất 5 người thuộc đúng target audience chưa?</p></div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 6</div><h2>Phễu Bán Hàng & Hành Trình Khách Hàng</h2></div>

  <section id="funnel">
  <div class="container">
    <div class="section-header">
      <div class="section-number">06</div>
      <div class="section-title-block"><h2>Marketing Funnel Thực Tế</h2><p class="section-desc">HAPAS dẫn dắt khách hàng như thế nào qua từng bước?</p></div>
    </div>
    <div class="big-quote">"Mỗi khách hàng đều bắt đầu từ <span>không biết bạn tồn tại</span>.<br>Nhiệm vụ của marketing là dắt họ đến điểm <span>trung thành</span>."</div>
    <div class="funnel-step"><div class="funnel-icon">A</div><div class="funnel-content"><h4>Awareness — Nhận biết</h4><p>Mục tiêu: khách hàng biết HAPAS tồn tại. Công cụ: TikTok viral, KOL mega, Shopee search ads.</p></div></div>
    <div class="funnel-step"><div class="funnel-icon">I</div><div class="funnel-content"><h4>Interest — Quan tâm</h4><p>Mục tiêu: khách hàng muốn tìm hiểu thêm. Công cụ: review YouTube chi tiết, mid-tier KOL review thật, website đẹp.</p></div></div>
    <div class="funnel-step"><div class="funnel-icon">D</div><div class="funnel-content"><h4>Desire — Mong muốn</h4><p>Mục tiêu: khách hàng MUỐN CÓ sản phẩm. Công cụ: ảnh lifestyle đẹp, limited edition tạo scarcity, collab Hoa hậu.</p></div></div>
    <div class="funnel-step"><div class="funnel-icon">A</div><div class="funnel-content"><h4>Action — Mua hàng</h4><p>Mục tiêu: click "Mua ngay". Công cụ: flash sale, mã giảm giá, review nhiều sao, quy trình thanh toán dễ.</p></div></div>
    <div class="funnel-step"><div class="funnel-icon">R</div><div class="funnel-content"><h4>Retention — Giữ chân</h4><p>Mục tiêu: mua lần 2, lần 3. Công cụ: email/Zalo chăm sóc, chương trình tích điểm, ưu đãi khách hàng thân thiết.</p></div></div>
    <div class="funnel-step"><div class="funnel-icon">L</div><div class="funnel-content"><h4>Loyalty & Advocacy</h4><p>Mục tiêu: khách hàng tự đi giới thiệu người khác. Đây là đỉnh của marketing funnel.</p></div></div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 7</div><h2>Đo Lường & Tối Ưu</h2><p>Nếu bạn không đo, bạn không biết mình có đang tiến không</p></div>

  <section id="measurement">
  <div class="container">
    <div class="section-header">
      <div class="section-number">07</div>
      <div class="section-title-block"><h2>KPI — Đo Cái Gì?</h2><p class="section-desc">Vanity metrics vs. Real metrics</p></div>
    </div>
    <table class="compare-table">
      <tr><th>Giai đoạn Funnel</th><th>KPI thật cần đo</th><th>Vanity metric (đừng bị lừa)</th></tr>
      <tr><td><strong>Awareness</strong></td><td class="good">Reach thực tế, CPM, Brand recall</td><td class="bad">Tổng lượt xem</td></tr>
      <tr><td><strong>Interest</strong></td><td class="good">CTR, Time on site, Bounce rate</td><td class="bad">Lượt like, lượt share</td></tr>
      <tr><td><strong>Desire</strong></td><td class="good">Add to cart rate, Wishlist adds</td><td class="bad">Số follower</td></tr>
      <tr><td><strong>Action</strong></td><td class="good">Conversion rate, CPA, Revenue</td><td class="bad">Doanh số tổng</td></tr>
      <tr><td><strong>Retention</strong></td><td class="good">Repeat purchase rate, LTV, Churn rate</td><td class="bad">Tổng số khách hàng</td></tr>
    </table>
    <div class="framework">
      <div class="framework-title">Bộ ba chỉ số kinh doanh cốt lõi</div>
      <div class="framework-grid">
        <div class="framework-item"><span class="fi-label">CAC</span><div class="fi-value">Chi phí/Khách hàng mới</div><div class="fi-note">= Tổng chi phí Marketing ÷ Số khách hàng mới</div></div>
        <div class="framework-item"><span class="fi-label">LTV</span><div class="fi-value">Giá trị vòng đời KH</div><div class="fi-note">= Giá trị đơn × Số lần mua/năm × Số năm</div></div>
        <div class="framework-item"><span class="fi-label">ROAS</span><div class="fi-value">Doanh thu/Chi phí ads</div><div class="fi-note">ROAS dưới 3 thường là đang lỗ</div></div>
      </div>
    </div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 8 — THỰC CHIẾN</div><h2>Lộ Trình 90 Ngày Đầu</h2><p>Bạn học xong — bây giờ làm gì?</p></div>

  <section id="roadmap">
  <div class="container">
    <div class="section-header">
      <div class="section-number">08</div>
      <div class="section-title-block"><h2>Kế Hoạch Thực Chiến</h2><p class="section-desc">Từng tuần, từng việc cụ thể</p></div>
    </div>
    <div class="action-week"><div class="action-week-header">Tuần 1–2: Xây Nền Tảng <span class="week-tag">Foundation</span></div><div class="action-week-body"><ul><li>Xác định STP rõ ràng bằng văn bản</li><li>Chọn 2 kênh chính — tập trung vào nơi khách hàng của bạn dành nhiều thời gian nhất</li><li>Lập brand identity cơ bản: logo, màu sắc, tone of voice</li><li>Nghiên cứu 3–5 đối thủ: họ đăng gì, tần suất bao nhiêu</li></ul></div></div>
    <div class="action-week"><div class="action-week-header">Tuần 3–4: Tạo Content Đầu Tiên <span class="week-tag">Content Launch</span></div><div class="action-week-body"><ul><li>Xác định 4 Content Pillar cho thương hiệu</li><li>Lên lịch content 30 ngày (ít nhất 3–4 bài/tuần)</li><li>Đăng 10 bài đầu tiên — đừng lo chưa hoàn hảo</li><li>Theo dõi bài nào được tương tác nhiều</li></ul></div></div>
    <div class="action-week"><div class="action-week-header">Tháng 2: Tối Ưu và Khuếch Đại <span class="week-tag">Optimize & Scale</span></div><div class="action-week-body"><ul><li>Phân tích dữ liệu 30 ngày đầu</li><li>Bắt đầu chạy Paid Ads ngân sách nhỏ (200–500k/ngày)</li><li>Tìm 3–5 micro-influencer phù hợp niche</li><li>Thu thập review từ khách hàng đầu tiên</li></ul></div></div>
    <div class="action-week"><div class="action-week-header">Tháng 3: Xây Hệ Thống <span class="week-tag">Systemize</span></div><div class="action-week-body"><ul><li>Tạo Content Calendar 3 tháng tiếp theo</li><li>Scale ad campaigns đang tốt</li><li>Bắt đầu xây email/Zalo list</li><li>Review: CAC, LTV dự kiến, ROAS</li></ul></div></div>
    <ol class="num-list">
      <li><strong>Khách hàng không quan tâm đến sản phẩm của bạn</strong> — họ quan tâm đến vấn đề của họ. Nói về vấn đề của họ trước.</li>
      <li><strong>Consistency hơn Perfection</strong> — đăng đều đặn còn quan trọng hơn đăng hoàn hảo.</li>
      <li><strong>Test, Measure, Optimize</strong> — không có công thức "đúng" cho tất cả.</li>
      <li><strong>Insight sâu > Ngân sách lớn</strong> — HAPAS beat đối thủ lớn hơn vì hiểu khách hàng hơn.</li>
      <li><strong>Marketing không thể cứu sản phẩm xấu</strong> — nếu sản phẩm không tốt, marketing chỉ giúp người ta biết đến sự tệ hại của bạn nhanh hơn.</li>
    </ol>
  </div>
  </section>
  <div class="doc-footer"><p style="margin-bottom:8px;font-size:15px;color:white;"><strong>Phần 1: Digital Marketing Foundation</strong></p><p>Chuyển sang "Content Strategy" hoặc "Bài Tập & AI Mentor" bằng menu phía trên.</p></div>
</div>

<!-- VIEW 2 -->
<div class="view-panel" id="view-content">
  <div class="hero" style="padding:60px 40px 40px;">
    <div class="hero-tag">Chương 10–16</div>
    <h1>Content <span>Strategy</span></h1>
    <p class="hero-sub">Từ lên kế hoạch nội dung đến storytelling, platform, đo lường, và quy trình sản xuất chuyên nghiệp.</p>
  </div>

  <section id="content-planning">
  <div class="container">
    <div class="section-header">
      <div class="section-number">10</div>
      <div class="section-title-block"><h2>Content Planning Là Gì?</h2><p class="section-desc">Và tại sao 90% người làm content đang làm sai từ đầu</p></div>
    </div>
    <div class="big-quote">"Hầu hết thương hiệu <span>thất bại về content</span> không phải vì thiếu ý tưởng — mà vì không biết <span>ý tưởng đó phục vụ mục tiêu gì</span>."</div>
    <div class="callout"><span class="callout-label">Nhận diện bệnh "đăng cho có"</span><p>• Thứ Hai chưa biết tuần này đăng gì<br>• Đăng sản phẩm liên tục, không có câu chuyện<br>• Không biết bài nào hiệu quả vì không có mục tiêu để so sánh<br>• Cảm giác đang "chạy trên máy xay" — làm nhiều mà không đi đến đâu</p></div>
    <div class="framework">
      <div class="framework-title">5 câu hỏi Content Planning phải trả lời</div>
      <div class="framework-grid">
        <div class="framework-item"><span class="fi-label">WHY</span><div class="fi-value">Tại sao?</div><div class="fi-note">Mục tiêu: Awareness? Conversion? Loyalty?</div></div>
        <div class="framework-item"><span class="fi-label">WHO</span><div class="fi-value">Cho ai?</div><div class="fi-note">Ai xem? Đang ở đâu trong funnel?</div></div>
        <div class="framework-item"><span class="fi-label">WHAT</span><div class="fi-value">Nội dung gì?</div><div class="fi-note">Format nào? Thông điệp cốt lõi là gì?</div></div>
        <div class="framework-item"><span class="fi-label">WHERE</span><div class="fi-value">Ở đâu?</div><div class="fi-note">Kênh nào? Adapt format thế nào?</div></div>
        <div class="framework-item"><span class="fi-label">WHEN</span><div class="fi-value">Khi nào?</div><div class="fi-note">Giờ vàng? Gắn với sự kiện nào?</div></div>
      </div>
    </div>
  </div>
  </section>

  <section id="content-pillar-deep">
  <div class="container">
    <div class="section-header">
      <div class="section-number">11</div>
      <div class="section-title-block"><h2>Content Pillar — Trụ Cột Nội Dung</h2><p class="section-desc">Cách xây "bộ khung" để không bao giờ hết ý tưởng</p></div>
    </div>
    <div class="case-block"><h4>HAPAS — 5 Content Pillar thực tế</h4><ul><li><strong>Pillar 1 — Product Hero:</strong> Giới thiệu sản phẩm, BST mới, màu sắc, chi tiết thiết kế</li><li><strong>Pillar 2 — Lifestyle Aspirational:</strong> Người thật dùng túi trong cuộc sống đẹp</li><li><strong>Pillar 3 — Social Proof:</strong> Review thật của khách hàng, unboxing, ảnh check-in</li><li><strong>Pillar 4 — Education/Value:</strong> Cách phối túi, bảo quản da, chọn size</li><li><strong>Pillar 5 — Brand Story & Values:</strong> Hành trình thương hiệu, "Điều bình thường tươi đẹp"</li></ul></div>
    <div class="callout gold"><span class="callout-label">Công thức tỷ lệ Content — Quy tắc 70-20-10</span><p>• <strong>70%</strong> Content tạo giá trị (dạy, giải trí, truyền cảm hứng)<br>• <strong>20%</strong> Content chia sẻ câu chuyện thương hiệu và người dùng (UGC, behind the scenes)<br>• <strong>10%</strong> Content bán hàng trực tiếp (giảm giá, CTA, flash sale)</p></div>
  </div>
  </section>

  <section id="content-calendar">
  <div class="container">
    <div class="section-header">
      <div class="section-number">12</div>
      <div class="section-title-block"><h2>Content Calendar</h2><p class="section-desc">Xây lịch thực tế mà bạn thật sự dùng được</p></div>
    </div>
    <div class="callout"><span class="callout-label">Nguyên tắc lập lịch bền vững</span><p>Bắt đầu từ <strong>50% công suất</strong> bạn nghĩ mình có thể làm. Đăng đều 3 bài/tuần trong 6 tháng > Đăng 7 bài/tuần trong 2 tuần rồi im lặng 3 tháng.</p></div>
    <div class="calendar-grid">
      <div class="cal-month"><div class="cal-month-header">Tháng 1–2</div><div class="cal-month-body"><div class="cal-event"><span class="cal-date">14/2</span><span class="cal-name">Valentine</span><span class="cal-note">Start 3 tuần trước — quà tặng, cặp đôi</span></div><div class="cal-event"><span class="cal-date">Tháng 1</span><span class="cal-name">Tết / Year-end</span><span class="cal-note">Outfit Tết, quà tặng gia đình</span></div></div></div>
      <div class="cal-month"><div class="cal-month-header">Tháng 3–4</div><div class="cal-month-body"><div class="cal-event"><span class="cal-date">8/3</span><span class="cal-name">Quốc tế Phụ nữ</span><span class="cal-note">HIGH SEASON — tôn vinh phụ nữ</span></div><div class="cal-event"><span class="cal-date">3/3, 4/4</span><span class="cal-name">Sale Double Day</span><span class="cal-note">Flash deals trên e-commerce</span></div></div></div>
      <div class="cal-month"><div class="cal-month-header">Tháng 9–10</div><div class="cal-month-body"><div class="cal-event"><span class="cal-date">20/10</span><span class="cal-name">Phụ nữ VN</span><span class="cal-note">HIGH SEASON #2 — bắt đầu từ đầu tháng 10</span></div><div class="cal-event"><span class="cal-date">9/9, 10/10</span><span class="cal-name">Sale Double Day</span><span class="cal-note">Đẩy TikTok Shop, Shopee mạnh nhất</span></div></div></div>
      <div class="cal-month"><div class="cal-month-header">Tháng 11–12</div><div class="cal-month-body"><div class="cal-event"><span class="cal-date">11/11</span><span class="cal-name">Singles' Day</span><span class="cal-note">Self-gifting trend — "tự thưởng bản thân"</span></div><div class="cal-event"><span class="cal-date">12/12, 25/12</span><span class="cal-name">Year-end & Giáng Sinh</span><span class="cal-note">Gift guide, set quà, năm mới</span></div></div></div>
    </div>
    <h3>Template Lịch Tuần Thực Tế</h3>
    <div class="week-template">
      <div class="week-day"><div class="week-day-label">Thứ Hai</div><div class="week-day-content"><span class="pillar-tag pillar-edu">Education</span><p>Bài "Tip/Thủ thuật" — dạy điều hữu ích. VD: "3 cách phối túi đeo chéo với outfit công sở"</p><small>Carousel/Reel 30s | Instagram + TikTok</small></div></div>
      <div class="week-day"><div class="week-day-label">Thứ Tư</div><div class="week-day-content"><span class="pillar-tag pillar-product">Product</span><p>Feature sản phẩm qua câu chuyện. VD: "Chiếc túi đã theo tôi qua 3 cuộc phỏng vấn..."</p><small>Video 45–60s | TikTok + Facebook</small></div></div>
      <div class="week-day"><div class="week-day-label">Thứ Sáu</div><div class="week-day-content"><span class="pillar-tag pillar-social">Social Proof</span><p>Repost review khách hàng, UGC, behind-the-scenes</p><small>Story + Feed post | Instagram + Facebook</small></div></div>
      <div class="week-day"><div class="week-day-label">Chủ Nhật</div><div class="week-day-content"><span class="pillar-tag pillar-lifestyle">Lifestyle</span><p>Content nhẹ nhàng, relatable — gắn với cuộc sống cuối tuần</p><small>Ảnh aesthetic | Instagram + TikTok</small></div></div>
    </div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 11</div><h2>Content Storytelling</h2><p>Tại sao con người mua cảm xúc — và cách tạo ra cảm xúc đó</p></div>

  <section id="storytelling">
  <div class="container">
    <div class="section-header">
      <div class="section-number">13</div>
      <div class="section-title-block"><h2>Nghệ Thuật Kể Chuyện Bán Hàng</h2><p class="section-desc">Câu chuyện kích hoạt 7 vùng não — thông số kỹ thuật chỉ kích hoạt 2</p></div>
    </div>
    <h3>Cấu trúc 5 Act — Framework kể chuyện bán hàng</h3>
    <div class="story-arc">
      <div class="arc-step"><div class="arc-num">1</div><div class="arc-content"><strong>Setup — Bối cảnh</strong><p>Giới thiệu nhân vật và hoàn cảnh. Khán giả phải nhìn thấy mình trong đó.</p></div></div>
      <div class="arc-step"><div class="arc-num">2</div><div class="arc-content"><strong>Conflict — Vấn đề / Nỗi đau</strong><p>Điều gì đang làm khó nhân vật? Đây là nơi bạn "chạm vào nỗi đau" của khách hàng.</p></div></div>
      <div class="arc-step"><div class="arc-num">3</div><div class="arc-content"><strong>Rising Action — Hành trình tìm giải pháp</strong><p>Nhân vật thử các giải pháp, thất bại, rồi tìm thấy thứ họ cần.</p></div></div>
      <div class="arc-step"><div class="arc-num">4</div><div class="arc-content"><strong>Climax — Sản phẩm là giải pháp</strong><p>Thương hiệu xuất hiện tự nhiên — không phải "mua ngay" mà là người hùng giải quyết vấn đề.</p></div></div>
      <div class="arc-step"><div class="arc-num">5</div><div class="arc-content"><strong>Resolution — Kết thúc có hậu + CTA</strong><p>Cuộc sống nhân vật tốt hơn như thế nào? Rồi mới đến lời mời hành động nhẹ nhàng.</p></div></div>
    </div>
    <h3>Hook — 3 giây đầu quyết định tất cả</h3>
    <div class="hook-grid">
      <div class="hook-item"><div class="hook-type">Hook Câu Hỏi</div><div class="hook-example">"Bạn đã bao giờ mua túi 2 triệu rồi không dám dùng vì sợ bẩn chưa?"</div><div class="hook-why">Kích hoạt câu trả lời trong đầu người xem ngay lập tức</div></div>
      <div class="hook-item"><div class="hook-type">Hook Số Liệu</div><div class="hook-example">"85% phụ nữ Việt sở hữu túi mà chưa tìm được chiếc 'đúng nhất' của mình"</div><div class="hook-why">Tạo tò mò, muốn biết 15% còn lại đã làm gì khác</div></div>
      <div class="hook-item"><div class="hook-type">Hook Ngược đời</div><div class="hook-example">"Đừng mua túi đắt tiền nếu bạn chưa đọc bài này"</div><div class="hook-why">Kích thích trí tò mò, phá vỡ kỳ vọng người xem</div></div>
      <div class="hook-item"><div class="hook-type">Hook Empathy</div><div class="hook-example">"Tôi hiểu cảm giác đứng trước gương 20 phút mà vẫn chưa chọn được túi nào..."</div><div class="hook-why">Người xem cảm thấy "đây là video về mình"</div></div>
      <div class="hook-item"><div class="hook-type">Hook Hứa Hẹn</div><div class="hook-example">"Sau video này bạn sẽ không bao giờ mua nhầm túi nữa"</div><div class="hook-why">Đặt kỳ vọng, người xem muốn đến cuối để nhận giá trị</div></div>
      <div class="hook-item"><div class="hook-type">Hook Visual</div><div class="hook-example">[Mở đầu bằng unboxing ngay lập tức, không nói gì]</div><div class="hook-why">Hành động ngay trong giây đầu — đặc biệt hiệu quả trên TikTok</div></div>
    </div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 12</div><h2>Content Theo Từng Nền Tảng</h2><p>"Đúng nội dung, sai nơi đăng" — sai lầm phổ biến nhất</p></div>

  <section id="platform-deep">
  <div class="container">
    <div class="section-header">
      <div class="section-number">14</div>
      <div class="section-title-block"><h2>Mỗi Platform Là Một Ngôn Ngữ Khác</h2><p class="section-desc">Copy-paste content từ platform này sang platform khác = lãng phí</p></div>
    </div>
    <div class="platform-guide">
      <div class="platform-card"><div class="platform-header tiktok"><span class="platform-icon">🎵</span><strong>TikTok</strong><span class="platform-tag">Giải trí + Khám phá</span></div><div class="platform-body"><p><strong>Thuật toán:</strong> Watch time, Completion rate, Shares. Không cần nhiều follower để viral.</p><p><strong>Content cần:</strong> Hook mạnh 3 giây đầu, kể chuyện qua video, giải trí trước bán hàng sau</p><p class="platform-dont"><strong>Đừng làm:</strong> Video dài >2 phút, quảng cáo đọc script cứng nhắc, watermark từ app khác</p></div></div>
      <div class="platform-card"><div class="platform-header instagram"><span class="platform-icon">📷</span><strong>Instagram</strong><span class="platform-tag">Aspiration + Community</span></div><div class="platform-body"><p><strong>Thuật toán:</strong> Saves (quan trọng nhất!), Shares, Comments chất lượng. Reels được ưu tiên reach mới.</p><p><strong>Content cần:</strong> Hình ảnh aesthetic nhất quán, Reels 30–90s, Stories daily</p><p class="platform-dont"><strong>Đừng làm:</strong> Inconsistent aesthetic, đăng thưa dưới 3 lần/tuần</p></div></div>
      <div class="platform-card"><div class="platform-header facebook"><span class="platform-icon">👥</span><strong>Facebook</strong><span class="platform-tag">Community + Conversion</span></div><div class="platform-body"><p><strong>Thuật toán:</strong> Meaningful interactions, video native, Group posts</p><p><strong>Content cần:</strong> Caption có depth, video native, bài đặt câu hỏi, thông tin hữu ích</p><p class="platform-dont"><strong>Đừng làm:</strong> Cross-post trực tiếp từ Instagram, bài chỉ là ảnh sản phẩm không có câu chuyện</p></div></div>
      <div class="platform-card"><div class="platform-header shopee"><span class="platform-icon">🛒</span><strong>Shopee / TikTok Shop</strong><span class="platform-tag">Conversion + Trust</span></div><div class="platform-body"><p><strong>Người dùng đến để:</strong> Mua hàng. Giai đoạn cuối funnel — đang so sánh và ra quyết định.</p><p><strong>Tối ưu cần:</strong> Ảnh chuẩn, mô tả chi tiết, video sản phẩm 360°, review nhiều sao, flash deal</p><p class="platform-dont"><strong>Đừng làm:</strong> Ảnh mờ nhòe, mô tả thiếu size/màu, không trả lời review</p></div></div>
    </div>
    <h3>Content Repurposing — Làm 1 lần, dùng 5 nơi</h3>
    <div class="repurpose-flow">
      <div class="repurpose-source"><strong>1 Video Interview dài (YouTube — 5–10 phút)</strong></div>
      <div class="repurpose-arrow">↓ Cắt thành</div>
      <div class="repurpose-items">
        <span class="repurpose-item">3–5 clip ngắn 30–60s cho TikTok/Reels</span>
        <span class="repurpose-item">10–15 quotes cho Twitter/Threads</span>
        <span class="repurpose-item">1 bài blog tóm tắt</span>
        <span class="repurpose-item">5–7 Stories Instagram</span>
        <span class="repurpose-item">1 carousel LinkedIn/Facebook</span>
      </div>
    </div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 13</div><h2>Content Performance</h2><p>Làm thế nào để biết content đang hoạt động — hay chỉ đang tồn tại?</p></div>

  <section id="content-performance">
  <div class="container">
    <div class="section-header">
      <div class="section-number">15</div>
      <div class="section-title-block"><h2>4 Cấp Độ Đo Lường Content</h2></div>
    </div>
    <div class="perf-level"><div class="perf-num l1">L1</div><div class="perf-content"><strong>Reach — Bao nhiêu người thấy?</strong><p>Impressions, Reach, Video Views. Dễ thấy nhất nhưng ít ý nghĩa nếu đứng một mình.</p><div class="perf-benchmark">Benchmark HAPAS: TikTok avg 50k+ views, Reels 10k+ reach</div></div></div>
    <div class="perf-level"><div class="perf-num l2">L2</div><div class="perf-content"><strong>Engagement — Người xem có react không?</strong><p><strong>Saves và Shares là chỉ số mạnh nhất</strong> — save = giá trị, share = đồng nhất với.</p><div class="perf-benchmark">Benchmark tốt: ER >3% (Instagram), >5% (TikTok). Dưới 1% = không resonating.</div></div></div>
    <div class="perf-level"><div class="perf-num l3">L3</div><div class="perf-content"><strong>Conversion — Content có dẫn đến hành động không?</strong><p>Click-through rate, Link clicks, Profile visits, Add to cart.</p><div class="perf-benchmark">Benchmark: CTR >1.5% là tốt cho fashion/lifestyle</div></div></div>
    <div class="perf-level"><div class="perf-num l4">L4</div><div class="perf-content"><strong>Revenue — Content có tạo ra tiền không?</strong><p>Revenue attributed to content, Content ROI. Khó đo nhất nhưng quan trọng nhất.</p><div class="perf-benchmark">Tool cần: UTM tracking links, Shopee/TikTok Shop analytics, Google Analytics</div></div></div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 14</div><h2>Content Creator Process</h2><p>Từ "không biết làm gì" đến quy trình sản xuất chuyên nghiệp</p></div>

  <section id="creator-deep">
  <div class="container">
    <div class="section-header">
      <div class="section-number">16</div>
      <div class="section-title-block"><h2>Bộ Công Cụ Tối Thiểu</h2></div>
    </div>
    <div class="big-quote">"Điện thoại 5 triệu + <span>hiểu sâu về khách hàng</span> > Studio 500 triệu + không có gì để nói."</div>
    <div class="framework">
      <div class="framework-title">Starter Kit — Từ 0 đến content chuyên nghiệp</div>
      <div class="framework-grid">
        <div class="framework-item"><span class="fi-label">Quay phim</span><div class="fi-value">Điện thoại bất kỳ</div><div class="fi-note">Thứ quan trọng hơn: ánh sáng tự nhiên và chân máy (150k)</div></div>
        <div class="framework-item"><span class="fi-label">Ánh sáng</span><div class="fi-value">Cửa sổ ban ngày</div><div class="fi-note">Ring light 200k nếu muốn nâng cấp</div></div>
        <div class="framework-item"><span class="fi-label">Edit video</span><div class="fi-value">CapCut (miễn phí)</div><div class="fi-note">Đủ mọi tính năng cần thiết, có template sẵn</div></div>
        <div class="framework-item"><span class="fi-label">Edit ảnh</span><div class="fi-value">Lightroom Mobile</div><div class="fi-note">Lưu preset để chỉnh màu nhất quán</div></div>
        <div class="framework-item"><span class="fi-label">Lên kế hoạch</span><div class="fi-value">Notion / Google Sheet</div><div class="fi-note">Miễn phí, đủ dùng cho team 1–5 người</div></div>
        <div class="framework-item"><span class="fi-label">Analytics</span><div class="fi-value">Native analytics</div><div class="fi-note">TikTok, Instagram Insights, Facebook Insights — miễn phí</div></div>
      </div>
    </div>
    <h3>Quy Trình 5 Bước Sản Xuất Content</h3>
    <div class="process-flow">
      <div class="process-step"><div class="process-num">①</div><div class="process-body"><strong>Brief (5–10 phút)</strong><p>Mục tiêu? Target? Thông điệp chính? Platform? Format? Bước này 90% content creator bỏ qua.</p></div></div>
      <div class="process-step"><div class="process-num">②</div><div class="process-body"><strong>Script/Storyboard (10–15 phút)</strong><p>Viết hook (giây 0–3), điểm chính, CTA. Tiết kiệm 50% thời gian quay.</p></div></div>
      <div class="process-step"><div class="process-num">③</div><div class="process-body"><strong>Production (15–60 phút)</strong><p>Quay nhiều hơn cần. Batch shooting — quay nhiều bài trong 1 lần setup.</p></div></div>
      <div class="process-step"><div class="process-num">④</div><div class="process-body"><strong>Edit + Copy (20–45 phút)</strong><p>Đừng filter quá đà. Caption phải có ít nhất 1 câu hỏi hoặc CTA rõ ràng.</p></div></div>
      <div class="process-step"><div class="process-num">⑤</div><div class="process-body"><strong>Publish + Monitor (5 phút + 48h)</strong><p>Reply tất cả comment trong 1 giờ đầu. Sau 48h: check metrics, ghi vào audit sheet.</p></div></div>
    </div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">Chương 15</div><h2>So Sánh Brand: HAPAS vs Các Brand Lớn</h2><p>Học từ người đã làm — cả đúng lẫn sai</p></div>

  <section id="case-compare">
  <div class="container">
    <div class="section-header">
      <div class="section-number">17</div>
      <div class="section-title-block"><h2>4 Brand, 4 Bài Học Khác Nhau</h2></div>
    </div>
    <div class="cs-card">
      <div class="cs-image-banner"><img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=900&q=80" alt="HAPAS"><div class="cs-image-overlay"></div><div class="cs-image-meta"><span class="cs-brand-name">HAPAS</span><span class="cs-verdict verdict-good">✓ Học điều đúng</span></div></div>
      <div class="cs-links"><a class="cs-link" href="https://hapas.vn" target="_blank"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>hapas.vn</a></div>
      <div class="cs-body">
        <div class="cs-col"><h4>Điều HAPAS làm đúng</h4><ul><li>Brand repositioning dũng cảm: đổi tên + đổi toàn bộ định vị</li><li>Insight từ đời thường: campaign 20/10 dùng insight "đàn ông hay quên tặng quà"</li><li>Product là marketing: hộp quà đẹp khiến khách tự đăng lên mạng</li><li>KOL 3 tầng: Mega → Mid → Micro</li></ul></div>
        <div class="cs-col"><h4>Điểm cần cải thiện</h4><ul><li>Campaign 8/3 chưa có "viral hook" rõ ràng như 20/10</li><li>Chưa xây được community platform sở hữu</li><li>Content education còn ít — là white space lớn</li><li>Retention marketing (email, Zalo OA) chưa tận dụng tốt</li></ul></div>
      </div>
    </div>
    <div class="cs-card">
      <div class="cs-image-banner"><img src="https://images.unsplash.com/photo-1563013544-824ae1b704d3?w=900&q=80" alt="Lemonade"><div class="cs-image-overlay"></div><div class="cs-image-meta"><span class="cs-brand-name">Lemonade</span><span class="cs-verdict verdict-good">✓ Storytelling qua Social Proof</span></div></div>
      <div class="cs-links"><a class="cs-link" href="https://www.lemonade.com" target="_blank"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>lemonade.com</a></div>
      <div class="cs-body">
        <div class="cs-col"><h4>Chiến lược content</h4><ul><li>Zero-jargon: không có từ chuyên ngành bảo hiểm nào — dùng ngôn ngữ người thật</li><li>Real claims, real people: video người dùng claim được giải quyết trong 3 phút</li><li>Transparency storytelling: công khai % tiền dùng cho từng mục đích</li></ul></div>
        <div class="cs-col"><h4>Áp dụng cho thương hiệu bạn</h4><ul><li>Tìm "nỗi sợ sâu nhất" của khách hàng → tạo content trực tiếp giải quyết</li><li>Social proof mạnh nhất = người thật, kết quả thật, không dàn dựng</li><li>Transparency bán được hàng — đặc biệt trong ngành nhiều nghi ngờ</li></ul></div>
      </div>
    </div>
    <div class="cs-card">
      <div class="cs-image-banner"><img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?w=900&q=80" alt="3CE"><div class="cs-image-overlay"></div><div class="cs-image-meta"><span class="cs-brand-name">3CE</span><span class="cs-verdict verdict-mixed">⚠ Học cả đúng lẫn sai</span></div></div>
      <div class="cs-body">
        <div class="cs-col"><h4>Điều 3CE làm đúng</h4><ul><li>Visual Universe nhất quán: hồng nude + trắng kem — ai nhìn vào cũng nhận ra ngay</li><li>Aspirational but attainable: đẹp nhưng fan có thể thấy mình trong đó</li></ul></div>
        <div class="cs-col"><h4>Bài học từ scandal</h4><ul><li>Khi xây được "thế giới quan" mạnh — content phá vỡ nó gây phản ứng gấp đôi</li><li>Crisis response đúng (xin lỗi + gỡ ngay trong 24h) có thể cứu thương hiệu</li></ul></div>
      </div>
    </div>
  </div>
  </section>
  <div class="doc-footer"><p style="margin-bottom:8px;font-size:15px;color:white;"><strong>Phần 2: Content Strategy</strong></p><p>Chuyển sang "Bài Tập & AI Mentor" để thực hành ngay.</p></div>
</div>

<!-- VIEW 3 -->
<div class="view-panel" id="view-practice">
  <div class="hero" style="padding:60px 40px 40px;">
    <div class="hero-tag">Thực hành</div>
    <h1>Bài Tập &<br><span>AI Mentor</span></h1>
    <p class="hero-sub">Kiến thức chỉ có giá trị khi được thực hành. Nộp bài tập và nhận phản hồi từ AI Marketing Mentor ngay trong trang này.</p>
  </div>

  <section id="exercises-section">
  <div class="container">
    <div class="section-header">
      <div class="section-number">18</div>
      <div class="section-title-block"><h2>6 Bài Tập Thực Chiến</h2><p class="section-desc">Làm hết 6 bài này — bạn đã làm được 80% công việc của một content marketer</p></div>
    </div>
    <div class="exercise-card">
      <div class="exercise-header"><span class="exercise-num">Bài 1</span><span class="exercise-title">Xác định Content Pillar cho thương hiệu của bạn</span><span class="exercise-level level-easy">Cơ bản</span></div>
      <div class="exercise-body"><p>Xác định 4–5 Content Pillar, phân bổ tỷ lệ, và viết 3 ý tưởng bài cụ thể cho mỗi Pillar.</p><ol><li>Chọn 1 thương hiệu (của bạn, hoặc giả định)</li><li>Xác định Target Audience cụ thể</li><li>Liệt kê 20 chủ đề có thể làm content</li><li>Nhóm thành 4–5 Pillar, đặt tên và mô tả</li><li>Phân bổ tỷ lệ % cho từng Pillar (tổng = 100%)</li></ol><button class="submit-exercise-btn" onclick="goToChat('Bài tập 1: Xác định Content Pillar')">Nộp bài & Nhận phản hồi từ AI →</button></div>
    </div>
    <div class="exercise-card">
      <div class="exercise-header"><span class="exercise-num">Bài 2</span><span class="exercise-title">Viết Hook cho 5 kiểu content khác nhau</span><span class="exercise-level level-easy">Cơ bản</span></div>
      <div class="exercise-body"><p>Viết 5 hook cho cùng 1 chủ đề, mỗi hook dùng 1 kiểu (Câu hỏi, Số liệu, Ngược đời, Empathy, Hứa hẹn).</p><ol><li>Chọn 1 thương hiệu và 1 chủ đề cụ thể</li><li>Viết 5 hook, mỗi câu 1–2 dòng</li><li>Kèm giải thích ngắn tại sao chọn angle đó</li></ol><button class="submit-exercise-btn" onclick="goToChat('Bài tập 2: Viết 5 Hook')">Nộp bài & Nhận phản hồi từ AI →</button></div>
    </div>
    <div class="exercise-card">
      <div class="exercise-header"><span class="exercise-num">Bài 3</span><span class="exercise-title">Lập Content Calendar 1 tháng</span><span class="exercise-level level-mid">Trung cấp</span></div>
      <div class="exercise-body"><p>Lên lịch thực tế cho tháng tới, đủ ít nhất 12–16 bài, áp dụng quy tắc 70-20-10.</p><ol><li>Xác định sự kiện/ngày lễ trong tháng</li><li>Phân bổ bài theo Pillar và tỷ lệ</li><li>Điền: ngày, Pillar, topic, platform, format</li><li>Chọn 1 "hero content" và brief chi tiết hơn</li></ol><button class="submit-exercise-btn" onclick="goToChat('Bài tập 3: Content Calendar 1 tháng')">Nộp bài & Nhận phản hồi từ AI →</button></div>
    </div>
    <div class="exercise-card">
      <div class="exercise-header"><span class="exercise-num">Bài 4</span><span class="exercise-title">Viết câu chuyện bán hàng theo cấu trúc 5 Act</span><span class="exercise-level level-mid">Trung cấp</span></div>
      <div class="exercise-body"><p>Viết caption bán 1 sản phẩm bằng câu chuyện — không được nói thẳng "mua đi, tốt lắm".</p><ol><li>Chọn 1 sản phẩm cụ thể</li><li>Viết theo 5 Act: Setup → Conflict → Rising Action → Climax → Resolution</li><li>Sản phẩm chỉ xuất hiện ở Climax. Độ dài: 150–250 từ</li><li>Kết thúc bằng CTA không quá "bán hàng"</li></ol><button class="submit-exercise-btn" onclick="goToChat('Bài tập 4: Caption 5 Act Storytelling')">Nộp bài & Nhận phản hồi từ AI →</button></div>
    </div>
    <div class="exercise-card">
      <div class="exercise-header"><span class="exercise-num">Bài 5</span><span class="exercise-title">Phân tích content của một thương hiệu đang làm tốt</span><span class="exercise-level level-mid">Trung cấp</span></div>
      <div class="exercise-body"><p>Chọn 1 thương hiệu Việt Nam, xem 10 bài gần nhất, phân tích top/flop và rút ra bài học.</p><ol><li>Đoán Content Pillar của họ</li><li>Phân tích 3 bài nhiều tương tác nhất</li><li>Phân tích 2 bài tệ nhất: tại sao không hiệu quả?</li><li>Rút ra 3 bài học áp dụng cho thương hiệu của mình</li></ol><button class="submit-exercise-btn" onclick="goToChat('Bài tập 5: Phân tích Content Competitor')">Nộp bài & Nhận phản hồi từ AI →</button></div>
    </div>
    <div class="exercise-card">
      <div class="exercise-header"><span class="exercise-num">Bài 6</span><span class="exercise-title">Xây dựng chiến lược content cho Campaign mùa vụ</span><span class="exercise-level level-hard">Nâng cao</span></div>
      <div class="exercise-body"><p>Bài tổng hợp — mini campaign brief thực sự. Làm tốt = có portfolio xin việc.</p><ol><li><strong>Brief:</strong> Thương hiệu, thời gian, ngân sách, mục tiêu KPI</li><li><strong>Insight:</strong> Tại sao khách hàng sẽ care?</li><li><strong>Big Idea:</strong> Concept sáng tạo trung tâm (1–2 dòng)</li><li><strong>Content Plan:</strong> 3 giai đoạn Teaser → Launch → Close</li><li><strong>Hero Content:</strong> Mô tả chi tiết 1 piece chính</li><li><strong>KOL Plan + Metrics</strong></li></ol><button class="submit-exercise-btn" onclick="goToChat('Bài tập 6: Campaign Strategy')">Nộp bài & Nhận phản hồi từ AI →</button></div>
    </div>
  </div>
  </section>

  <div class="chapter-divider"><div class="chapter-num">AI Mentor</div><h2>Hỏi & Thảo Luận<br>Với Marketing Mentor AI</h2><p>Nộp bài tập, đặt câu hỏi, nhận phản hồi — ngay tại đây</p></div>

  <section id="chat-interface">
  <div class="container">
    <div class="section-header">
      <div class="section-number">AI</div>
      <div class="section-title-block"><h2>Marketing Mentor AI</h2><p class="section-desc">Chấm bài, giải đáp, brainstorm, phân tích case study</p></div>
    </div>
    <div class="chat-disclaimer"><strong>Mentor AI có thể:</strong> Chấm và góp ý bài tập • Giải thích khái niệm khó • Phân tích case study bạn đưa ra • Brainstorm ý tưởng content • Phản biện chiến lược của bạn. <em>Hãy cụ thể khi hỏi — câu hỏi càng rõ, phản hồi càng chất lượng.</em></div>
    <div class="chat-container">
      <div class="chat-messages" id="chatMessages">
        <div class="chat-msg ai-msg">
          <div class="chat-avatar">🎓</div>
          <div class="chat-bubble">
            <p>Xin chào! Tôi là Marketing Mentor AI — ở đây để giúp bạn học Digital Marketing và Content Strategy qua bài giảng này.</p>
            <p>Tôi có thể:</p>
            <ul>
              <li>📝 <strong>Chấm bài tập</strong> — paste bài vào đây và tôi sẽ cho điểm + phân tích chi tiết</li>
              <li>❓ <strong>Giải đáp thắc mắc</strong> về bất kỳ khái niệm nào</li>
              <li>🔍 <strong>Phân tích case study</strong> — đưa tên thương hiệu, tôi giải mã strategy</li>
              <li>💡 <strong>Brainstorm</strong> — cần ý tưởng content cho ngành của bạn? Hỏi tôi</li>
            </ul>
            <p>Bắt đầu từ đâu? 🚀</p>
          </div>
        </div>
      </div>
      <div class="chat-quick-prompts">
        <div class="quick-prompt-label">Câu hỏi gợi ý:</div>
        <button class="quick-prompt" onclick="sendQuickPrompt(this)">Giải thích Content Pillar như tôi 10 tuổi</button>
        <button class="quick-prompt" onclick="sendQuickPrompt(this)">Tôi bán đồ ăn online, Content Pillar của tôi nên là gì?</button>
        <button class="quick-prompt" onclick="sendQuickPrompt(this)">Phân tích tại sao HAPAS thành công trên TikTok Shop</button>
        <button class="quick-prompt" onclick="sendQuickPrompt(this)">Tôi không có ý tưởng content, làm thế nào?</button>
        <button class="quick-prompt" onclick="sendQuickPrompt(this)">Sự khác nhau giữa Instagram và TikTok về content là gì?</button>
        <button class="quick-prompt" onclick="sendQuickPrompt(this)">Cách tính LTV và tại sao quan trọng?</button>
      </div>
      <div class="chat-input-area">
        <textarea id="chatInput" placeholder="Nhập câu hỏi hoặc paste bài tập vào đây... (Shift+Enter xuống dòng, Enter gửi)" rows="3"></textarea>
        <button id="chatSendBtn" onclick="sendMessage()">
          <span id="sendBtnText">Gửi →</span>
          <span id="sendBtnLoading" style="display:none">Đang xử lý...</span>
        </button>
      </div>
    </div>
  </div>
  </section>
  <div class="doc-footer"><p style="margin-bottom:8px;font-size:15px;color:white;"><strong>HAPAS Digital Marketing Masterclass</strong></p><p>Phân tích dựa trên dữ liệu công khai từ các chiến dịch HAPAS (2019–2026). Được biên soạn với 15+ năm kinh nghiệm marketing thực chiến.</p></div>
</div>

<script>
  function switchView(viewName) {
    document.querySelectorAll('.view-panel').forEach(p => p.classList.remove('active'));
    document.getElementById('view-' + viewName).classList.add('active');
    document.querySelectorAll('.nav-section-btn').forEach(b => b.classList.remove('active'));
    document.getElementById('btn-' + viewName).classList.add('active');
    document.querySelectorAll('.section-tabs').forEach(t => t.style.display = 'none');
    document.getElementById('tabs-' + viewName).style.display = 'flex';
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
  function scrollToId(id, e) {
    const el = document.getElementById(id);
    if (el) {
      el.scrollIntoView({ behavior: 'smooth' });
      if (e && e.target) {
        const tabs = e.target.closest('.section-tabs');
        if (tabs) { tabs.querySelectorAll('.tab-btn').forEach(t => t.classList.remove('active')); e.target.classList.add('active'); }
      }
    }
  }
  function goToChat(exerciseName) {
    switchView('practice');
    setTimeout(() => {
      document.getElementById('chat-interface').scrollIntoView({ behavior: 'smooth' });
      setTimeout(() => {
        const input = document.getElementById('chatInput');
        input.value = `Tôi muốn nộp ${exerciseName}. Đây là bài làm của tôi:\n\n[Dán bài tập của bạn vào đây]`;
        input.focus();
      }, 400);
    }, 300);
  }

  const SYSTEM_PROMPT = `Bạn là một Marketing Mentor AI chuyên về Digital Marketing và Content Strategy cho thị trường Việt Nam. Bạn có hơn 15 năm kinh nghiệm thực chiến trong marketing, đặc biệt hiểu sâu về thị trường thương hiệu thời trang Việt Nam, TikTok marketing, và content strategy.

Bạn đang hỗ trợ học viên của một bài giảng digital marketing chi tiết, lấy HAPAS làm case study chính. Bài giảng bao gồm: STP Framework, Content Planning, Content Pillars, Storytelling, Platform Strategy (TikTok, Instagram, Facebook, Shopee), Content Performance, và các case study về HAPAS, Lemonade, 3CE, CHAUTFIFTH.

Vai trò của bạn:
1. CHẤM BÀI TẬP: Khi học viên nộp bài, phân tích chi tiết theo từng tiêu chí, cho điểm 1-10, chỉ ra điểm mạnh, điểm yếu, và cách cải thiện cụ thể
2. GIẢI ĐÁP: Trả lời câu hỏi bằng tiếng Việt đơn giản, dùng ví dụ thực tế từ thị trường Việt Nam
3. PHÂN TÍCH: Khi được đưa case study, phân tích sâu với góc nhìn của một marketing professional
4. BRAINSTORM: Giúp học viên tìm ý tưởng content cụ thể cho ngành của họ
5. PHẢN BIỆN: Thách thức tư duy của học viên, đặt câu hỏi ngược để họ suy nghĩ sâu hơn

Phong cách: thẳng thắn nhưng khuyến khích, dùng ngôn ngữ thực tế không hàn lâm, luôn kèm ví dụ cụ thể, khi chấm bài cho điểm rõ ràng và actionable feedback. Trả lời bằng tiếng Việt.`;

  let conversationHistory = [];
  let isLoading = false;

  function sendQuickPrompt(btn) {
    document.getElementById('chatInput').value = btn.textContent;
    sendMessage();
  }

  async function sendMessage() {
    const input = document.getElementById('chatInput');
    const text = input.value.trim();
    if (!text || isLoading) return;
    isLoading = true;
    const sendBtn = document.getElementById('chatSendBtn');
    document.getElementById('sendBtnText').style.display = 'none';
    document.getElementById('sendBtnLoading').style.display = 'inline';
    sendBtn.disabled = true;
    addMessage('user', text);
    input.value = '';
    conversationHistory.push({ role: 'user', content: text });
    const typingId = addTyping();
    try {
      const res = await fetch('https://api.anthropic.com/v1/messages', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({
          model: 'claude-sonnet-4-20250514',
          max_tokens: 1000,
          system: SYSTEM_PROMPT,
          messages: conversationHistory
        })
      });
      const data = await res.json();
      removeTyping(typingId);
      if (data.content && data.content[0]) {
        const aiText = data.content[0].text;
        conversationHistory.push({ role: 'assistant', content: aiText });
        addMessage('ai', aiText);
      } else {
        addMessage('ai', 'Xin lỗi, có lỗi xảy ra. Vui lòng thử lại.');
      }
    } catch (e) {
      removeTyping(typingId);
      addMessage('ai', 'Không thể kết nối. Vui lòng kiểm tra kết nối mạng và thử lại.');
    }
    isLoading = false;
    sendBtn.disabled = false;
    document.getElementById('sendBtnText').style.display = 'inline';
    document.getElementById('sendBtnLoading').style.display = 'none';
  }

  function addMessage(role, text) {
    const container = document.getElementById('chatMessages');
    const div = document.createElement('div');
    div.className = `chat-msg ${role === 'user' ? 'user-msg' : 'ai-msg'}`;
    div.innerHTML = `<div class="chat-avatar">${role === 'user' ? '👤' : '🎓'}</div><div class="chat-bubble">${fmt(text)}</div>`;
    container.appendChild(div);
    container.scrollTop = container.scrollHeight;
  }

  function fmt(text) {
    return text
      .replace(/\*\*(.*?)\*\*/g, '<strong>$1</strong>')
      .replace(/\*(.*?)\*/g, '<em>$1</em>')
      .replace(/^### (.*?)$/gm, '<h4 style="margin:12px 0 6px;font-size:15px;">$1</h4>')
      .replace(/^## (.*?)$/gm, '<h3 style="margin:14px 0 8px;">$1</h3>')
      .replace(/^- (.*?)$/gm, '<li>$1</li>')
      .replace(/(<li>.*?<\/li>\n?)+/gs, '<ul style="padding-left:18px;margin:8px 0;">$&</ul>')
      .replace(/\n\n/g, '</p><p>')
      .replace(/\n/g, '<br>');
  }

  function addTyping() {
    const container = document.getElementById('chatMessages');
    const id = 'typing-' + Date.now();
    const div = document.createElement('div');
    div.id = id;
    div.className = 'chat-msg ai-msg';
    div.innerHTML = `<div class="chat-avatar">🎓</div><div class="chat-bubble"><div class="chat-typing"><div class="dot"></div><div class="dot"></div><div class="dot"></div></div></div>`;
    container.appendChild(div);
    container.scrollTop = container.scrollHeight;
    return id;
  }

  function removeTyping(id) {
    const el = document.getElementById(id);
    if (el) el.remove();
  }

  document.getElementById('chatInput').addEventListener('keydown', e => {
    if (e.key === 'Enter' && !e.shiftKey) { e.preventDefault(); sendMessage(); }
  });
</script>
</body>
</html>
