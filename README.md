# <!doctype html>
<html lang="bn">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Limon Store — মোবাইল শপ / Mobile Shop</title>
  <meta name="description" content="Limon Store — মোবাইল বিক্রয়, সার্ভিস ও আনুষঙ্গিক পণ্য। বাংলা + English ব্রাউজিং।">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{--bg:#0b1020;--card:#0f1724;--glass:rgba(255,255,255,0.06);--accent1:#ff6b6b;--accent2:#ffd166;--glow:rgba(255,182,87,0.18);--muted:#cbd5e1;font-family:'Poppins',system-ui,Segoe UI,Roboto,Arial}
    *{box-sizing:border-box}
    body{margin:0;background:radial-gradient(1200px 600px at 10% 10%,rgba(255,107,107,0.09),transparent),radial-gradient(900px 500px at 90% 90%,rgba(255,209,102,0.06),transparent),var(--bg);color:#fff}
    .wrap{max-width:1100px;margin:28px auto;padding:20px}
    header{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;align-items:center;gap:14px}
    .logo{width:64px;height:64px;border-radius:14px;background:linear-gradient(135deg,var(--accent1),#7c3aed);display:flex;align-items:center;justify-content:center;font-weight:800;font-size:18px;box-shadow:0 8px 30px var(--glow)}
    nav{display:flex;gap:14px;align-items:center}
    .lang-switch{display:flex;gap:8px}
    .btn{padding:10px 14px;border-radius:12px;border:none;cursor:pointer;font-weight:600}
    .btn.primary{background:linear-gradient(90deg,var(--accent1),#7c3aed);color:#061320;box-shadow:0 8px 30px rgba(124,58,237,0.2)}
    .btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)}
    .hero{display:grid;grid-template-columns:1fr 380px;gap:20px;margin-top:22px;align-items:center}
    .card{background:linear-gradient(180deg,rgba(255,255,255,0.02),rgba(255,255,255,0.01));padding:22px;border-radius:16px;backdrop-filter:blur(4px);box-shadow:0 6px 30px rgba(2,6,23,0.6)}
    h1{margin:0;font-size:28px}
    p.lead{color:var(--muted);margin-top:10px}
    .badges{display:flex;gap:10px;margin-top:14px}
    .badge{padding:8px 10px;border-radius:999px;background:linear-gradient(90deg,rgba(255,255,255,0.03),rgba(255,255,255,0.02));font-weight:600;color:var(--muted)}
    .products{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:18px}
    .product{background:linear-gradient(180deg,rgba(255,255,255,0.015),rgba(255,255,255,0.01));padding:12px;border-radius:12px;text-align:center}
    .product img{max-width:100%;height:160px;object-fit:contain}
    .price{font-weight:700;margin-top:8px}
    .services{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-top:16px}
    .service{padding:12px;border-radius:12px;background:linear-gradient(90deg,rgba(255,255,255,0.02),transparent)}
    footer{margin-top:26px;text-align:center;color:var(--muted);font-size:14px}
    /* contact */
    .contact-row{display:flex;gap:14px;margin-top:16px}
    form{flex:1}
    input,textarea,select{width:100%;padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit;margin-top:8px}
    textarea{min-height:120px}
    /* responsive */
    @media (max-width:980px){.hero{grid-template-columns:1fr}.products{grid-template-columns:repeat(2,1fr)}.services{grid-template-columns:1fr}.product img{height:140px}}
    @media (max-width:560px){.products{grid-template-columns:1fr}.brand .name{display:none}.logo{width:52px;height:52px}}
    /* glamorous accents */
    .glow-card{position:relative;overflow:hidden}
    .glow-card::after{content:"";position:absolute;inset:-40%;background:linear-gradient(120deg,rgba(255,107,107,0.12),rgba(255,209,102,0.08),rgba(124,58,237,0.06));transform:rotate(15deg);filter:blur(60px);opacity:0.9}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">LS</div>
        <div>
          <div class="name" style="font-weight:800">Limon Store</div>
          <div style="color:var(--muted);font-size:13px">মোবাইল & Accessories • Mobile & Accessories</div>
        </div>
      </div>

      <nav>
        <div class="lang-switch">
          <button class="btn ghost" id="bnBtn">বাংলা</button>
          <button class="btn ghost" id="enBtn">English</button>
        </div>
        <button class="btn primary" onclick="toggleContact()" id="contactBtn">যোগাযোগ / Contact</button>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="card glow-card">
          <h1 data-i18n-bn="Limon Store- মোবাইল শপ" data-i18n-en="Limon Store — Mobile Shop">Limon Store — মোবাইল শপ</h1>
          <p class="lead" data-i18n-bn="নতুন ও রিলায়েবল ফোন — আমরা বিক্রি ও সার্ভিস করি." data-i18n-en="New & reliable phones — sales and service.">নতুন ও রিলায়েবল ফোন — আমরা বিক্রি ও সার্ভিস করি.</p>

          <div class="badges">
            <div class="badge" data-i18n-bn="সর্বনিম্ন মূল্য" data-i18n-en="Best Prices">সর্বনিম্ন মূল্য</div>
            <div class="badge" data-i18n-bn="মূল্য নিশ্চিত" data-i18n-en="Warranty">মূল্য নিশ্চিত</div>
            <div class="badge" data-i18n-bn="বিতরণ দ্রুত" data-i18n-en="Fast Delivery">বিতরণ দ্রুত</div>
          </div>

          <div class="products" id="productGrid">
            <!-- product cards inserted by JS -->
          </div>
        </div>

        <aside style="width:100%">
          <div class="card">
            <h3 data-i18n-bn="আমাদের সম্পর্কে" data-i18n-en="About Us">আমাদের সম্পর্কে</h3>
            <p class="lead small" data-i18n-bn="Limon Store-এ আমরা নতুন ও রিকন্ডিশন্ড ফোন বিক্রি করি। ৩ মাস ওয়ারেন্টি এবং বিক্রয়োত্তর সেবা।" data-i18n-en="At Limon Store we sell new & refurbished phones. 3-month warranty & after-sales service.">Limon Store-এ আমরা নতুন ও রিকন্ডিশন্ড ফোন বিক্রি করি। ৩ মাস ওয়ারেন্টি এবং বিক্রয়োত্তর সেবা।</p>

            <h4 style="margin-top:12px" data-i18n-bn="সেবা" data-i18n-en="Services">সেবা</h4>
            <div class="services">
              <div class="service">
                <strong data-i18n-bn="ফোন বিক্রয়" data-i18n-en="Phone Sales">ফোন বিক্রয়</strong>
                <div class="small" data-i18n-bn="নতুন ও রিফারবিশড মডেল।" data-i18n-en="New & refurbished models.">নতুন ও রিফারবিশড মডেল।</div>
              </div>
              <div class="service">
                <strong data-i18n-bn="রিপেয়ার ও সার্ভিস" data-i18n-en="Repair & Service">রিপেয়ার ও সার্ভিস</strong>
                <div class="small" data-i18n-bn="স্ক্রিন, ব্যাটারি, সফটওয়্যার।" data-i18n-en="Screen, battery & software fixes.">স্ক্রিন, ব্যাটারি, সফটওয়্যার।</div>
              </div>
            </div>

            <div style="margin-top:12px">
              <button class="btn primary" onclick="scrollToContact()" data-i18n-bn="অর্ডার দিন" data-i18n-en="Place Order">অর্ডার দিন</button>
            </div>
          </div>

          <div class="card" style="margin-top:14px">
            <h3 data-i18n-bn="যোগাযোগ" data-i18n-en="Contact">যোগাযোগ</h3>
            <div class="small" style="margin-top:8px">📞 +8801XXXXXXXXX</div>
            <div class="small">📍 Dhaka, Bangladesh</div>
            <div class="small">✉️ limon@example.com</div>
          </div>
        </aside>
      </section>

      <section style="margin-top:20px" id="contactSection">
        <div class="card">
          <h2 data-i18n-bn="আমাদের সেবা" data-i18n-en="Our Services">আমাদের সেবা</h2>
          <p class="small" data-i18n-bn="নীচে কিছু জনপ্রিয় সেবার তালিকা।" data-i18n-en="Below are some popular services.">নীচে কিছু জনপ্রিয় সেবার তালিকা।</p>

          <div class="services" style="margin-top:12px">
            <div class="service">
              <strong data-i18n-bn="স্ক্রিন রিপ্লেস" data-i18n-en="Screen Replacement">স্ক্রিন রিপ্লেস</strong>
              <div class="small" data-i18n-bn="অরিজিনাল/অ্যাফটারমার্কেট বিকল্প।" data-i18n-en="Original & aftermarket options.">অরিজিনাল/অ্যাফটারমার্কেট বিকল্প।</div>
            </div>
            <div class="service">
              <strong data-i18n-bn="ব্যাটারি পরিবর্তন" data-i18n-en="Battery Replacement">ব্যাটারি পরিবর্তন</strong>
              <div class="small" data-i18n-bn="খড়া ব্যাটারি সাপ্লাই ও ইনস্টল।" data-i18n-en="Genuine batteries & installation.">খড়া ব্যাটারি সাপ্লাই ও ইনস্টল।</div>
            </div>
          </div>

          <div class="contact-row">
            <form class="card" onsubmit="handleContact(event)">
              <label data-i18n-bn="নাম" data-i18n-en="Name">নাম</label>
              <input id="cname" placeholder="আপনার নাম / Your name" required>

              <label data-i18n-bn="ফোন বা ইমেইল" data-i18n-en="Phone or Email">ফোন বা ইমেইল</label>
              <input id="ccontact" placeholder="+8801... or email@example.com" required>

              <label data-i18n-bn="বিস্তারিত" data-i18n-en="Details">বিস্তারিত</label>
              <textarea id="cmessage" placeholder="আপনি কী চান — সংক্ষেপে লিখুন / Write your request" required></textarea>

              <div style="margin-top:10px;display:flex;gap:10px">
                <button class="btn primary" type="submit" data-i18n-bn="পাঠান" data-i18n-en="Send">পাঠান</button>
                <button type="button" class="btn ghost" onclick="fillDemo()" data-i18n-bn="ডেমো পূরণ" data-i18n-en="Fill Demo">ডেমো পূরণ</button>
              </div>
            </form>

            <div style="width:320px" class="card">
              <h4 data-i18n-bn="অফার" data-i18n-en="Offers">অফার</h4>
              <p class="small" data-i18n-bn="এই মাসে প্রতিটি ফোনে ১০% ছাড়।" data-i18n-en="10% off on all phones this month.">এই মাসে প্রতিটি ফোনে ১০% ছাড়।</p>

              <h4 style="margin-top:10px" data-i18n-bn="কাজের সময়" data-i18n-en="Hours">কাজের সময়</h4>
              <div class="small" data-i18n-bn="সোম — শনি: ১০টা — ৮টা" data-i18n-en="Mon — Sat: 10:00 — 20:00">সোম — শনি: ১০টা — ৮টা</div>
            </div>
          </div>
        </div>
      </section>

    </main>

    <footer>
      © <span id="year"></span> Limon Store — All Rights Reserved
    </footer>
  </div>

  <script>
    // sample products
    const products = [
      {name_bn:'Samsung Galaxy A15', name_en:'Samsung Galaxy A15', price:'৳19,500', img:''},
      {name_bn:'Xiaomi Redmi Note 12', name_en:'Xiaomi Redmi Note 12', price:'৳22,400', img:''},
      {name_bn:'iPhone SE (Refurb)', name_en:'iPhone SE (Refurb)', price:'৳18,800', img:''},
      {name_bn:'Realme C55', name_en:'Realme C55', price:'৳12,900', img:''},
      {name_bn:'OnePlus Nord CE', name_en:'OnePlus Nord CE', price:'৳26,300', img:''},
      {name_bn:'Infinix Note 40', name_en:'Infinix Note 40', price:'৳16,700', img:''}
    ];

    function makeSVGPlaceholder(text){
      return 'data:image/svg+xml;utf8,' + encodeURIComponent(`
        <svg xmlns="http://www.w3.org/2000/svg" width="400" height="300">
          <rect width="100%" height="100%" fill="#0f1724"/>
          <text x="50%" y="50%" fill="#9aa4b2" font-family="Poppins, Arial" font-size="18" dominant-baseline="middle" text-anchor="middle">${text}</text>
        </svg>`);
    }

    const grid = document.getElementById('productGrid');
    products.forEach(p=>{
      const el = document.createElement('div'); el.className='product';
      const img = document.createElement('img'); img.src = makeSVGPlaceholder(p.name_en);
      const title = document.createElement('div'); title.className='title'; title.textContent = p.name_bn + ' / ' + p.name_en;
      const price = document.createElement('div'); price.className='price'; price.textContent = p.price;
      const buy = document.createElement('button'); buy.className='btn primary'; buy.style.marginTop='10px'; buy.textContent='Order / অর্ডার'; buy.onclick = ()=> alert('Thanks! Please contact +8801XXXXXXXXX to place order.');
      el.appendChild(img); el.appendChild(title); el.appendChild(price); el.appendChild(buy);
      grid.appendChild(el);
    });

    // language toggle
    const bnBtn = document.getElementById('bnBtn');
    const enBtn = document.getElementById('enBtn');
    let lang = 'bn';
    function setLang(l){
      lang = l;
      document.querySelectorAll('[data-i18n-bn]').forEach(el=>{
        el.textContent = el.getAttribute('data-i18n-'+l) || el.textContent;
      });
      bnBtn.classList.toggle('primary', l==='bn');
      enBtn.classList.toggle('primary', l==='en');
    }
    bnBtn.onclick = ()=>setLang('bn');
    enBtn.onclick = ()=>setLang('en');
    setLang('bn');

    function scrollToContact(){ document.getElementById('contactSection').scrollIntoView({behavior:'smooth'}); }
    function toggleContact(){ scrollToContact(); }

    function handleContact(e){
      e.preventDefault();
      const name = document.getElementById('cname').value.trim();
      const contact = document.getElementById('ccontact').value.trim();
      const msg = document.getElementById('cmessage').value.trim();
      if(!name||!contact||!msg){ alert('সব ঘর পূরণ করুন / Fill all fields'); return; }
      alert('ধন্যবাদ, '+name+'! আমরা দ্রুত যোগাযোগ করব।
Thank you! We will contact you soon.');
      e.target.reset();
    }
    function fillDemo(){ document.getElementById('cname').value='Limon'; document.getElementById('ccontact').value='+8801XXXXXXXXX'; document.getElementById('cmessage').value='আমি একটি Samsung ফোন অর্ডার করতে চাই। / I want to order a Samsung phone.' }
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>


তৈরি হয়ে গেল — আমি “Limon Store” (ঝলমলে, বাংলা+English, মোবাইল ব্যবসার জন্য) একটি সম্পূর্ণ HTML টেমপ্লেট canvas-এ আপডেট করে দিলাম।

কী করবেন এখন:

Canvas-এ থাকা লিমনের_ওয়েবসাইট.html খুলে দেখুন — সেটিই আপডেট ফাইল।

চাইলে আমি এটাকে GitHub Pages বা Netlify-এ ডিপ্লয় করার স্টেপ-বাই-স্টেপ বাংলা নির্দেশনা লিখে দেব।

বা যদি কোনো কন্টেন্ট (দাম, ফোন নম্বর, লোগো ইত্যাদি) বদলাতে চান, বললেই আমি সরাসরি পরিবর্তন করে দেব।


বলুন, এখন কি আপনাকে ডিপ্লয় করার নির্দেশনা লিখে দিব?
