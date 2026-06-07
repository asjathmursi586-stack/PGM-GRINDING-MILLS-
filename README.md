# -gems- <!DOCTYPE html>
<html lang="ta">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>NEW PGM GRINDING MILLS | Big Premium Website</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;400;600;700;800&family=Playfair+Display:wght@400;600;700;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            user-select: none;
        }
        body {
            font-family: 'Inter', sans-serif;
            background: #0a0c10;
            color: #f5f0e8;
            line-height: 1.5;
            overflow-x: hidden;
        }
        /* Animated grain texture */
        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('https://www.transparenttextures.com/patterns/grain.png');
            opacity: 0.08;
            pointer-events: none;
            z-index: 0;
        }
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 40px;
            position: relative;
            z-index: 2;
        }
        /* Language Bar */
        .lang-bar {
            display: flex;
            justify-content: flex-end;
            gap: 15px;
            padding: 20px 0;
            border-bottom: 1px solid rgba(255,215,150,0.2);
        }
        .lang-btn {
            background: rgba(20,22,27,0.8);
            backdrop-filter: blur(8px);
            border: 1px solid rgba(230,180,52,0.4);
            padding: 8px 24px;
            border-radius: 60px;
            cursor: pointer;
            font-weight: bold;
            font-size: 1rem;
            color: #f5f0e8;
            transition: 0.3s;
        }
        .lang-btn.active, .lang-btn:hover {
            background: #E6B422;
            color: #0a0c10;
            border-color: #E6B422;
            transform: scale(1.02);
        }
        /* Navbar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 30px 0;
            flex-wrap: wrap;
            gap: 20px;
        }
        .logo h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.2rem;
            font-weight: 900;
            background: linear-gradient(135deg, #FFD966, #E6B422);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            letter-spacing: 1px;
        }
        .logo p {
            font-size: 0.85rem;
            color: #d4af7a;
            letter-spacing: 2px;
        }
        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
            flex-wrap: wrap;
        }
        .nav-links a {
            text-decoration: none;
            color: #f5f0e8;
            font-weight: 600;
            font-size: 1.05rem;
            transition: 0.3s;
            cursor: pointer;
            padding: 5px 0;
        }
        .nav-links a:hover {
            color: #E6B422;
            border-bottom: 2px solid #E6B422;
        }
        /* Hero Section - BIG animation */
        .hero {
            min-height: 90vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: radial-gradient(circle at 30% 20%, rgba(230,180,34,0.12), transparent);
        }
        .hero-content {
            max-width: 900px;
        }
        .hero h2 {
            font-family: 'Playfair Display', serif;
            font-size: 4.2rem;
            font-weight: 900;
            background: linear-gradient(135deg, #FFF0C0, #F3C26B);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: fadeUpScale 1.2s cubic-bezier(0.2, 0.9, 0.4, 1.1);
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 1.3rem;
            color: #e0d4c0;
            max-width: 700px;
            margin: 20px auto;
            animation: fadeUp 1s ease 0.2s both;
        }
        .btn-wa {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: #25D366;
            color: white;
            padding: 16px 38px;
            border-radius: 80px;
            font-weight: bold;
            font-size: 1.1rem;
            text-decoration: none;
            transition: 0.3s;
            box-shadow: 0 10px 25px rgba(37,211,102,0.4);
            animation: fadeUp 1s ease 0.4s both;
        }
        .btn-wa:hover {
            transform: scale(1.05);
            background: #1da15a;
            box-shadow: 0 15px 35px rgba(37,211,102,0.6);
        }
        /* Tabs */
        .tabs {
            display: flex;
            gap: 20px;
            margin: 50px 0 30px;
            border-bottom: 2px solid rgba(230,180,52,0.3);
            padding-bottom: 12px;
            flex-wrap: wrap;
        }
        .tab-btn {
            background: transparent;
            border: none;
            padding: 12px 28px;
            border-radius: 60px;
            cursor: pointer;
            font-weight: bold;
            font-size: 1rem;
            color: #f5f0e8;
            transition: 0.3s;
        }
        .tab-btn.active, .tab-btn:hover {
            background: #E6B422;
            color: #0a0c10;
        }
        .tab-pane {
            display: none;
            animation: fadeUp 0.6s ease;
        }
        .tab-pane.active {
            display: block;
        }
        /* Section Titles */
        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.8rem;
            text-align: center;
            margin: 40px 0 30px;
        }
        .section-title:after {
            content: '';
            display: block;
            width: 100px;
            height: 4px;
            background: #E6B422;
            margin: 15px auto;
            border-radius: 4px;
        }
        /* Product & Service Cards */
        .products-grid, .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 35px;
            margin: 40px 0;
        }
        .glass-card {
            background: rgba(20,22,27,0.7);
            backdrop-filter: blur(12px);
            border-radius: 40px;
            padding: 28px 20px;
            border: 1px solid rgba(230,180,52,0.3);
            transition: all 0.4s cubic-bezier(0.2, 0.9, 0.4, 1.1);
            text-align: center;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeUp 0.7s forwards;
        }
        .glass-card:hover {
            transform: translateY(-12px) scale(1.02);
            border-color: #E6B422;
            box-shadow: 0 30px 40px rgba(230,180,52,0.2);
        }
        .product-image {
            width: 100%;
            height: 220px;
            object-fit: cover;
            border-radius: 28px;
            margin-bottom: 20px;
            background: #2a2c33;
            transition: 0.3s;
        }
        .glass-card h3 {
            font-size: 1.8rem;
            margin-bottom: 12px;
        }
        .price {
            font-weight: bold;
            font-size: 1.4rem;
            color: #FFD966;
            margin: 12px 0;
        }
        .order-now {
            display: inline-block;
            background: #E6B422;
            color: #0a0c10;
            padding: 10px 28px;
            border-radius: 60px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 15px;
            transition: 0.2s;
        }
        .order-now:hover {
            background: #f5c542;
            transform: scale(0.97);
        }
        /* Admin Panel */
        .admin-section {
            background: rgba(20,22,27,0.8);
            backdrop-filter: blur(12px);
            border-radius: 48px;
            padding: 30px;
            margin: 30px 0;
        }
        .admin-actions {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            margin-bottom: 25px;
            align-items: center;
        }
        input, select {
            background: #1e1f25;
            border: 1px solid #E6B422;
            color: white;
            padding: 12px 16px;
            border-radius: 40px;
            font-size: 0.9rem;
            flex: 1;
            min-width: 150px;
        }
        button {
            background: #E6B422;
            color: #0a0c10;
            border: none;
            padding: 10px 22px;
            border-radius: 40px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.2s;
        }
        button:hover {
            background: #f5c542;
            transform: scale(1.02);
        }
        table {
            width: 100%;
            border-collapse: collapse;
            background: rgba(0,0,0,0.5);
            border-radius: 28px;
            overflow: auto;
            display: block;
        }
        th, td {
            padding: 14px 10px;
            text-align: left;
            border-bottom: 1px solid rgba(230,180,52,0.2);
            vertical-align: middle;
        }
        .thumbnail-img {
            width: 55px;
            height: 55px;
            object-fit: cover;
            border-radius: 16px;
        }
        /* About & Address */
        .about {
            background: rgba(0,0,0,0.4);
            border-radius: 48px;
            padding: 45px;
            margin: 60px 0;
            backdrop-filter: blur(5px);
        }
        .address {
            background: rgba(230,180,52,0.1);
            padding: 20px;
            border-radius: 32px;
            margin-top: 20px;
            border-left: 5px solid #E6B422;
        }
        footer {
            text-align: center;
            padding: 40px;
            border-top: 1px solid rgba(255,215,150,0.2);
            margin-top: 60px;
            font-size: 0.9rem;
        }
        @keyframes fadeUpScale {
            from { opacity: 0; transform: translateY(60px) scale(0.9); }
            to { opacity: 1; transform: translateY(0) scale(1); }
        }
        @keyframes fadeUp {
            from { opacity: 0; transform: translateY(40px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @media (max-width: 800px) {
            .container { padding: 0 20px; }
            .hero h2 { font-size: 2.5rem; }
            .navbar { flex-direction: column; text-align: center; }
            .lang-bar { justify-content: center; }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="lang-bar">
        <button class="lang-btn active" data-lang="ta">தமிழ்</button>
        <button class="lang-btn" data-lang="en">English</button>
        <button class="lang-btn" data-lang="si">සිංහල</button>
    </div>
    <nav class="navbar">
        <div class="logo">
            <h1 id="shopName">NEW PGM GRINDING MILLS</h1>
            <p id="tagline">Premium Quality Since 1995</p>
        </div>
        <ul class="nav-links">
            <li><a id="navHome">🏠 முகப்பு</a></li>
            <li><a id="navProducts">📦 பொருட்கள்</a></li>
            <li><a id="navServices">🛠️ சேவைகள்</a></li>
            <li><a id="navAdmin">🔐 நிர்வாகம்</a></li>
        </ul>
    </nav>
</div>

<section class="hero">
    <div class="container">
        <div class="hero-content">
            <h2 id="heroTitle">மாவு அரைப்பதில் <br> நம்பிக்கையின் சின்னம்</h2>
            <p id="heroDesc">Freshly ground flours, pulses & specialty grains – traditional taste with modern hygiene.</p>
            <a href="https://wa.me/94786861074" class="btn-wa" target="_blank" id="heroWaBtn">
                <i class="fab fa-whatsapp"></i> <span>WhatsApp இல் ஆர்டர் செய்க</span>
            </a>
        </div>
    </div>
</section>

<div class="container">
    <!-- Products Tab -->
    <div id="productsTab" class="tab-pane active">
        <h2 id="productsTitle" class="section-title">✨ எங்கள் பொருட்கள்</h2>
        <div id="productsList" class="products-grid"></div>
    </div>

    <!-- Services Tab -->
    <div id="servicesTab" class="tab-pane">
        <h2 id="servicesTitle" class="section-title">⚙️ எங்கள் சேவைகள்</h2>
        <div id="servicesList" class="services-grid"></div>
    </div>

    <!-- Admin Tab -->
    <div id="adminTab" class="tab-pane">
        <div class="admin-section">
            <h3 id="adminHeading" style="font-size:1.8rem; margin-bottom:20px;">📦 பொருட்கள் நிர்வாகம் (படங்களுடன்)</h3>
            <div class="admin-actions">
                <input type="text" id="newProdName" placeholder="பெயர்">
                <input type="text" id="newProdPrice" placeholder="விலை (₹45/kg)">
                <input type="text" id="newProdStock" placeholder="கையிருப்பு">
                <input type="text" id="newProdDesc" placeholder="விளக்கம்">
                <input type="file" id="newProdImage" accept="image/*">
                <button id="addProductBtn">➕ சேர்</button>
            </div>
            <div class="admin-actions">
                <button id="exportCsvBtn">📎 CSV எக்ஸ்போர்ட்</button>
                <label for="csvImport" style="background:#E6B422; padding:10px 22px; border-radius:40px; cursor:pointer;">📂 CSV இறக்குமதி</label>
                <input type="file" id="csvImport" accept=".csv" style="display:none">
                <button id="resetDefaultBtn">⟳ முன்னிருப்பு தரவு</button>
            </div>
            <div style="overflow-x:auto;">
                <table id="productTable">
                    <thead><tr><th>#</th><th>படம்</th><th>பெயர்</th><th>விலை</th><th>கையிருப்பு</th><th>விளக்கம்</th><th>செயல்</th></tr></thead>
                    <tbody id="productTableBody"></tbody>
                </table>
            </div>
            <p id="adminMsg" style="color:#FFD966; margin-top:20px;"></p>
        </div>
    </div>

    <!-- About & Address -->
    <div class="about">
        <h3 id="aboutHeading" style="font-size:2rem;">🏭 NEW PGM GRINDING MILLS</h3>
        <p id="aboutDesc" style="margin:15px 0;">25+ வருட அனுபவம், பேறுவளை, களுத்துறை. இயற்கை முறை கல் அரைப்பு.</p>
        <div class="address">
            <i class="fas fa-map-marker-alt" style="color:#E6B422;"></i> <strong id="addrLabel">முகவரி:</strong> <span id="addressText">பேறுவளை, களுத்துறை மாவட்டம், இலங்கை</span>
        </div>
        <p style="margin-top:15px;">📞 <span id="contactLabel">தொடர்புக்கு:</span> +94 78 686 1074</p>
    </div>

    <footer>
        <p id="footerText">© 2025 NEW PGM GRINDING MILLS | பேறுவளை, களுத்துறை | All Rights Reserved</p>
    </footer>
</div>

<script>
    // ---------- Anti Theft ----------
    document.addEventListener('contextmenu', e => { e.preventDefault(); alert("⚠️ Content protected"); });
    document.addEventListener('keydown', e => {
        if(e.ctrlKey && (e.key==='c'||e.key==='x'||e.key==='v')) { e.preventDefault(); alert("Copy disabled"); }
        if(e.key==='F12'||(e.ctrlKey&&e.shiftKey&&e.key==='I')) { e.preventDefault(); alert("Dev tools disabled"); }
    });
    window.addEventListener('dragstart', e => e.preventDefault());

    // ---------- Data ----------
    let products = [];
    const DEFAULT_PRODUCTS = [
        { id: 1, name: "கோதுமை மாவு", price: "₹45/kg", stock: "100kg", description: "100% தூய கோதுமை, கல் அரைப்பு", imageBase64: "" },
        { id: 2, name: "ராகி மாவு", price: "₹70/kg", stock: "80kg", description: "நார்ச்சத்து நிறைந்தது", imageBase64: "" },
        { id: 3, name: "சோள மாவு", price: "₹55/kg", stock: "60kg", description: "மரபு உணவுகளுக்கு", imageBase64: "" },
        { id: 4, name: "அரிசி மாவு", price: "₹60/kg", stock: "120kg", description: "இடியாப்பம், புட்டுக்கு", imageBase64: "" }
    ];
    const DEFAULT_SERVICES = [
        { name: "தனிப்பயன் அரைப்பு", desc: "உங்கள் தானியங்களைக் கொண்டு வந்து அரைக்கலாம்", price: "₹5/kg" },
        { name: "வீட்டு டெலிவரி", desc: "5 கிலோவுக்கு மேல் இலவச டெலிவரி (5km)", price: "" },
        { name: "மொத்த விற்பனை", desc: "உணவகங்களுக்கு சிறப்பு விலை", price: "" }
    ];

    function saveProducts() { localStorage.setItem("pgm_big_products", JSON.stringify(products)); }
    function loadProducts() {
        const stored = localStorage.getItem("pgm_big_products");
        if(stored) products = JSON.parse(stored);
        else products = JSON.parse(JSON.stringify(DEFAULT_PRODUCTS));
    }
    function resetToDefault() { products = JSON.parse(JSON.stringify(DEFAULT_PRODUCTS)); saveProducts(); renderProductTable(); renderProductsPage(); showAdminMsg("Default products loaded."); }

    function resizeAndGetBase64(file, callback) {
        const reader = new FileReader();
        reader.onload = function(e) {
            const img = new Image();
            img.onload = function() {
                const canvas = document.createElement('canvas');
                let width = img.width, height = img.height;
                const maxSize = 300;
                if(width > height) { if(width > maxSize) { height *= maxSize/width; width = maxSize; } }
                else { if(height > maxSize) { width *= maxSize/height; height = maxSize; } }
                canvas.width = width; canvas.height = height;
                const ctx = canvas.getContext('2d');
                ctx.drawImage(img, 0, 0, width, height);
                const base64 = canvas.toDataURL('image/jpeg', 0.7);
                callback(base64);
            };
            img.src = e.target.result;
        };
        reader.readAsDataURL(file);
    }

    function renderProductTable() {
        const tbody = document.getElementById('productTableBody');
        if(!tbody) return;
        tbody.innerHTML = '';
        products.forEach((p, idx) => {
            const row = tbody.insertRow();
            row.insertCell(0).innerText = idx+1;
            const imgCell = row.insertCell(1);
            const imgPreview = document.createElement('img');
            imgPreview.src = p.imageBase64 || 'https://via.placeholder.com/60?text=No+Img';
            imgPreview.className = 'thumbnail-img';
            const fileInput = document.createElement('input');
            fileInput.type = 'file'; fileInput.accept = 'image/*'; fileInput.style.marginTop='5px';
            fileInput.addEventListener('change', (e) => {
                if(e.target.files[0]) resizeAndGetBase64(e.target.files[0], (b64) => { p.imageBase64 = b64; saveProducts(); renderProductTable(); renderProductsPage(); showAdminMsg("Image updated"); });
            });
            const clearBtn = document.createElement('button'); clearBtn.innerText = 'Clear'; clearBtn.style.marginLeft='5px'; clearBtn.style.padding='2px 8px';
            clearBtn.onclick = () => { p.imageBase64 = ''; saveProducts(); renderProductTable(); renderProductsPage(); showAdminMsg("Image removed"); };
            imgCell.appendChild(imgPreview); imgCell.appendChild(document.createElement('br')); imgCell.appendChild(fileInput); imgCell.appendChild(clearBtn);
            
            const nameInput = document.createElement('input'); nameInput.value = p.name;
            row.insertCell(2).appendChild(nameInput);
            const priceInput = document.createElement('input'); priceInput.value = p.price;
            row.insertCell(3).appendChild(priceInput);
            const stockInput = document.createElement('input'); stockInput.value = p.stock;
            row.insertCell(4).appendChild(stockInput);
            const descInput = document.createElement('input'); descInput.value = p.description;
            row.insertCell(5).appendChild(descInput);
            
            const actionCell = row.insertCell(6);
            const saveBtn = document.createElement('button'); saveBtn.innerText = '💾 சேமி';
            saveBtn.onclick = () => { p.name = nameInput.value; p.price = priceInput.value; p.stock = stockInput.value; p.description = descInput.value; saveProducts(); renderProductTable(); renderProductsPage(); showAdminMsg("Saved"); };
            const delBtn = document.createElement('button'); delBtn.innerText = '🗑️'; delBtn.style.marginLeft='8px'; delBtn.style.background='#a13e0c';
            delBtn.onclick = () => { products = products.filter(pr => pr.id !== p.id); saveProducts(); renderProductTable(); renderProductsPage(); showAdminMsg("Deleted"); };
            actionCell.appendChild(saveBtn); actionCell.appendChild(delBtn);
        });
    }

    function addNewProduct() {
        const name = document.getElementById('newProdName').value.trim();
        const price = document.getElementById('newProdPrice').value.trim();
        const stock = document.getElementById('newProdStock').value.trim();
        const desc = document.getElementById('newProdDesc').value.trim();
        const file = document.getElementById('newProdImage').files[0];
        if(!name) { showAdminMsg("பெயர் கட்டாயம்"); return; }
        const newId = Date.now();
        const newProduct = { id: newId, name, price: price || "₹0", stock: stock || "0", description: desc || "", imageBase64: "" };
        if(file) {
            resizeAndGetBase64(file, (b64) => {
                newProduct.imageBase64 = b64;
                products.push(newProduct);
                saveProducts();
                renderProductTable(); renderProductsPage();
                showAdminMsg("பொருள் சேர்க்கப்பட்டது!");
            });
        } else {
            products.push(newProduct);
            saveProducts();
            renderProductTable(); renderProductsPage();
            showAdminMsg("பொருள் சேர்க்கப்பட்டது!");
        }
        document.getElementById('newProdName').value = '';
        document.getElementById('newProdPrice').value = '';
        document.getElementById('newProdStock').value = '';
        document.getElementById('newProdDesc').value = '';
        document.getElementById('newProdImage').value = '';
    }

    function exportToCSV() {
        let csv = "Name,Price,Stock,Description,ImageBase64\n";
        products.forEach(p => { csv += `"${p.name}","${p.price}","${p.stock}","${p.description}","${p.imageBase64 || ''}"\n`; });
        const blob = new Blob([csv], {type: "text/csv"});
        const a = document.createElement('a'); a.href = URL.createObjectURL(blob); a.download = "products.csv"; a.click();
    }

    function importCSV(file) {
        const reader = new FileReader();
        reader.onload = function(e) {
            const text = e.target.result;
            const lines = text.split("\n");
            const newProducts = [];
            for(let i=1; i<lines.length; i++) {
                if(!lines[i].trim()) continue;
                const parts = lines[i].split(/,(?=(?:(?:[^"]*"){2})*[^"]*$)/).map(s => s.replace(/^"|"$/g, '').trim());
                if(parts.length >= 4) {
                    newProducts.push({ id: Date.now()+i, name: parts[0], price: parts[1], stock: parts[2], description: parts[3], imageBase64: parts[4] || "" });
                }
            }
            if(newProducts.length) { products = newProducts; saveProducts(); renderProductTable(); renderProductsPage(); showAdminMsg(`Imported ${newProducts.length} products.`); }
            else showAdminMsg("Invalid CSV");
        };
        reader.readAsText(file);
    }

    function showAdminMsg(msg) { const el = document.getElementById('adminMsg'); if(el) { el.innerText = msg; setTimeout(()=>el.innerText='',3000); } }

    function renderProductsPage() {
        const container = document.getElementById('productsList');
        if(!container) return;
        if(products.length===0) { container.innerHTML = "<p>⚠️ No products yet. Add from Admin panel.</p>"; return; }
        container.innerHTML = products.map(p => `
            <div class="glass-card">
                <img src="${p.imageBase64 || 'https://via.placeholder.com/300?text=No+Image'}" class="product-image" alt="${escapeHtml(p.name)}">
                <h3>${escapeHtml(p.name)}</h3>
                <p>${escapeHtml(p.description)}</p>
                <div class="price">${escapeHtml(p.price)}</div>
                <div><small>📦 ${escapeHtml(p.stock)}</small></div>
                <a href="https://wa.me/94786861074?text=I want to order ${encodeURIComponent(p.name)} (${p.price})" class="order-now" target="_blank">WhatsApp ஆர்டர்</a>
            </div>
        `).join('');
    }
    function renderServicesPage() {
        const container = document.getElementById('servicesList');
        if(!container) return;
        container.innerHTML = DEFAULT_SERVICES.map(s => `
            <div class="glass-card">
                <i class="fas fa-tools" style="font-size:3rem; color:#E6B422; margin-bottom:15px; display:block;"></i>
                <h3>${escapeHtml(s.name)}</h3>
                <p>${escapeHtml(s.desc)}</p>
                ${s.price ? `<div class="price">${escapeHtml(s.price)}</div>` : ''}
                <a href="https://wa.me/94786861074?text=I need ${encodeURIComponent(s.name)}" class="order-now" target="_blank">WhatsApp விபரம்</a>
            </div>
        `).join('');
    }
    function escapeHtml(str) { return String(str).replace(/[&<>]/g, function(m){ if(m==='&') return '&amp;'; if(m==='<') return '&lt;'; if(m==='>') return '&gt;'; return m;}); }

    // Multilingual
    const langTexts = {
        ta: { shopName:"NEW PGM GRINDING MILLS", tagline:"உயர்தரம் 1995 முதல்", navHome:"🏠 முகப்பு", navProducts:"📦 பொருட்கள்", navServices:"🛠️ சேவைகள்", navAdmin:"🔐 நிர்வாகம்", heroTitle:"மாவு அரைப்பதில் <br> நம்பிக்கையின் சின்னம்", heroDesc:"புதிதாக அரைத்த மாவுகள், தானியங்கள் – பாரம்பரிய சுவையுடன் நவீன தூய்மை.", heroWa:"WhatsApp இல் ஆர்டர் செய்க", productsTitle:"✨ எங்கள் பொருட்கள்", servicesTitle:"⚙️ எங்கள் சேவைகள்", adminHeading:"📦 பொருட்கள் நிர்வாகம் (படங்களுடன்)", aboutHeading:"🏭 NEW PGM GRINDING MILLS", aboutDesc:"25+ வருட அனுபவம், பேறுவளை, களுத்துறை. இயற்கை முறை கல் அரைப்பு.", addrLabel:"முகவரி:", addressText:"பேறுவளை, களுத்துறை மாவட்டம், இலங்கை", contactLabel:"தொடர்புக்கு", footerText:"© 2025 NEW PGM GRINDING MILLS | பேறுவளை, களுத்துறை | All Rights Reserved" },
        en: { shopName:"NEW PGM GRINDING MILLS", tagline:"Premium Quality Since 1995", navHome:"🏠 Home", navProducts:"📦 Products", navServices:"🛠️ Services", navAdmin:"🔐 Admin", heroTitle:"The Trusted Name <br> in Flour Milling", heroDesc:"Freshly ground flours, pulses & specialty grains – traditional taste with modern hygiene.", heroWa:"Order on WhatsApp", productsTitle:"✨ Our Products", servicesTitle:"⚙️ Our Services", adminHeading:"📦 Product Manager (with Images)", aboutHeading:"🏭 NEW PGM GRINDING MILLS", aboutDesc:"25+ years experience, Beruwala, Kalutara. Traditional stone grinding.", addrLabel:"Address:", addressText:"Beruwala, Kalutara District, Sri Lanka", contactLabel:"Contact", footerText:"© 2025 NEW PGM GRINDING MILLS | Beruwala, Kalutara | All Rights Reserved" },
        si: { shopName:"NEW PGM GRINDING MILLS", tagline:"උසස් තත්ත්වය 1995 සිට", navHome:"🏠 මුල් පිටුව", navProducts:"📦 නිෂ්පාදන", navServices:"🛠️ සේවා", navAdmin:"🔐 පරිපාලන", heroTitle:"පිටි ඇඹරීමේ <br> විශ්වාසයේ සංකේතය", heroDesc:"නැවුම්ව අඹරන ලද පිටි, පරිප්පු - නවීන සනීපාරක්ෂාව සමග සම්ප්‍රදායික රසය.", heroWa:"WhatsApp මත ඇණවුම් කරන්න", productsTitle:"✨ අපගේ නිෂ්පාදන", servicesTitle:"⚙️ අපගේ සේවා", adminHeading:"📦 භාණ්ඩ කළමනාකරණය (පින්තූර සහිත)", aboutHeading:"🏭 NEW PGM GRINDING MILLS", aboutDesc:"වසර 25+ ක පළපුරුද්ද, බේරුවල, කළුතර. ස්වභාවික ගල් ඇඹරුම්.", addrLabel:"ලිපිනය:", addressText:"බේරුවල, කළුතර දිස්ත්‍රික්කය, ශ්‍රී ලංකාව", contactLabel:"සම්බන්ධතා", footerText:"© 2025 NEW PGM GRINDING MILLS | බේරුවල, කළුතර | සියලුම හිමිකම් ඇවිරිණි" }
    };
    let currentLang = 'ta';
    function applyLanguage() {
        const t = langTexts[currentLang];
        document.getElementById('shopName').innerText = t.shopName;
        document.getElementById('tagline').innerText = t.tagline;
        document.getElementById('navHome').innerHTML = t.navHome;
        document.getElementById('navProducts').innerHTML = t.navProducts;
        document.getElementById('navServices').innerHTML = t.navServices;
        document.getElementById('navAdmin').innerHTML = t.navAdmin;
        document.getElementById('heroTitle').innerHTML = t.heroTitle;
        document.getElementById('heroDesc').innerText = t.heroDesc;
        document.getElementById('heroWaBtn').querySelector('span').innerText = t.heroWa;
        document.getElementById('productsTitle').innerText = t.productsTitle;
        document.getElementById('servicesTitle').innerText = t.servicesTitle;
        document.getElementById('adminHeading').innerHTML = t.adminHeading;
        document.getElementById('aboutHeading').innerText = t.aboutHeading;
        document.getElementById('aboutDesc').innerText = t.aboutDesc;
        document.getElementById('addrLabel').innerHTML = t.addrLabel;
        document.getElementById('addressText').innerText = t.addressText;
        document.getElementById('contactLabel').innerText = t.contactLabel;
        document.getElementById('footerText').innerHTML = t.footerText;
    }
    document.querySelectorAll('.lang-btn').forEach(btn => {
        btn.addEventListener('click', () => {
            currentLang = btn.getAttribute('data-lang');
            document.querySelectorAll('.lang-btn').forEach(b=>b.classList.remove('active'));
            btn.classList.add('active');
            applyLanguage();
        });
    });

    // Tab switching
    function showTab(tabId) {
        document.getElementById('productsTab').classList.remove('active');
        document.getElementById('servicesTab').classList.remove('active');
        document.getElementById('adminTab').classList.remove('active');
        document.getElementById(tabId).classList.add('active');
        if(tabId === 'adminTab') renderProductTable();
        if(tabId === 'productsTab') renderProductsPage();
        if(tabId === 'servicesTab') renderServicesPage();
    }
    document.getElementById('navHome').addEventListener('click', () => window.scrollTo({ top: 0, behavior: 'smooth' }));
    document.getElementById('navProducts').addEventListener('click', () => showTab('productsTab'));
    document.getElementById('navServices').addEventListener('click', () => showTab('servicesTab'));
    document.getElementById('navAdmin').addEventListener('click', () => showTab('adminTab'));

    // Admin buttons
    document.getElementById('addProductBtn').addEventListener('click', addNewProduct);
    document.getElementById('exportCsvBtn').addEventListener('click', exportToCSV);
    document.getElementById('resetDefaultBtn').addEventListener('click', resetToDefault);
    document.getElementById('csvImport').addEventListener('change', (e) => { if(e.target.files.length) importCSV(e.target.files[0]); e.target.value=''; });

    // Initial load
    loadProducts();
    renderProductTable();
    renderProductsPage();
    renderServicesPage();
    applyLanguage();
    showTab('productsTab');
</script>
</body>
</html>
