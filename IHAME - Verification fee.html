<!DOCTYPE html>
<html lang="ha">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jami'ar IHAME - Receipt Generator & Verify</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #006400; /* Traditional green */
            --primary-light: #4CAF50; /* Brighter green for highlights */
            --primary-glow: #00C853; /* Glowing effect green */
            --secondary: #8BC34A; /* Complementary green */
            --accent: #FFC107; /* Gold accent for contrast */
            --muted: #4b5563;
            --card: #ffffff;
            --paper: #f8fdf8; /* Very light green background */
        }

        body {
            font-family: 'Roboto', system-ui, Arial, sans-serif;
            background: var(--paper);
            color: #111;
            padding: 20px;
            margin: 0;
        }

        header {
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            color: #fff;
            padding: 15px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 20px;
            box-shadow: 0 4px 12px rgba(0, 100, 0, 0.2);
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: -10px;
            left: -10px;
            right: -10px;
            bottom: -10px;
            background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transform: rotate(45deg);
            z-index: 0;
        }

        header img {
            height: 50px;
            z-index: 1;
        }

        header h1 {
            font-size: 24px;
            margin: 0;
            z-index: 1;
        }

        .tabs {
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
            flex-wrap: wrap;
        }

        .tab {
            padding: 10px 15px;
            border-radius: 8px;
            background: var(--card);
            cursor: pointer;
            border: 1px solid var(--muted);
            transition: all 0.3s ease;
            font-weight: 500;
        }

        .tab:hover, .tab.active {
            background: var(--primary);
            color: #fff;
            border-color: var(--primary);
            box-shadow: 0 2px 8px rgba(0, 100, 0, 0.3);
        }

        .container {
            display: flex;
            gap: 16px;
            flex-wrap: wrap;
            animation: fadeIn 0.5s ease-in;
        }

        .left, .right {
            background: var(--card);
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            flex: 1;
            min-width: 280px;
            border: 1px solid rgba(0, 100, 0, 0.1);
        }

        form .row {
            display: flex;
            gap: 8px;
            margin-bottom: 12px;
            align-items: center;
        }

        label {
            font-size: 13px;
            color: var(--muted);
            min-width: 110px;
            font-weight: 500;
        }

        input[type=text], input[type=number], textarea, select {
            flex: 1;
            padding: 12px; /* Increased padding for larger inputs */
            border-radius: 6px;
            border: 1px solid #ddd;
            font-size: 16px; /* Increased font size */
            transition: border-color 0.3s ease;
        }

        input:focus, select:focus, textarea:focus {
            border-color: var(--primary);
            outline: none;
            box-shadow: 0 0 0 2px rgba(0, 100, 0, 0.1);
        }

        textarea {
            min-height: 100px; /* Increased height */
            resize: vertical;
        }

        .receipt-preview {
            border: 2px solid var(--primary);
            padding: 20px;
            border-radius: 12px;
            background: var(--card);
            background-image: linear-gradient(rgba(255, 255, 255, 0.9), rgba(255, 255, 255, 0.9)), url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><text x="50%" y="50%" font-size="12" text-anchor="middle" fill="rgba(0,100,0,0.05)" dy=".3em">IHAME</text></svg>');
            background-size: 50%;
            background-repeat: repeat;
            min-height: 350px;
            position: relative;
            box-shadow: 0 4px 8px rgba(0, 100, 0, 0.1);
        }

        .rc-top {
            text-align: center;
            padding-bottom: 15px;
            border-bottom: 1px solid var(--muted);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .rc-title {
            font-weight: 700;
            color: var(--primary);
            font-size: 22px;
            text-transform: uppercase;
            text-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
        }

        .rc-sub {
            font-size: 12px;
            color: var(--muted);
            margin-bottom: 10px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 12px;
        }

        td, th {
            padding: 8px;
            border: 1px solid #eee;
            font-size: 14px;
        }

        th {
            background-color: rgba(0, 100, 0, 0.05);
        }

        .qr-box {
            border: 1px solid #eee;
            padding: 8px;
            background: var(--card);
            border-radius: 6px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            text-align: center;
            margin-top: 10px;
        }

        .actions {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
        }

        button {
            padding: 10px 15px;
            border-radius: 8px;
            border: none;
            background: linear-gradient(to right, var(--primary), var(--primary-light));
            color: #fff;
            cursor: pointer;
            transition: all 0.3s ease;
            font-size: 14px;
            font-weight: 500;
            box-shadow: 0 2px 4px rgba(0, 100, 0, 0.2);
        }

        button:hover {
            opacity: 0.9;
            box-shadow: 0 4px 8px rgba(0, 100, 0, 0.3);
            transform: translateY(-1px);
        }

        button.secondary {
            background: linear-gradient(to right, var(--secondary), #9CCC65);
        }

        button.accent {
            background: linear-gradient(to right, var(--accent), #FFD54F);
            color: #333;
        }

        small {
            color: var(--muted);
        }

        .verify-view {
            background: var(--card);
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            animation: fadeIn 0.5s ease-in;
            border: 1px solid rgba(0, 100, 0, 0.1);
        }

        .status-ok {
            color: var(--primary);
            font-weight: 700;
        }

        .status-fail {
            color: #c62828;
            font-weight: 700;
        }

        footer {
            margin-top: 20px;
            font-size: 13px;
            color: var(--muted);
            text-align: center;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 768px) {
            .container {
                flex-direction: column;
            }
            .left, .right {
                min-width: 100%;
            }
            .row {
                flex-direction: column;
            }
            label, input, select, textarea {
                width: 100%;
            }
            button {
                width: 100%;
                padding: 12px;
            }
            .qr-box {
                position: static;
                margin: 10px auto;
                text-align: center;
            }
            .rc-top {
                flex-direction: column;
            }
        }

        @media (print) {
            body { padding: 0; }
            .tabs, .left .form-actions, .actions, header, .right { display: none; }
            .receipt-preview { border: none; box-shadow: none; }
            .rc-top { flex-direction: row; }
        }

        /* New styles for photo upload and display */
        .photo-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 10px;
        }

        .photo-preview {
            width: 120px;
            height: 120px;
            border: 1px solid #ddd;
            border-radius: 6px;
            overflow: hidden;
            margin-top: 5px;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #f9f9f9;
        }

        .photo-preview img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        .photo-placeholder {
            color: #999;
            font-size: 12px;
            text-align: center;
        }

        .verify-qr {
            display: flex;
            justify-content: center;
            margin-top: 15px;
        }
    </style>
</head>
<body>

<header>
    <img src="https://i.ibb.co/DHhQsbhb/Royal-Blue-and-Gold-University-Logo-20250822-190530-0000.png" alt="IHAME University Logo">
    <div>
        <h1>Jami'ar IHAME</h1>
        <small>Home of Knowledge — Shaidar Biyan Kuɗi / Admission</small>
    </div>
    <div style="margin-left:auto"><small>Platform: <strong>Verify / Tabbatarwa</strong></small></div>
</header>

<div class="tabs" id="tabs">
    <div class="tab active" data-section="r1">Receipt 1</div>
    <div class="tab" data-section="r2">Receipt 2</div>
    <div class="tab" data-section="r3">Receipt 3</div>
    <div class="tab" data-section="verify" style="margin-left:8px;">Duba Tabbatarwa</div>
</div>

<div class="container">
    <div class="left">
        <form id="mainForm">
            <input type="hidden" id="section" value="r1">
            
            <div class="row">
                <label>Hotun Mai Biya</label>
                <div style="flex:1">
                    <input type="file" id="photoUpload" accept="image/*" style="width:100%;padding:8px">
                    <div class="photo-container">
                        <div class="photo-preview" id="photoPreview">
                            <div class="photo-placeholder">Babu hoto</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="row">
                <label>Sunan ɗalibi / Mai biya</label>
                <input id="name" type="text" placeholder="Sunan cikakke..." required>
            </div>
            <div class="row">
                <label>Imel</label>
                <input id="email" type="text" placeholder="example@mail.com">
            </div>
            <div class="row">
                <label>Lambar waya</label>
                <input id="phone" type="text" placeholder="0907xxxxxxx">
            </div>
            <div class="row">
                <label>Dalibi ID / Reg No</label>
                <input id="studentId" type="text" placeholder="Reg-2025-0001">
            </div>
            <div class="row">
                <label>Abin da aka biya</label>
                <input id="description" type="text" placeholder="Misb. Karatu / Jarabawa / Rajista">
            </div>
            <div class="row">
                <label>Adadin (₦)</label>
                <input id="amount" type="number" placeholder="20000">
            </div>
            <div class="row">
                <label>Hanyar Biyan Kuɗi</label>
                <select id="paymentMethod">
                    <option value="Bank Transfer">Bank Transfer</option>
                    <option value="Cash">Cash</option>
                    <option value="POS">POS</option>
                    <option value="Online">Online</option>
                </select>
            </div>
            <div class="row">
                <label>Account Name</label>
                <input id="accName" type="text" placeholder="Abdulhadi Lawal">
            </div>
            <div class="row">
                <label>Account Number</label>
                <input id="accNumber" type="text" placeholder="2213099281">
            </div>
            <div class="row">
                <label>Bank</label>
                <input id="bankName" type="text" placeholder="UBA">
            </div>
            <div class="row">
                <label>Sauran bayanai</label>
                <textarea id="notes" placeholder="Karin bayani... (optional)"></textarea>
            </div>
            <div class="form-actions" style="display:flex;gap:10px;">
                <button type="button" id="generate">Generate / Ajiye & ƙirƙiri QR</button>
                <button type="button" class="secondary" id="clear">Share fom</button>
            </div>
        </form>
    </div>

    <div class="right">
        <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
            <strong>Preview — Zaka iya duba kafin bugawa</strong>
            <small id="refLabel">Ref: -</small>
        </div>
        <div class="receipt-preview" id="preview">
            <div class="rc-top">
                <div>
                    <img src="https://i.ibb.co/DHhQsbhb/Royal-Blue-and-Gold-University-Logo-20250822-190530-0000.png" alt="IHAME University Logo" style="height:60px">
                </div>
                <div>
                    <div class="rc-title">JAMI'AR IHAME</div>
                    <div class="rc-sub">Home of Knowledge — Shaidar Biyan Kuɗi / Admission</div>
                </div>
                <div class="photo-preview" id="previewPhoto" style="width:80px;height:80px;">
                    <div class="photo-placeholder">Babu hoto</div>
                </div>
            </div>
            <table>
                <tr><th>Sunan</th><td id="pName">-</td></tr>
                <tr><th>Imel</th><td id="pEmail">-</td></tr>
                <tr><th>Phone</th><td id="pPhone">-</td></tr>
                <tr><th>Student ID</th><td id="pStudentId">-</td></tr>
                <tr><th>Abin da aka biya</th><td id="pDesc">-</td></tr>
                <tr><th>Amount (₦)</th><td id="pAmount">-</td></tr>
                <tr><th>Hanyar Biyan</th><td id="pPayMethod">-</td></tr>
                <tr><th>Account</th><td id="pAccount">-</td></tr>
            </table>
            <div><small id="pNotes">-</small></div>
            <div class="qr-box" id="qrBox">
                <div id="qrPlaceholder" style="width:120px;height:120px;background:#f5f5f5;display:flex;align-items:center;justify-content:center;color:#999;font-size:12px;margin:0 auto;">QR Code</div>
                <div style="font-size:11px;text-align:center;margin-top:5px"><small>Scan don Tabbatarwa</small></div>
            </div>
            <div style="margin-top:15px"><small>Wanda za a tuntuba: Registrar — Dr. Muslaf. Phone: 09074765785 / 07071992912</small></div>
        </div>
        <div class="actions" style="margin-top:12px">
            <button id="printBtn">Print / Bugawa</button>
            <button id="downloadBtn" class="secondary">Download Image (PNG)</button>
            <button id="openVerify" class="accent">Bude Verify Page</button>
        </div>
    </div>
</div>

<hr style="margin:20px 0">

<div id="verifySection" class="verify-view" style="display:none">
    <h3 style="color:var(--primary)">Verify / Tabbatarwa</h3>
    <div id="verifyResult">
        <p>Shigar da Reference ko danna QR (idan QR ɗin daga wannan system ɗin zai nuna bayanin):</p>
        <div style="display:flex;gap:10px;margin-bottom:10px">
            <input id="verifyRef" type="text" placeholder="Ref-2025-xxxxx" style="flex:1;padding:12px;border-radius:6px;border:1px solid #ddd;font-size:16px">
            <button id="doVerify">Duba</button>
        </div>
        <div id="verifyOutput"></div>
        <hr>
        <h4 style="color:var(--primary)">History (Saved locally)</h4>
        <div id="historyList"><small>Ba a sami saved receipts ba.</small></div>
    </div>
</div>

<footer>
    <small>Note: Wannan fayil zai adana bayanai a browser (localStorage). Idan kana son ajiya a server ka sanar ni domin in tsara backend (PHP/Node/Firebase).</small>
</footer>

<script>
    /* Helper utilities */
    function $(s){return document.querySelector(s)}
    function $all(s){return Array.from(document.querySelectorAll(s))}

    function genRef(prefix='REF'){
        const t = Date.now().toString(36).toUpperCase();
        const r = Math.random().toString(36).slice(2,6).toUpperCase();
        return prefix + '-' + t.slice(-6) + r;
    }

    function buildVerifyURL(ref){
        try{
            const base = location.href.split('#')[0];
            return base + '#verify:' + encodeURIComponent(ref);
        }catch(e){
            return '#verify:' + encodeURIComponent(ref);
        }
    }

    function makeQRDataURL(data, size=200){
        const u = encodeURIComponent(data);
        // Using multiple QR code APIs as fallback
        const apis = [
            `https://api.qrserver.com/v1/create-qr-code/?size=${size}x${size}&data=${u}`,
            `https://chart.googleapis.com/chart?cht=qr&chs=${size}x${size}&chl=${u}&chld=L|1`,
            `https://quickchart.io/qr?text=${u}&size=${size}`
        ];
        return apis[0]; // Use the first one
    }

    function saveRecord(ref, obj){
        const all = JSON.parse(localStorage.getItem('ihame_receipts_v1') || '{}');
        all[ref] = obj;
        localStorage.setItem('ihame_receipts_v1', JSON.stringify(all));
    }

    function loadRecord(ref){
        const all = JSON.parse(localStorage.getItem('ihame_receipts_v1') || '{}');
        return all[ref] || null;
    }

    function renderHistory(){
        const all = JSON.parse(localStorage.getItem('ihame_receipts_v1') || '{}');
        const keys = Object.keys(all).sort().reverse();
        const container = $('#historyList');
        if(!keys.length){ container.innerHTML = '<small>Ba a sami saved receipts ba.</small>'; return; }
        container.innerHTML = '';
        keys.forEach(k=>{
            const r = all[k];
            const div = document.createElement('div');
            div.style.borderTop='1px solid #f1f1f1'; div.style.padding='8px 0';
            div.innerHTML = `<strong>${k}</strong> — ${r.name || '-'} — ₦${r.amount || 0} — <button data-ref="${k}" class="viewRefBtn">View</button> <button data-ref="${k}" class="openRefBtn">Open Verify</button>`;
            container.appendChild(div);
        });
        $all('.viewRefBtn').forEach(b=>b.addEventListener('click', e=>{
            const k = e.target.dataset.ref;
            const r = loadRecord(k);
            if(!r) return alert('Babu');
            alert(JSON.stringify(r,null,2));
        }));
        $all('.openRefBtn').forEach(b=>b.addEventListener('click', e=>{
            const k = e.target.dataset.ref;
            location.hash = 'verify:' + encodeURIComponent(k);
            showVerifySection(true);
            doVerify(k);
        }));
    }

    function fillPreview(data, ref){
        $('#pName').textContent = data.name || '-';
        $('#pEmail').textContent = data.email || '-';
        $('#pPhone').textContent = data.phone || '-';
        $('#pStudentId').textContent = data.studentId || '-';
        $('#pDesc').textContent = data.description || '-';
        $('#pAmount').textContent = data.amount || '0';
        $('#pPayMethod').textContent = data.paymentMethod || '-';
        $('#pAccount').textContent = (data.accName||'') + ' / ' + (data.accNumber||'') + ' (' + (data.bankName||'') + ')';
        $('#pNotes').textContent = data.notes || '-';
        $('#refLabel').textContent = 'Ref: ' + (ref || '-');
        
        // Display photo if available
        const previewPhoto = $('#previewPhoto');
        if (data.photo) {
            previewPhoto.innerHTML = '';
            const img = document.createElement('img');
            img.src = data.photo;
            img.alt = "Payer Photo";
            img.style.maxWidth = '100%';
            img.style.maxHeight = '100%';
            previewPhoto.appendChild(img);
        } else {
            previewPhoto.innerHTML = '<div class="photo-placeholder">Babu hoto</div>';
        }
        
        // Generate QR code only if we have a reference
        if (ref && ref !== '-') {
            const verifyURL = buildVerifyURL(ref);
            const qrCodeURL = makeQRDataURL(verifyURL, 120);
            
            const qrBox = $('#qrBox');
            qrBox.innerHTML = ''; // Clear existing content
            
            const qrImg = document.createElement('img');
            qrImg.src = qrCodeURL;
            qrImg.alt = "QR Code";
            qrImg.width = 120;
            qrImg.height = 120;
            qrImg.style.display = 'block';
            qrImg.style.margin = '0 auto';
            
            // Add error handling for QR code
            qrImg.onerror = function() {
                console.log('QR code failed to load, trying fallback...');
                // Try fallback API
                const fallbackURL = `https://chart.googleapis.com/chart?cht=qr&chs=120x120&chl=${encodeURIComponent(verifyURL)}&chld=L|1`;
                qrImg.src = fallbackURL;
            };
            
            qrBox.appendChild(qrImg);
            
            const scanText = document.createElement('div');
            scanText.style.fontSize = '11px';
            scanText.style.textAlign = 'center';
            scanText.style.marginTop = '5px';
            scanText.innerHTML = '<small>Scan don Tabbatarwa</small>';
            qrBox.appendChild(scanText);
        }
    }

    function readForm(){
        return {
            name: $('#name').value.trim(),
            email: $('#email').value.trim(),
            phone: $('#phone').value.trim(),
            studentId: $('#studentId').value.trim(),
            description: $('#description').value.trim(),
            amount: $('#amount').value.trim(),
            paymentMethod: $('#paymentMethod').value,
            accName: $('#accName').value.trim(),
            accNumber: $('#accNumber').value.trim(),
            bankName: $('#bankName').value.trim(),
            notes: $('#notes').value.trim(),
            photo: $('#photoPreview img') ? $('#photoPreview img').src : null,
            createdAt: new Date().toISOString()
        };
    }

    function downloadAsImage(el, filename = 'receipt.png'){
        const svgNS = "http://www.w3.org/2000/svg";
        const serializer = new XMLSerializer();
        const width = el.offsetWidth;
        const height = el.offsetHeight;
        const cloned = el.cloneNode(true);
        cloned.querySelectorAll('button, input').forEach(n=>n.remove());
        const svg = document.createElementNS(svgNS, "svg");
        svg.setAttribute("xmlns", svgNS);
        svg.setAttribute("width", width);
        svg.setAttribute("height", height);
        const foreign = document.createElementNS(svgNS, "foreignObject");
        foreign.setAttribute("width", "100%");
        foreign.setAttribute("height", "100%");
        foreign.appendChild(cloned);
        svg.appendChild(foreign);
        const svgString = serializer.serializeToString(svg);
        const blob = new Blob([svgString], {type: 'image/svg+xml;charset=utf-8'});
        const url = URL.createObjectURL(blob);
        const img = new Image();
        img.onload = function(){
            const canvas = document.createElement('canvas');
            canvas.width = img.width;
            canvas.height = img.height;
            const ctx = canvas.getContext('2d');
            ctx.fillStyle = '#ffffff';
            ctx.fillRect(0,0,canvas.width,canvas.height);
            ctx.drawImage(img,0,0);
            URL.revokeObjectURL(url);
            canvas.toBlob(function(b){
                const a = document.createElement('a');
                a.download = filename;
                a.href = URL.createObjectURL(b);
                a.click();
                URL.revokeObjectURL(a.href);
            }, 'image/png');
        };
        img.onerror = function(){
            alert('Ba a iya sauke hoton a wasu browsers. Yi amfani da Print to PDF ko buɗe a Chrome/Edge.');
        };
        img.src = url;
    }

    function doVerify(ref){
        const r = loadRecord(ref);
        const out = $('#verifyOutput');
        if(!r){
            out.innerHTML = `<div><p class="status-fail">Invalid / Babu wannan Reference: <strong>${ref}</strong></p></div>`;
            return;
        }
        
        // Generate QR code for verification
        const verifyURL = buildVerifyURL(ref);
        const qrCodeURL = makeQRDataURL(verifyURL, 150);
        
        let photoHTML = '';
        if (r.photo) {
            photoHTML = `
            <tr>
                <th>Hotun Mai Biya</th>
                <td><img src="${r.photo}" alt="Payer Photo" style="max-width:120px;max-height:120px;"></td>
            </tr>`;
        }
        
        out.innerHTML = `<div>
            <p class="status-ok">✅ Valid — Reference: <strong>${ref}</strong></p>
            <table>
                <tr><th>Sunan</th><td>${r.name||''}</td></tr>
                <tr><th>Student ID</th><td>${r.studentId||''}</td></tr>
                <tr><th>Amount</th><td>₦${r.amount||''}</td></tr>
                <tr><th>Payment</th><td>${r.paymentMethod||''}</td></tr>
                ${photoHTML}
                <tr><th>Saved at</th><td>${r.createdAt||''}</td></tr>
            </table>
            <div class="verify-qr">
                <div class="qr-box">
                    <img src="${qrCodeURL}" alt="QR Code" width="150" height="150">
                    <div style="font-size:11px;text-align:center;margin-top:5px"><small>Scan don Tabbatarwa</small></div>
                </div>
            </div>
            <div style="margin-top:8px"><button onclick="window.print()">Print / Bugawa (ɗauki wannan shafi)</button></div>
        </div>`;
    }

    function showVerifySection(show){
        if(show){
            $('#verifySection').style.display = 'block';
            $('.container').style.display = 'none';
        } else {
            $('#verifySection').style.display = 'none';
            $('.container').style.display = 'flex';
        }
    }

    document.addEventListener('DOMContentLoaded', ()=>{
        $all('.tab').forEach(t=>{
            t.addEventListener('click', e=>{
                $all('.tab').forEach(x=>x.classList.remove('active'));
                t.classList.add('active');
                const sec = t.dataset.section;
                $('#section').value = sec;
                if(sec === 'verify'){
                    showVerifySection(true);
                    renderHistory();
                } else {
                    showVerifySection(false);
                }
            });
        });

        // Handle photo upload
        $('#photoUpload').addEventListener('change', function(e) {
            const file = e.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(event) {
                    const photoPreview = $('#photoPreview');
                    photoPreview.innerHTML = '';
                    const img = document.createElement('img');
                    img.src = event.target.result;
                    img.alt = "Payer Photo";
                    img.style.maxWidth = '100%';
                    img.style.maxHeight = '100%';
                    photoPreview.appendChild(img);
                };
                reader.readAsDataURL(file);
            }
        });

        $('#generate').addEventListener('click', ()=>{
            const data = readForm();
            if(!data.name){ 
                alert('Da fatan za a saka sunan mai biya.'); 
                return; 
            }
            
            const ref = genRef('IH');
            const section = $('#section').value || 'r1';
            const record = Object.assign({ref, section}, data);
            
            // Save the record first
            saveRecord(ref, record);
            
            // Then fill the preview with the data and reference
            fillPreview(data, ref);
            
            // Render history
            renderHistory();
            
            alert('An adana & ƙirƙiri QR. Reference: ' + ref);
        });

        $('#clear').addEventListener('click', ()=>{
            if(!confirm('Kana so a share fom?')) return;
            $('#mainForm').reset();
            const blank = {
                name:'-', email:'-', phone:'-', studentId:'-', 
                description:'-', amount:'-', paymentMethod:'-', 
                accName:'', accNumber:'', bankName:'', notes:'', photo: null
            };
            fillPreview(blank, '-');
            $('#refLabel').textContent = 'Ref: -';
            
            // Reset photo preview
            $('#photoPreview').innerHTML = '<div class="photo-placeholder">Babu hoto</div>';
            
            // Reset QR code to placeholder
            const qrBox = $('#qrBox');
            qrBox.innerHTML = '';
            const placeholder = document.createElement('div');
            placeholder.id = 'qrPlaceholder';
            placeholder.style.width = '120px';
            placeholder.style.height = '120px';
            placeholder.style.background = '#f5f5f5';
            placeholder.style.display = 'flex';
            placeholder.style.alignItems = 'center';
            placeholder.style.justifyContent = 'center';
            placeholder.style.color = '#999';
            placeholder.style.fontSize = '12px';
            placeholder.style.margin = '0 auto';
            placeholder.textContent = 'QR Code';
            qrBox.appendChild(placeholder);
            
            const scanText = document.createElement('div');
            scanText.style.fontSize = '11px';
            scanText.style.textAlign = 'center';
            scanText.style.marginTop = '5px';
            scanText.innerHTML = '<small>Scan don Tabbatarwa</small>';
            qrBox.appendChild(scanText);
        });

        $('#printBtn').addEventListener('click', ()=>{
            window.print();
        });

        $('#downloadBtn').addEventListener('click', ()=>{
            const el = $('#preview');
            const refText = $('#refLabel').textContent.replace('Ref: ','').trim();
            const filename = (refText && refText !== '-') ? (refText + '.png') : 'receipt.png';
            downloadAsImage(el, filename);
        });

        $('#openVerify').addEventListener('click', ()=>{
            location.hash = 'verify:';
            showVerifySection(true);
            renderHistory();
        });

        $('#doVerify').addEventListener('click', ()=>{
            const ref = $('#verifyRef').value.trim();
            if(!ref){ 
                alert('Da fatan za a shigar da reference number.'); 
                return; 
            }
            doVerify(ref);
        });

        function handleHash(){
            const h = location.hash || '';
            if(h.startsWith('#verify:')){
                const ref = decodeURIComponent(h.replace('#verify:',''));
                showVerifySection(true);
                renderHistory();
                if(ref) {
                    $('#verifyRef').value = ref;
                    doVerify(ref);
                }
            } else {
                showVerifySection(false);
            }
        }
        window.addEventListener('hashchange', handleHash);
        handleHash();

        // Initialize with empty preview
        const initialData = {
            name:'-', email:'-', phone:'-', studentId:'-', 
            description:'-', amount:'-', paymentMethod:'-', 
            accName:'', accNumber:'', bankName:'', notes:'', photo: null
        };
        fillPreview(initialData, '-');
    });
</script>

</body>
</html>
