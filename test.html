<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WhatsApp Generator & OTP</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        }
        body {
            min-height: 100vh;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }
        .container {
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            width: 100%;
            max-width: 500px;
            padding: 40px;
        }
        h1 {
            color: #333;
            font-size: 28px;
            margin-bottom: 10px;
            text-align: center;
        }
        .subtitle {
            color: #666;
            text-align: center;
            margin-bottom: 30px;
            font-size: 14px;
        }
        .tab-container {
            display: flex;
            margin-bottom: 30px;
            border-bottom: 2px solid #f0f0f0;
        }
        .tab {
            flex: 1;
            text-align: center;
            padding: 10px;
            cursor: pointer;
            color: #666;
            font-weight: 500;
            transition: all 0.3s;
        }
        .tab.active {
            color: #667eea;
            border-bottom: 2px solid #667eea;
            margin-bottom: -2px;
        }
        .form-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 8px;
            color: #333;
            font-weight: 500;
            font-size: 14px;
        }
        input {
            width: 100%;
            padding: 12px 16px;
            border: 2px solid #e0e0e0;
            border-radius: 10px;
            font-size: 16px;
            transition: border-color 0.3s;
        }
        input:focus {
            outline: none;
            border-color: #667eea;
        }
        .btn {
            width: 100%;
            padding: 14px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            border-radius: 10px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: transform 0.2s;
        }
        .btn:hover {
            transform: translateY(-2px);
        }
        .result-box {
            margin-top: 20px;
            padding: 15px;
            background: #f8f9fa;
            border-radius: 10px;
            border-left: 4px solid #667eea;
        }
        .result-box.hidden {
            display: none;
        }
        .result-title {
            font-weight: 600;
            color: #333;
            margin-bottom: 5px;
            font-size: 14px;
        }
        .result-content {
            color: #667eea;
            font-size: 18px;
            word-break: break-all;
        }
        .otp-list {
            margin-top: 20px;
            max-height: 200px;
            overflow-y: auto;
        }
        .otp-item {
            padding: 10px;
            background: #f8f9fa;
            border-radius: 8px;
            margin-bottom: 8px;
            border-left: 3px solid #667eea;
        }
        .otp-number {
            font-weight: 600;
            color: #333;
            font-size: 14px;
        }
        .otp-code {
            color: #667eea;
            font-size: 16px;
            font-weight: 600;
            margin-top: 4px;
        }
        .otp-time {
            color: #999;
            font-size: 12px;
            margin-top: 4px;
        }
        .status-badge {
            display: inline-block;
            padding: 4px 8px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 600;
            margin-left: 8px;
        }
        .status-success {
            background: #d4edda;
            color: #155724;
        }
        .clear-btn {
            background: #dc3545;
            margin-top: 10px;
        }
        .clear-btn:hover {
            background: #c82333;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>WhatsApp Generator</h1>
        <div class="subtitle">Generate nomor WhatsApp & verifikasi OTP</div>
        
        <div class="tab-container">
            <div class="tab active" onclick="switchTab('generate')">Generate</div>
            <div class="tab" onclick="switchTab('login')">Login</div>
        </div>

        <!-- Generate Tab -->
        <div id="generateTab">
            <div class="form-group">
                <label>Jumlah Nomor</label>
                <input type="number" id="jumlahNomor" min="1" max="10" value="1" placeholder="Masukkan jumlah (1-10)">
            </div>
            <div class="form-group">
                <label>Negara (Kode)</label>
                <input type="text" id="kodeNegara" value="62" placeholder="Contoh: 62 untuk Indonesia">
            </div>
            <button class="btn" onclick="generateNomor()">Generate Nomor WhatsApp</button>
            
            <div id="generateResult" class="result-box hidden">
                <div class="result-title">Nomor WhatsApp Tergenerate:</div>
                <div id="nomorList" class="result-content"></div>
            </div>
        </div>

        <!-- Login Tab -->
        <div id="loginTab" style="display: none;">
            <div class="form-group">
                <label>Nomor WhatsApp</label>
                <input type="text" id="nomorLogin" placeholder="Masukkan nomor WhatsApp">
            </div>
            <button class="btn" onclick="requestOTP()">Request OTP</button>
            
            <div id="otpSection" style="display: none;">
                <div class="form-group" style="margin-top: 20px;">
                    <label>Kode OTP</label>
                    <input type="text" id="kodeOTP" placeholder="Masukkan kode OTP">
                </div>
                <button class="btn" onclick="verifyOTP()">Verifikasi OTP</button>
            </div>
        </div>

        <!-- OTP Inbox -->
        <div class="otp-list" id="otpInbox">
            <div style="text-align: center; color: #999; padding: 20px;">
                Belum ada OTP masuk
            </div>
        </div>
        
        <button class="btn clear-btn" onclick="clearOTP()">Hapus Semua OTP</button>
    </div>

    <script>
        // Data storage
        let otpDatabase = [];
        let generatedNumbers = [];

        function switchTab(tab) {
            const generateTab = document.getElementById('generateTab');
            const loginTab = document.getElementById('loginTab');
            const tabs = document.querySelectorAll('.tab');
            
            if (tab === 'generate') {
                generateTab.style.display = 'block';
                loginTab.style.display = 'none';
                tabs[0].classList.add('active');
                tabs[1].classList.remove('active');
            } else {
                generateTab.style.display = 'none';
                loginTab.style.display = 'block';
                tabs[0].classList.remove('active');
                tabs[1].classList.add('active');
            }
        }

        function generateNomor() {
            const jumlah = parseInt(document.getElementById('jumlahNomor').value) || 1;
            const kodeNegara = document.getElementById('kodeNegara').value || '62';
            
            if (jumlah > 10) {
                alert('Maksimal 10 nomor per generate');
                return;
            }

            generatedNumbers = [];
            let nomorListHtml = '';

            for (let i = 0; i < jumlah; i++) {
                // Generate random 10-12 digit number
                const randomDigits = Math.floor(Math.random() * 9000000000) + 1000000000;
                const fullNumber = kodeNegara + randomDigits.toString();
                generatedNumbers.push(fullNumber);
                nomorListHtml += `<div style="margin-bottom: 5px;">✓ ${fullNumber}</div>`;
            }

            document.getElementById('nomorList').innerHTML = nomorListHtml;
            document.getElementById('generateResult').classList.remove('hidden');
        }

        function requestOTP() {
            const nomor = document.getElementById('nomorLogin').value;
            
            if (!nomor) {
                alert('Masukkan nomor WhatsApp');
                return;
            }

            // Generate random 6-digit OTP
            const otp = Math.floor(100000 + Math.random() * 900000).toString();
            const timestamp = new Date().toLocaleString('id-ID');
            
            // Add to OTP database
            otpDatabase.push({
                nomor: nomor,
                otp: otp,
                timestamp: timestamp,
                verified: false
            });

            // Show OTP section
            document.getElementById('otpSection').style.display = 'block';
            
            // Update OTP inbox display
            updateOTPInbox();
            
            alert(`OTP telah dikirim ke ${nomor}`);
        }

        function verifyOTP() {
            const nomor = document.getElementById('nomorLogin').value;
            const kodeOTP = document.getElementById('kodeOTP').value;
            
            if (!nomor || !kodeOTP) {
                alert('Masukkan nomor dan kode OTP');
                return;
            }

            // Find matching OTP
            const otpEntry = otpDatabase.find(entry => 
                entry.nomor === nomor && entry.otp === kodeOTP && !entry.verified
            );

            if (otpEntry) {
                otpEntry.verified = true;
                updateOTPInbox();
                alert('✅ Verifikasi berhasil! Login sukses.');
                document.getElementById('kodeOTP').value = '';
                document.getElementById('nomorLogin').value = '';
                document.getElementById('otpSection').style.display = 'none';
            } else {
                alert('❌ Kode OTP salah atau sudah digunakan');
            }
        }

        function updateOTPInbox() {
            const inbox = document.getElementById('otpInbox');
            
            if (otpDatabase.length === 0) {
                inbox.innerHTML = '<div style="text-align: center; color: #999; padding: 20px;">Belum ada OTP masuk</div>';
                return;
            }

            let html = '';
            // Show last 10 OTPs, newest first
            [...otpDatabase].reverse().slice(0, 10).forEach(entry => {
                const statusClass = entry.verified ? 'status-success' : '';
                const statusText = entry.verified ? '✓ Terverifikasi' : '⏳ Menunggu';
                
                html += `
                    <div class="otp-item">
                        <div class="otp-number">
                            ${entry.nomor}
                            <span class="status-badge ${statusClass}">${statusText}</span>
                        </div>
                        <div class="otp-code">Kode: ${entry.otp}</div>
                        <div class="otp-time">${entry.timestamp}</div>
                    </div>
                `;
            });
            
            inbox.innerHTML = html;
        }

        function clearOTP() {
            if (confirm('Hapus semua riwayat OTP?')) {
                otpDatabase = [];
                updateOTPInbox();
                document.getElementById('otpSection').style.display = 'none';
                document.getElementById('kodeOTP').value = '';
            }
        }
    </script>
</body>
</html>
