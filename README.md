# BLING BLING GEMS 
!-- Services Tab -->
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