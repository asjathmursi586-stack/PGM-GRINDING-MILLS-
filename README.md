
<!DOCTYPE html>
<html lang="ta">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Garuvida Gemstone Manager | கல் மேலாண்மை அமைப்பு</title>
    <!-- Bootstrap 5 + Icons + Fonts -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            background: #f8f4e9;
            font-family: 'Segoe UI', 'Poppins', 'Noto Sans Tamil', system-ui;
        }
        .navbar-brand {
            font-weight: bold;
            letter-spacing: 1px;
            background: linear-gradient(135deg, #d4af37, #b8860b);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent !important;
        }
        .gem-hero {
            background: linear-gradient(145deg, #2c2418, #1f1a10);
            border-radius: 2rem;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 20px 30px rgba(0,0,0,0.2);
        }
        .gem-img {
            font-size: 5rem;
            filter: drop-shadow(0 8px 12px gold);
            animation: gentleGlow 2s infinite;
        }
        @keyframes gentleGlow {
            0% { text-shadow: 0 0 5px #ffd966; }
            100% { text-shadow: 0 0 20px #f0b27a; }
        }
        .page {
            display: none;
            animation: fade 0.3s ease;
        }
        .active-page {
            display: block;
        }
        @keyframes fade {
            from { opacity: 0; transform: translateY(10px);}
            to { opacity: 1; transform: translateY(0);}
        }
        .card-gem {
            border-left: 5px solid #d4af37;
            transition: all 0.2s;
            background: white;
        }
        .status-badge {
            font-size: 0.7rem;
            font-weight: bold;
        }
        .btn-whatsapp {
            background-color: #25D366;
            color: white;
            border: none;
        }
        .btn-whatsapp:hover {
            background-color: #128C7E;
            color: white;
        }
        footer {
            background: #1e2a2e;
            color: #cddde0;
        }
        .gold-text {
            color: #b8860b;
        }
        .nav-tabs .nav-link.active {
            background-color: #d4af37;
            color: #1f1a10;
            font-weight: bold;
        }
        .table-responsive {
            border-radius: 1rem;
        }
    </style>
</head>
<body>

<!-- Navigation Bar -->
<nav class="navbar navbar-expand-lg bg-dark navbar-dark shadow-lg sticky-top">
    <div class="container">
        <a class="navbar-brand" href="#"><i class="fas fa-gem me-2"></i>Garuvida <span class="gold-text">GemSphere</span></a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ms-auto">
                <li class="nav-item"><a class="nav-link page-link-nav active" data-page="home" href="#"><i class="fas fa-home"></i> முகப்பு</a></li>
                <li class="nav-item"><a class="nav-link page-link-nav" data-page="purchasing" href="#"><i class="fas fa-shopping-cart"></i> கொள்வனவு</a></li>
                <li class="nav-item"><a class="nav-link page-link-nav" data-page="selling" href="#"><i class="fas fa-chart-line"></i> விற்பனை</a></li>
                <li class="nav-item"><a class="nav-link page-link-nav" data-page="recut" href="#"><i class="fas fa-cut"></i> மறுபதம் (Recut)</a></li>
                <li class="nav-item"><a class="nav-link page-link-nav" data-page="giveaway" href="#"><i class="fas fa-gift"></i> கொடுத்த கற்கள்</a></li>
                <li class="nav-item"><a class="nav-link page-link-nav" data-page="suppliers" href="#"><i class="fas fa-truck"></i> சப்ளையர்கள்</a></li>
            </ul>
        </div>
    </div>
</nav>

<div class="container my-4">
    <!-- ======================= HOME PAGE ======================= -->
    <div id="page-home" class="page active-page">
        <div class="gem-hero text-white p-5 text-center">
            <div class="gem-img">
                <i class="fas fa-gem fa-7x" style="color: #ffd966;"></i>
            </div>
            <h1 class="display-4 fw-bold mt-3" style="font-family: 'Georgia';">Garuvida</h1>
            <p class="lead">உங்கள் நம்பகமான இரத்தின கற்கள் மேலாண்மை தளம் 💎</p>
            <hr class="w-50 mx-auto bg-white">
            <p>துல்லியமான கணக்கீடு, விற்பனை, மறுபதம் & கொடை பதிவுகள்</p>
            <div class="mt-4">
                <i class="fas fa-chart-pie me-3"></i> <i class="fas fa-whatsapp me-3"></i> <i class="fas fa-database"></i>
            </div>
        </div>
        <div class="row mt-5 g-4 text-center">
            <div class="col-md-3"><div class="card p-3 shadow-sm"><i class="fas fa-cart-plus fa-2x gold-text"></i><h5>கொள்வனவு</h5><small>கல் & LOT விவரம்</small></div></div>
            <div class="col-md-3"><div class="card p-3 shadow-sm"><i class="fas fa-money-bill-wave fa-2x gold-text"></i><h5>விற்பனை</h5><small>விலை, வாங்குநர், நாள்</small></div></div>
            <div class="col-md-3"><div class="card p-3 shadow-sm"><i class="fas fa-cut fa-2x gold-text"></i><h5>Recut</h5><small>மறுபதம் செலவு</small></div></div>
            <div class="col-md-3"><div class="card p-3 shadow-sm"><i class="fab fa-whatsapp fa-2x gold-text"></i><h5>WhatsApp</h5><small>தானியங்கு செய்தி</small></div></div>
        </div>
    </div>

    <!-- ======================= PURCHASING PAGE ======================= -->
    <div id="page-purchasing" class="page">
        <div class="d-flex justify-content-between align-items-center flex-wrap">
            <h3><i class="fas fa-shopping-cart gold-text"></i> கல் கொள்வனவு பதிவு</h3>
            <button class="btn btn-dark" data-bs-toggle="modal" data-bs-target="#addStoneModal"><i class="fas fa-plus"></i> புதிய கல் / LOT சேர்</button>
        </div>
        <div class="alert alert-info mt-2"><i class="fas fa-info-circle"></i> ஒவ்வொரு கல்லும் தனித்தனி பதிவு. LOT எனில் ஒரே நேரத்தில் பல கற்களை "LOT" தேர்வு செய்து அளவு குறிப்பிடுக.</div>
        <div class="table-responsive mt-3">
            <table class="table table-bordered table-hover bg-white">
                <thead class="table-dark">
                    <tr><th>ID</th><th>கல் பெயர்</th><th>வடிவம்</th><th>CRT</th><th>வாங்கிய விலை</th><th>சப்ளையர்</th><th>நாள்</th><th>பாக்கி?</th><th>வாக்குறுதி நாள்</th><th>செயல்</th></tr>
                </thead>
                <tbody id="purchaseTableBody"></tbody>
            </table>
        </div>
        <div class="card mt-3"><div class="card-header bg-warning">⏳ செலுத்த வேண்டிய பாக்கிகள் (Pending Dues)</div><div class="card-body" id="dueList"></div></div>
    </div>

    <!-- ======================= SELLING PAGE ======================= -->
    <div id="page-selling" class="page">
        <h3><i class="fas fa-chart-line gold-text"></i> விற்பனை மையம்</h3>
        <div class="row"><div class="col-md-6"><div class="card bg-light mb-3"><div class="card-header"><strong>💰 மொத்த Recut செலவு</strong></div><div class="card-body"><h2 id="totalRecutCostDisplay">₹0</h2><small>வங்கி கணக்கு விவரங்கள் உள்ளடக்கம்</small></div></div></div></div>
        <ul class="nav nav-tabs" id="sellTab" role="tablist">
            <li class="nav-item"><a class="nav-link active" data-bs-toggle="tab" href="#unsoldTab">கையிருப்பு கற்கள்</a></li>
            <li class="nav-item"><a class="nav-link" data-bs-toggle="tab" href="#recutPendingTab">Recut செல்லும் கற்கள்</a></li>
            <li class="nav-item"><a class="nav-link" data-bs-toggle="tab" href="#soldTab">விற்கப்பட்டவை</a></li>
        </ul>
        <div class="tab-content mt-3">
            <div class="tab-pane active" id="unsoldTab"><div class="table-responsive"><table class="table table-sm" id="unsoldTable"><thead><tr><th>கல்</th><th>CRT</th><th>வாங்கிய விலை</th><th>விற்பனை</th><th>Recut அனுப்பு</th></tr></thead><tbody></tbody></table></div></div>
            <div class="tab-pane" id="recutPendingTab"><div class="table-responsive"><table class="table" id="recutPendingTable"><thead><tr><th>கல்</th><th>Recut நிலை</th><th>செயல்</th></tr></thead><tbody></tbody></table></div></div>
            <div class="tab-pane" id="soldTab"><div class="table-responsive"><table class="table" id="soldTable"><thead><tr><th>கல்</th><th>விற்ற விலை</th><th>வாங்குநர்</th><th>பணம் தரும் நாள்</th></tr></thead><tbody></tbody></table></div></div>
        </div>
    </div>

    <!-- ======================= RECUT PAGE ======================= -->
    <div id="page-recut" class="page">
        <h3><i class="fas fa-cut gold-text"></i> மறுபதம் (Recut) மேலாண்மை</h3>
        <p>Recut க்கு அனுப்பப்பட்ட கற்களுக்கு செலவு மற்றும் வங்கி கணக்கு பதிவு செய்க</p>
        <div id="recutStonesList" class="row g-3"></div>
        <div class="card mt-4"><div class="card-header">மொத்த Recut செலவு வரலாறு</div><div class="card-body"><table class="table" id="recutHistoryTable"><thead><tr><th>கல்</th><th>செலவு (₹)</th><th>வங்கி கணக்கு</th></tr></thead><tbody></tbody></table></div></div>
    </div>

    <!-- ======================= GIVEAWAY PAGE ======================= -->
    <div id="page-giveaway" class="page">
        <h3><i class="fas fa-gift gold-text"></i> கற்கள் கொடுத்தல் / வழங்குதல்</h3>
        <div class="row">
            <div class="col-md-6"><h5>✅ கொடுக்க கிடைக்கும் கற்கள்</h5><div id="availableGiveawayList" class="list-group"></div></div>
            <div class="col-md-6"><h5>🎁 ஏற்கனவே கொடுக்கப்பட்ட கற்கள்</h5><div id="givenAwayList" class="list-group"></div></div>
        </div>
    </div>

    <!-- ======================= SUPPLIERS PAGE ======================= -->
    <div id="page-suppliers" class="page">
        <h3><i class="fas fa-truck gold-text"></i> சப்ளையர்கள் & WhatsApp பகிர்வு</h3>
        <div id="suppliersContainer" class="row"></div>
    </div>
</div>

<footer class="text-center p-3 mt-5 small">Garuvida Gem Manager 💎 | தரவுகள் உங்கள் உலாவியில் சேமிக்கப்படும்</footer>

<!-- Add Stone Modal -->
<div class="modal fade" id="addStoneModal" tabindex="-1"><div class="modal-dialog modal-lg"><div class="modal-content"><div class="modal-header bg-dark text-white"><h5>💎 புதிய கல் / LOT பதிவு</h5><button type="button" class="btn-close" data-bs-dismiss="modal"></button></div><div class="modal-body">
    <form id="stoneForm">
        <div class="row"><div class="col-md-6"><label>கல் பெயர்*</label><input type="text" id="stoneName" class="form-control" required></div>
        <div class="col-md-6"><label>வடிவம் (Shape)</label><input type="text" id="shape" class="form-control"></div></div>
        <div class="row mt-2"><div class="col-md-4"><label>CRT / சான்றிதழ்</label><input type="text" id="crt" class="form-control"></div>
        <div class="col-md-4"><label>வாங்கிய விலை (₹)</label><input type="number" id="purchasePrice" class="form-control" required></div>
        <div class="col-md-4"><label>வாங்கிய நாள்</label><input type="date" id="purchaseDate" class="form-control"></div></div>
        <div class="row mt-2"><div class="col-md-6"><label>சப்ளையர் பெயர்*</label><input type="text" id="supplierName" class="form-control" required></div>
        <div class="col-md-6"><label>சப்ளையர் போன்</label><input type="tel" id="supplierPhone" class="form-control"></div></div>
        <div class="form-check mt-2"><input type="checkbox" id="paymentDue" class="form-check-input"><label>பணம் கொடுக்க வேண்டும் (பாக்கி உள்ளது)</label></div>
        <div class="mt-2"><label>வாக்குறுதி நாள் (பணம் தருவதாக கூறிய நாள்)</label><input type="date" id="promisedDate" class="form-control"></div>
        <div class="form-check mt-2"><input type="checkbox" id="isLotCheck"><label class="fw-bold">LOT (ஒரே நேரத்தில் பல கற்கள்)</label> <small>அளவு உள்ளிடுக</small><input type="number" id="lotQuantity" placeholder="கல் எண்ணிக்கை" class="form-control mt-1"></div>
        <div class="modal-footer"><button type="submit" class="btn btn-warning">சேமி & சேர்</button></div>
    </form>
</div></div></div></div>

<!-- Sell Modal -->
<div class="modal fade" id="sellModal" tabindex="-1"><div class="modal-dialog"><div class="modal-content"><div class="modal-header"><h5>விற்பனை விவரம்</h5></div><div class="modal-body"><input type="hidden" id="sellStoneId"><label>விற்ற விலை</label><input type="number" id="sellPrice" class="form-control"><label>வாங்குநர் பெயர்</label><input id="buyerName" class="form-control"><label>வாங்குநர் போன்</label><input id="buyerPhone" class="form-control"><label>பணம் தரும் நாள் (வாக்குறுதி)</label><input type="date" id="soldPromisedDate" class="form-control"></div><div class="modal-footer"><button class="btn btn-success" id="confirmSellBtn">விற்பனை முடி</button></div></div></div></div>

<!-- Giveaway Modal -->
<div class="modal fade" id="giveawayModal" tabindex="-1"><div class="modal-dialog"><div class="modal-content"><div class="modal-header"><h5>கல் கொடுப்பது</h5></div><div class="modal-body"><input type="hidden" id="giveStoneId"><label>பெறுநர் பெயர்</label><input id="receiverName" class="form-control"><label>WhatsApp எண் (10 டிஜிட்)</label><input id="receiverPhone" class="form-control"><label>குறிப்பு (வடிவம்,CRT)</label><textarea id="giveNote" class="form-control" readonly></textarea></div><div class="modal-footer"><button class="btn btn-success" id="sendGiveawayBtn"><i class="fab fa-whatsapp"></i> WhatsApp செய்தி & கொடு</button></div></div></div></div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
<script>
    // ---------- DATA MODEL ----------
    let stones = JSON.parse(localStorage.getItem('garuvida_stones')) || [];

    function saveStones() { localStorage.setItem('garuvida_stones', JSON.stringify(stones)); }

    // helper: generate ID
    function genId() { return Date.now() + '-' + Math.random().toString(36).substr(2, 6); }

    // render all
    function renderAll() {
        renderPurchaseTable();
        renderDuePayments();
        renderSellingPages();
        renderRecutPage();
        renderGiveawayPage();
        renderSuppliersPage();
        updateTotalRecutCost();
    }

    function updateTotalRecutCost() {
        let total = stones.reduce((sum, s) => sum + (s.recutCost ? Number(s.recutCost) : 0), 0);
        document.getElementById('totalRecutCostDisplay').innerHTML = `₹${total.toLocaleString('en-IN')}`;
    }

    // Purchase table
    function renderPurchaseTable() {
        let tbody = document.getElementById('purchaseTableBody');
        tbody.innerHTML = stones.map(s => `<tr><td>${s.id.slice(-6)}</td><td>${s.stoneName}</td><td>${s.shape || '-'}</td><td>${s.crt || '-'}</td><td>₹${s.purchasePrice}</td><td>${s.supplierName}</td><td>${s.purchaseDate || '-'}</td><td>${s.paymentDue ? '✅ பாக்கி' : 'முழுமை'}</td><td>${s.promisedPaymentDate || '-'}</td><td><button class="btn btn-sm btn-outline-danger" onclick="deleteStone('${s.id}')"><i class="fas fa-trash"></i></button></td></tr>`).join('');
    }

    function deleteStone(id) { if(confirm("நீக்க வேண்டுமா?")){ stones = stones.filter(s=>s.id!=id); saveStones(); renderAll(); } }

    function renderDuePayments() {
        let dueStones = stones.filter(s=>s.paymentDue===true && s.status!=='sold');
        let dueList = document.getElementById('dueList');
        if(dueStones.length===0) { dueList.innerHTML='<p class="text-muted">பாக்கி எதுவும் இல்லை ✅</p>'; return; }
        dueList.innerHTML = `<ul class="list-group">${dueStones.map(s=>`<li class="list-group-item d-flex justify-content-between">${s.stoneName} - ₹${s.purchasePrice} (சப்ளையர்: ${s.supplierName}) வாக்குறுதி: ${s.promisedPaymentDate || 'குறிப்பிடவில்லை'} <button class="btn btn-sm btn-success" onclick="markPaid('${s.id}')">பணம் செலுத்தப்பட்டது</button></li>`).join('')}</ul>`;
    }
    window.markPaid = (id) => { let stone = stones.find(s=>s.id===id); if(stone){ stone.paymentDue = false; saveStones(); renderAll(); } };

    // Selling Page
    function renderSellingPages() {
        let unsold = stones.filter(s=> s.status === 'in_stock');
        let recutPending = stones.filter(s=> s.status === 'recut_pending');
        let sold = stones.filter(s=> s.status === 'sold');
        let unsoldTable = document.querySelector('#unsoldTable tbody');
        unsoldTable.innerHTML = unsold.map(s=>`<tr><td>${s.stoneName} (${s.shape||'-'}) CRT:${s.crt||'-'}</td><td>${s.crt}</td><td>₹${s.purchasePrice}</td><td><button class="btn btn-sm btn-primary" onclick="openSellModal('${s.id}')">விற்க</button></td><td><button class="btn btn-sm btn-warning" onclick="sendToRecut('${s.id}')">Recut அனுப்பு</button></td></tr>`).join('');
        let recutTable = document.querySelector('#recutPendingTable tbody');
        recutTable.innerHTML = recutPending.map(s=>`<tr><td>${s.stoneName}</td><td>Recut செயல்பாட்டில்...</td><td><button class="btn btn-info btn-sm" onclick="locationToRecutPageAndFocus('${s.id}')">Recut செலவு சேர்</button></td></tr>`).join('');
        let soldTable = document.querySelector('#soldTable tbody');
        soldTable.innerHTML = sold.map(s=>`<tr><td>${s.stoneName}</td><td>₹${s.soldPrice || '-'}</td><td>${s.soldTo || '-'}</td><td>${s.soldPromisedDate || '-'}</td></tr>`).join('');
    }
    window.openSellModal = (id) => {
        window.currentSellId = id;
        let modal = new bootstrap.Modal(document.getElementById('sellModal'));
        modal.show();
    };
    document.getElementById('confirmSellBtn').onclick = () => {
        let id = window.currentSellId;
        let stone = stones.find(s=>s.id===id);
        if(stone && stone.status==='in_stock'){
            stone.status = 'sold';
            stone.soldPrice = document.getElementById('sellPrice').value;
            stone.soldTo = document.getElementById('buyerName').value;
            stone.soldToPhone = document.getElementById('buyerPhone').value;
            stone.soldPromisedDate = document.getElementById('soldPromisedDate').value;
            stone.soldDate = new Date().toISOString().slice(0,10);
            saveStones();
            renderAll();
            bootstrap.Modal.getInstance(document.getElementById('sellModal')).hide();
        }
    };
    window.sendToRecut = (id) => {
        let stone = stones.find(s=>s.id===id);
        if(stone && stone.status==='in_stock'){
            stone.status = 'recut_pending';
            stone.recutCost = stone.recutCost || 0;
            saveStones();
            renderAll();
            alert(`${stone.stoneName} Recut பக்கத்திற்கு அனுப்பப்பட்டது. அங்கு செலவு பதிவு செய்யவும்.`);
        }
    };
    window.locationToRecutPageAndFocus = (id) => { 
        document.querySelectorAll('.page-link-nav')[3].click(); 
        setTimeout(()=>{ document.getElementById(`recut-card-${id}`)?.scrollIntoView({behavior:'smooth'}); },200);
    };

    // Recut Page
    function renderRecutPage() {
        let recutList = stones.filter(s=> s.status === 'recut_pending');
        let container = document.getElementById('recutStonesList');
        if(recutList.length===0) container.innerHTML = '<div class="alert alert-secondary">Recut க்கு அனுப்பிய கற்கள் இல்லை</div>';
        else {
            container.innerHTML = recutList.map(s=>`<div class="col-md-6" id="recut-card-${s.id}"><div class="card"><div class="card-body"><h5>${s.stoneName} (${s.shape})</h5><p>CRT: ${s.crt} | வாங்கிய விலை: ₹${s.purchasePrice}</p><input type="number" id="recutCost_${s.id}" class="form-control mb-2" placeholder="Recut செலவு (₹)"><input type="text" id="recutBank_${s.id}" class="form-control mb-2" placeholder="வங்கி கணக்கு விவரம்"><button class="btn btn-success" onclick="completeRecut('${s.id}')">Recut நிறைவு & கையிருப்புக்கு சேர்</button></div></div></div>`).join('');
        }
        let recutHistory = stones.filter(s=>s.recutCost && s.recutCost>0);
        let historyBody = document.querySelector('#recutHistoryTable tbody');
        historyBody.innerHTML = recutHistory.map(s=>`<tr><td>${s.stoneName}</td><td>₹${s.recutCost}</td><td>${s.recutBankAccount || '-'}</td></tr>`).join('');
    }
    window.completeRecut = (id) => {
        let stone = stones.find(s=>s.id===id);
        if(stone){
            let cost = document.getElementById(`recutCost_${id}`).value;
            let bank = document.getElementById(`recutBank_${id}`).value;
            if(cost && !isNaN(cost)) stone.recutCost = (stone.recutCost || 0) + Number(cost);
            else stone.recutCost = stone.recutCost || 0;
            stone.recutBankAccount = bank;
            stone.status = 'in_stock';
            saveStones();
            renderAll();
            alert(`${stone.stoneName} recut முடிந்தது. மொத்த recut செலவு: ₹${stone.recutCost}`);
        }
    };

    // Giveaway
    function renderGiveawayPage() {
        let available = stones.filter(s=> s.status === 'in_stock');
        let given = stones.filter(s=> s.status === 'given_away');
        let availDiv = document.getElementById('availableGiveawayList');
        availDiv.innerHTML = available.map(s=>`<div class="list-group-item d-flex justify-content-between"><div><strong>${s.stoneName}</strong> (${s.shape}) CRT:${s.crt} ₹${s.purchasePrice}</div><button class="btn btn-sm btn-outline-success" onclick="openGiveawayModal('${s.id}')">கொடு & WhatsApp</button></div>`).join('');
        let givenDiv = document.getElementById('givenAwayList');
        givenDiv.innerHTML = given.map(s=>`<div class="list-group-item bg-light">${s.stoneName} → ${s.givenTo || '?'} (${s.givenToPhone}) நாள்:${s.givenDate}</div>`).join('');
    }
    window.openGiveawayModal = (id) => {
        let stone = stones.find(s=>s.id===id);
        if(stone){
            document.getElementById('giveStoneId').value = id;
            document.getElementById('receiverName').value = '';
            document.getElementById('receiverPhone').value = '';
            let note = `✨ கல் விவரம்: ${stone.stoneName}\nவடிவம்: ${stone.shape}\nCRT: ${stone.crt}\nமதிப்பு: ₹${stone.purchasePrice}\nவணக்கம், இந்த கல்லை உங்களுக்கு வழங்குகிறேன். நன்றி! - Garuvida`;
            document.getElementById('giveNote').value = note;
            new bootstrap.Modal(document.getElementById('giveawayModal')).show();
        }
    };
    document.getElementById('sendGiveawayBtn').onclick = () => {
        let stoneId = document.getElementById('giveStoneId').value;
        let stone = stones.find(s=>s.id===stoneId);
        let name = document.getElementById('receiverName').value;
        let phone = document.getElementById('receiverPhone').value.replace(/\D/g,'');
        if(!name || !phone){ alert("பெயர் மற்றும் போன் எண் கட்டாயம்"); return; }
        let msg = document.getElementById('giveNote').value;
        let waLink = `https://wa.me/${phone}?text=${encodeURIComponent(msg)}`;
        window.open(waLink, '_blank');
        stone.status = 'given_away';
        stone.givenTo = name;
        stone.givenToPhone = phone;
        stone.givenDate = new Date().toISOString().slice(0,10);
        saveStones();
        renderAll();
        bootstrap.Modal.getInstance(document.getElementById('giveawayModal')).hide();
        alert("WhatsApp செய்தி அனுப்பப்பட்டது, கல் கொடுக்கப்பட்டதாக பதிவு செய்தோம்.");
    };

    // Suppliers page with WhatsApp purchase summary
    function renderSuppliersPage() {
        let supplierMap = new Map();
        stones.forEach(s=>{
            if(!supplierMap.has(s.supplierName)) supplierMap.set(s.supplierName, {phone:s.supplierPhone, purchases:[]});
            supplierMap.get(s.supplierName).purchases.push(s);
        });
        let container = document.getElementById('suppliersContainer');
        if(supplierMap.size===0) container.innerHTML='<div class="alert alert-warning">இதுவரை சப்ளையர் இல்லை</div>';
        else {
            container.innerHTML = Array.from(supplierMap.entries()).map(([name,data])=>`<div class="col-md-6 mb-3"><div class="card"><div class="card-header bg-dark text-white">${name} <i class="fab fa-whatsapp"></i></div><div class="card-body"><p>📞 ${data.phone || 'எண் இல்லை'}</p><ul>${data.purchases.map(p=>`<li>${p.stoneName} | CRT:${p.crt} | ₹${p.purchasePrice} | ${p.purchaseDate}</li>`).join('')}</ul><button class="btn btn-whatsapp btn-sm" onclick="sendSupplierSummary('${name}','${data.phone || ''}')"><i class="fab fa-whatsapp"></i> WhatsAppல் சுருக்கம் அனுப்பு</button></div></div></div>`).join('');
        }
    }
    window.sendSupplierSummary = (supplierName, phoneNum) => {
        let purchases = stones.filter(s=>s.supplierName===supplierName);
        let summary = `🏷️ *Garuvida - கொள்வனவு சுருக்கம்*\nசப்ளையர்: ${supplierName}\n\n`;
        let total =0;
        purchases.forEach(p=>{ summary += `🔹 ${p.stoneName} | ${p.shape || ''} | CRT:${p.crt} | விலை:₹${p.purchasePrice} | நாள்:${p.purchaseDate}\n`; total+=p.purchasePrice; });
        summary += `\n*மொத்தம்: ₹${total.toLocaleString('en-IN')}*\nநன்றி - Garuvida Gem`;
        if(phoneNum && phoneNum.trim()!=="") window.open(`https://wa.me/${phoneNum.replace(/\D/g,'')}?text=${encodeURIComponent(summary)}`, '_blank');
        else alert("சப்ளையரின் போன் எண் இல்லை, முதலில் கொள்வனவில் சேர்க்கவும்.");
    };

    // Add stone (support LOT)
    document.getElementById('stoneForm').addEventListener('submit', (e)=>{
        e.preventDefault();
        let isLot = document.getElementById('isLotCheck').checked;
        let lotQty = parseInt(document.getElementById('lotQuantity').value) || 1;
        let baseStone = {
            id: genId(), stoneName: document.getElementById('stoneName').value, shape: document.getElementById('shape').value,
            crt: document.getElementById('crt').value, purchasePrice: parseFloat(document.getElementById('purchasePrice').value),
            purchaseDate: document.getElementById('purchaseDate').value || new Date().toISOString().slice(0,10),
            supplierName: document.getElementById('supplierName').value, supplierPhone: document.getElementById('supplierPhone').value,
            paymentDue: document.getElementById('paymentDue').checked, promisedPaymentDate: document.getElementById('promisedDate').value,
            status: 'in_stock', recutCost: 0
        };
        if(isLot && lotQty>1){
            for(let i=0;i<lotQty;i++){
                let newStone = {...baseStone, id: genId(), stoneName: `${baseStone.stoneName} (LOT-${i+1})`};
                stones.push(newStone);
            }
        } else { stones.push({...baseStone}); }
        saveStones();
        renderAll();
        bootstrap.Modal.getInstance(document.getElementById('addStoneModal')).hide();
        document.getElementById('stoneForm').reset();
    });

    // Page navigation
    document.querySelectorAll('.page-link-nav').forEach(link=>{
        link.addEventListener('click',(e)=>{
            e.preventDefault();
            let pageId = link.getAttribute('data-page');
            document.querySelectorAll('.page').forEach(page=>page.classList.remove('active-page'));
            document.getElementById(`page-${pageId}`).classList.add('active-page');
            document.querySelectorAll('.page-link-nav').forEach(nav=>nav.classList.remove('active'));
            link.classList.add('active');
            renderAll();
        });
    });
    renderAll();
</script>
</body>
</html>
``` 
