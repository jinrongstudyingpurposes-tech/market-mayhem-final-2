
        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            padding: 12px;
            font-size: 16px; /* Prevents auto-zoom on iOS mobile forms */
            transition: background-color 0.5s ease;
            -webkit-text-size-adjust: 100%;
        }
        
        body.goal-achieved {
            background-color: var(--goal-met-bg) !important;
        }

        .container { width: 100%; max-width: 1200px; margin: 0 auto; }
        header { text-align: center; margin-bottom: 20px; border-bottom: 2px solid var(--border-color); padding-bottom: 12px; }
        h1 { color: var(--accent-color); font-size: 2rem; }
        header p { color: #94a3b8; font-size: 0.9rem; margin-top: 4px; }
        h2 { margin-bottom: 15px; color: #cbd5e1; border-left: 4px solid var(--accent-color); padding-left: 10px; font-size: 1.3rem; }
        h3 { font-size: 1.1rem; margin-bottom: 10px; color: #cbd5e1; }
        
        .view-panel { display: none; background: var(--card-bg); border: 1px solid var(--border-color); border-radius: 12px; padding: 20px; box-shadow: 0 10px 25px -5px rgba(0,0,0,0.4); margin-bottom: 15px; }
        .view-panel.active-view { display: block; }

        .form-group { margin-bottom: 18px; }
        label { display: block; margin-bottom: 6px; font-weight: 600; color: #94a3b8; font-size: 0.9rem; }
        input, select { width: 100%; padding: 14px; background: #0f172a; border: 1px solid var(--border-color); color: var(--text-color); border-radius: 8px; font-size: 1rem; -webkit-appearance: none; }
        input:focus, select:focus { border-color: var(--accent-color); outline: none; }

        button { width: 100%; background: var(--accent-color); color: white; border: none; padding: 14px 22px; border-radius: 8px; cursor: pointer; font-size: 1rem; font-weight: bold; transition: opacity 0.2s, transform 0.1s; text-align: center; display: inline-block; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
        button:hover { opacity: 0.9; }
        button:active { transform: scale(0.99); }
        .btn-danger { background: var(--danger-color); }
        .btn-success { background: var(--success-color); }
        .btn-secondary { background: #475569; }

        /* Force table text and fields visibility over custom backgrounds */
        table, th, td {
            color: var(--text-color) !important;
        }

        /* Cross-Device Adaptive Nav Layout */
        .adaptive-nav-bar { display: flex; flex-direction: column; gap: 10px; margin-bottom: 20px; background: rgba(15, 23, 42, 0.8); padding: 14px; border-radius: 8px; border: 1px solid var(--border-color); }
        .nav-buttons-cluster { display: flex; flex-direction: column; gap: 8px; width: 100%; }
        
        .portfolio-value-banner { text-align: center; font-size: 1.1rem; font-weight: bold; color: var(--warning-color); background: #0f172a; padding: 12px; border-radius: 6px; border: 1px dashed var(--warning-color); width: 100%; }
        .live-badge { display: inline-block; background: var(--success-color); color: white; font-size: 0.75rem; padding: 2px 8px; border-radius: 20px; font-weight: bold; text-transform: uppercase; letter-spacing: 1px; }

        .layout-grid { display: flex; flex-direction: column; gap: 20px; }
        .sub-panel { background: rgba(15, 23, 42, 0.5); border: 1px solid var(--border-color); border-radius: 8px; padding: 15px; height: fit-content; }

        .table-responsive-wrapper { width: 100%; overflow-x: auto; -webkit-overflow-scrolling: touch; border-radius: 6px; border: 1px solid var(--border-color); margin-bottom: 15px; background: #0f172a; }
        .overview-table { width: 100%; border-collapse: collapse; min-width: 550px; }
        .overview-table th, .overview-table td { padding: 12px 10px; text-align: left; border-bottom: 1px solid var(--border-color); font-size: 0.85rem; }
        .overview-table th { background-color: #1e293b; color: var(--accent-color); font-weight: bold; }
        
        .risk-badge { padding: 2px 6px; font-size: 0.75rem; border-radius: 4px; font-weight: bold; display: inline-block; }
        .risk-1 { background-color: var(--success-color); color: white; }
        .risk-2 { background-color: var(--warning-color); color: black; }
        .risk-3 { background-color: var(--danger-color); color: white; }

        .change-positive { color: var(--success-color); font-weight: bold; }
        .change-negative { color: var(--danger-color); font-weight: bold; }
        .change-none { color: #64748b; font-weight: bold; }
        .active-mod-tag { display: inline-block; background: #9333ea; color: white; padding: 2px 6px; font-size: 0.75rem; font-weight: bold; border-radius: 4px; margin-top: 4px; margin-right: 4px; }

        .bought-profit { color: var(--success-color) !important; font-weight: bold; }
        .bought-loss { color: var(--danger-color) !important; font-weight: bold; }

        .confirm-preview-box { background: #0f172a; border: 1px dashed var(--border-color); border-radius: 8px; padding: 20px; margin-bottom: 15px; text-align: center; }
        .confirm-price-display { font-size: 2.2rem; font-weight: bold; color: var(--warning-color); margin: 8px 0; }

        .invoice-box { background: white; color: #1e293b; padding: 20px; border-radius: 8px; border-left: 6px solid var(--accent-color); margin: 15px 0; font-family: monospace; }
        .invoice-box h3 { border-bottom: 1px dashed #cbd5e1; padding-bottom: 6px; margin-bottom: 10px; font-size: 1.2rem; color: #0f172a; border-left: none; }
        .invoice-amount { font-size: 1.8rem; font-weight: bold; margin: 10px 0; color: #0f172a; }

        .goal-indicator { font-size: 1.1rem; font-weight: bold; padding: 12px; border-radius: 6px; text-align: center; margin-top: 12px; }
        .goal-not-met { background: #334155; color: #cbd5e1; border: 1px dashed #64748b; }
        .goal-met { background: var(--success-color); color: white; box-shadow: 0 0 15px rgba(34,213,94,0.5); }

        .modal-overlay { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(15, 23, 42, 0.85); backdrop-filter: blur(4px); z-index: 9999; justify-content: center; align-items: center; padding: 15px; }
        .modal-box { background-color: var(--card-bg); border: 1px solid var(--border-color); border-radius: 12px; max-width: 480px; width: 100%; padding: 20px; box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.5); }
        .modal-overlay.active-modal { display: flex; }
        .modal-header { font-size: 1.2rem; font-weight: bold; margin-bottom: 10px; color: var(--accent-color); border-bottom: 1px solid var(--border-color); padding-bottom: 6px; }
        .modal-body { font-size: 0.95rem; margin-bottom: 15px; color: #e2e8f0; line-height: 1.4; white-space: pre-wrap; }
        .modal-footer { display: flex; justify-content: flex-end; gap: 10px; }
        .modal-footer button { width: auto; padding: 10px 20px; }

        @media (min-width: 768px) {
            body { padding: 24px; }
            h1 { font-size: 2.4rem; }
            .view-panel { padding: 25px; }
            .layout-grid { display: grid; grid-template-columns: 2fr 1fr; gap: 24px; }
            .adaptive-nav-bar { flex-direction: row; justify-content: space-between; align-items: center; }
            .nav-buttons-cluster { flex-direction: row; width: auto; }
            .nav-buttons-cluster button { width: auto; }
            .portfolio-value-banner { width: auto; min-width: 250px; }
            button { width: auto; }
        }
    </style>

    <script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/8.10.1/firebase-database.js"></script>
</head>
<body>

<div class="container">
    <header>
        <h1>Market Mayhem</h1>
        <p>Live Collaborative Workspace Engine <span class="live-badge" id="lobby-status-pill">Offline</span></p>
    </header>

    <div id="view-gateway" class="view-panel active-view">
        <h2>Enter Live Game Space</h2>
        <div class="form-group">
            <label for="input-lobby-code">Live Game ID (Room Code):</label>
            <input type="text" id="input-lobby-code" placeholder="e.g. 5005" style="text-transform: uppercase; font-family: monospace; letter-spacing: 2px; text-align: center; font-size: 1.4rem; max-width: 350px; margin: 0 auto; display: block; margin-bottom: 15px;">
            
            <label for="input-user-name">Your Game Username:</label>
            <input type="text" id="input-user-name" placeholder="Enter name or initials" style="text-align: center; font-size: 1.2rem; max-width: 350px; margin: 0 auto; display: block;">
        </div>
        <div style="text-align: center; margin-top: 10px;">
            <button onclick="connectToLobbyRoom()">Connect to Shared Room</button>
        </div>
    </div>

    <div id="view-setup" class="view-panel">
        <h2>Select Your Assigned Profile Card</h2>
        <div class="form-group">
            <label for="player-profile-select">Profile Identity:</label>
            <select id="player-profile-select">
                <option value="Z1">Z1 - The Risky Rizzler (Aggressive Risk-Taker)</option>
                <option value="Z2">Z2 - The Safe Skibidi (Conservative Investor)</option>
                <option value="Z3">Z3 - The Balanced Baller (Balanced Framework)</option>
            </select>
        </div>
        <button onclick="initializeTrackerDashboard()">Launch Tracker Dashboard</button>
    </div>

    <div id="view-overview" class="view-panel">
        <div class="adaptive-nav-bar">
            <div class="nav-buttons-cluster">
                <button class="btn-success" onclick="openBuyMarketScreen()">Buy Asset</button>
                <button class="btn-danger" onclick="openSellPortfolioScreen()">Sell Asset</button>
                <button class="btn-secondary" onclick="backToProfileSelection()">Back to Profiles</button>
                <button class="btn-danger" style="background-color:#991b1b;" onclick="triggerEndGameDiscard()">End Game</button>
            </div>
            <div class="portfolio-value-banner" id="room-code-banner" style="font-size: 1.1rem; color: #cbd5e1; border: 1px solid var(--border-color); padding: 12px;">Room: ----</div>
            <div class="portfolio-value-banner">
                Total Portfolio Value: <span id="total-portfolio-display">$0</span>
            </div>
        </div>

        <div class="layout-grid">
            <div class="sub-panel">
                <h2>Your Owned Portfolio Assets</h2>
                <div class="table-responsive-wrapper">
                    <table class="overview-table">
                        <thead>
                            <tr>
                                <th>Instance ID</th>
                                <th>Asset ID</th>
                                <th>Asset Name</th>
                                <th>Risk Tier</th>
                                <th>Bought Price</th>
                                <th>Current Value</th>
                                <th>Net Change</th>
                            </tr>
                        </thead>
                        <tbody id="portfolio-table-body"></tbody>
                    </table>
                </div>
            </div>

            <div class="sub-panel">
                <h2>Global Scenario Deck</h2>
                <p style="font-size: 0.8rem; color: #cbd5e1; margin-bottom: 8px;"><strong>Peer Rule:</strong> Any player can execute the card here. Doing so updates the database and pushes calculations to all players simultaneously.</p>
                <div class="form-group">
                    <label for="scenario-select">Drawn Scenario Card:</label>
                    <select id="scenario-select" onchange="previewScenarioInfo()">
                        <option value="">-- Choose Active Scenario --</option>
                    </select>
                    <p id="scenario-preview-text" style="font-size: 0.8rem; color: #94a3b8; margin-top: 6px; font-style: italic; min-height: 20px;"></p>
                </div>
                <button style="width: 100%; margin-bottom: 25px;" onclick="triggerScenarioConfirmation()">Confirm &amp; Broadcast Scenario</button>

                <h2>Action Card Deck (Holding Assets Only)</h2>
                <div class="form-group">
                    <label for="action-select">Play Value-Altering Card:</label>
                    <select id="action-select" onchange="previewActionInfo()">
                        <option value="">-- Select Modifying Card --</option>
                        <option value="A3">A3: Diversification (Halves Scenario loss instantly/retroactively)</option>
                        <option value="A4">A4: Expert Advice (Peek at next market trends)</option>
                        <option value="A6">A6: Safe Haven (Immunizes 1 specific owned asset card)</option>
                        <option value="A8">A8: Rebalance Portfolio (Swap card instance at current value)</option>
                        <option value="A9">A9: Hedge Funds (Bypasses worst single calculation loss)</option>
                        <option value="A10">A10: Investment Strategy (x2 Base growth permanently)</option>
                        <option value="A11">A11: Bad Advice (Halves next scenario returns)</option>
                        <option value="A12">A12: Overconfidence (x2 Gains AND x2 Losses)</option>
                        <option value="A15">A15: Greed (Doubles total scenario losses)</option>
                        <option value="A16">A16: Market Rumour (Doubles targeted sector losses)</option>
                        <option value="A19">A19: FOMO (Forces rapid sector entry investment)</option>
                        <option value="A11_TARGET">Attack: Pass Bad Advice (A11) to Player</option>
                        <option value="A12_TARGET">Attack: Pass Overconfidence (A12) to Player</option>
                        <option value="A15_TARGET">Attack: Pass Greed (A15) to Player</option>
                        <option value="A16_TARGET">Attack: Pass Market Rumour (A16) to Player</option>
                    </select>
                    <p id="action-preview-text" style="font-size: 0.8rem; color: #eab308; margin-top: 6px; font-style: italic; min-height: 20px;"></p>
                </div>
                
                <div class="form-group" id="target-player-group" style="display: none;">
                    <label for="target-player-select">Select Target Player:</label>
                    <select id="target-player-select"></select>
                </div>
                
                <button style="width: 100%; background: #9333ea;" onclick="executeActionCardDirect()">Apply Action Card</button>

                <div style="margin-top: 25px; border-top: 1px solid var(--border-color); padding-top: 15px;">
                    <h3>Profile Target Status</h3>
                    <p id="profile-text-desc" style="font-size: 0.85rem; color: #cbd5e1; margin-top: 5px; line-height: 1.4;"></p>
                    <div id="goal-status-box" class="goal-indicator goal-not-met">Objective Parameters Unmet</div>
                </div>
            </div>
        </div>
    </div>

    <div id="view-buy-market" class="view-panel">
        <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 15px;">
            <h2>Available Market Assets (Buy Board)</h2>
            <button class="btn-secondary" style="width: auto;" onclick="showScreen('view-overview')">Back to Overview</button>
        </div>
        <div class="table-responsive-wrapper">
            <table class="overview-table">
                <thead>
                    <tr>
                        <th>Asset ID</th>
                        <th>Asset Name</th>
                        <th>Risk Tier</th>
                        <th>Asset Sector</th>
                        <th>Market Value (Cost)</th>
                        <th>Purchase Action</th>
                    </tr>
                </thead>
                <tbody id="buy-market-table-body"></tbody>
            </table>
        </div>
    </div>

    <div id="view-sell-portfolio" class="view-panel">
        <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 15px;">
            <h2>Your Portfolio Holdings (Sell Board)</h2>
            <button class="btn-secondary" style="width: auto;" onclick="showScreen('view-overview')">Back to Overview</button>
        </div>
        <div class="table-responsive-wrapper">
            <table class="overview-table">
                <thead>
                    <tr>
                        <th>Instance ID</th>
                        <th>Asset ID</th>
                        <th>Asset Name</th>
                        <th>Risk Tier</th>
                        <th>Your Stacked Card Value</th>
                        <th>Liquidation Action</th>
                    </tr>
                </thead>
                <tbody id="sell-portfolio-table-body"></tbody>
            </table>
        </div>
    </div>

    <div id="view-confirm-transaction" class="view-panel">
        <h2>Confirm Financial Action</h2>
        <div class="confirm-preview-box">
            <h3 id="confirm-action-type" style="font-size: 1.3rem; color: #cbd5e1; margin-bottom: 8px;">ACTION PREVIEW</h3>
            <div id="confirm-asset-details" style="font-size: 1.1rem; font-weight: 600;">[ID] Name Details</div>
            <div class="confirm-price-display" id="confirm-price-readout">$0</div>
        </div>
        <div style="display: flex; gap: 15px; justify-content: center; flex-wrap: wrap;">
            <button class="btn-success" style="min-width: 160px;" onclick="commitConfirmedTransaction(false)">Confirm &amp; Complete</button>
            <button class="btn-success" style="background-color: var(--warning-color); color: black; min-width: 160px;" id="confirm-multi-btn" onclick="commitConfirmedTransaction(true)">Confirm &amp; Buy Another</button>
            <button class="btn-secondary" style="min-width: 160px;" id="confirm-cancel-btn" onclick="showScreen('view-overview')">Cancel</button>
        </div>
    </div>

    <div id="view-invoice" class="view-panel">
        <h2>Transaction Logged Successfully</h2>
        <div class="invoice-box">
            <h3>MARKET SIMULATION BALANCING RECORD</h3>
            <div><strong>Transaction Model:</strong> <span id="inv-type">N/A</span></div>
            <div><strong>Asset Reference:</strong> <span id="inv-asset">N/A</span></div>
            <div class="invoice-amount" id="inv-cash-flow">$0</div>
            <div id="inv-instruction" style="font-size: 0.9rem; color: #475569; border-top: 1px solid #e2e8f0; padding-top: 8px; line-height: 1.4;"></div>
        </div>
        <button class="btn-success" id="invoice-return-btn" onclick="returnToOverviewAfterInvoice()">Return to Overview Dashboard</button>
    </div>
</div>

<div id="input-modal-overlay" class="modal-overlay">
    <div class="modal-box">
        <div id="input-modal-title" class="modal-header">Input Required</div>
        <div id="input-modal-body" class="modal-body" style="white-space:pre-wrap;"></div>
        <input type="text" id="input-modal-field" style="margin-bottom:15px; font-size:1.1rem; letter-spacing:1px;" placeholder="">
        <div class="modal-footer">
            <button id="input-modal-cancel" class="btn-secondary" style="width:auto; padding:10px 20px;">Cancel</button>
            <button id="input-modal-confirm" class="btn-success" style="width:auto; padding:10px 20px;">Confirm</button>
        </div>
    </div>
</div>

<div id="custom-modal-overlay" class="modal-overlay">
    <div class="modal-box">
        <div id="custom-modal-title" class="modal-header">Notification</div>
        <div id="custom-modal-body" class="modal-body">Message contents...</div>
        <div id="custom-modal-footer" class="modal-footer">
            <button id="modal-btn-cancel" class="btn-secondary">Cancel</button>
            <button id="modal-btn-confirm" class="btn-success">OK</button>
        </div>
    </div>
</div>

<script>
    // --- COLLABORATIVE HARDCODED FIREBASE URL NODE CONNECTION ---
    const firebaseConfig = {
        databaseURL: "https://market-mayhem-tracker-default-rtdb.asia-southeast1.firebasedatabase.app/"
    };
    
    if (!firebase.apps.length) { firebase.initializeApp(firebaseConfig); }
    const rtdb = firebase.database();

    // --- SYSTEM FIXED ASSETS DICTIONARY STRUCTURES ---
    const PROFILE_DB = {
        "Z1": { id: "Z1", name: "The Risky Rizzler (Risk-Taker)", desc: "Goal: Total Portfolio Assets Value >= $1,100 AND simultaneously hold at least 4 High-Risk (🔴) assets." },
        "Z2": { id: "Z2", name: "The Safe Skibidi (Conservative)", desc: "Goal: Total Portfolio Assets Value >= $800, collection of at least 5 assets with ZERO High-Risk (🔴) assets." },
        "Z3": { id: "Z3", name: "The Balanced Baller (Balanced)", desc: "Goal: Own exactly 2 Low, 2 Mid, and 2 High risk items and accumulate baseline card passive yields >= $400." }
    };

    const ASSET_TEMPLATES = {
        "E1": { name: "ST Engineering", risk: 1, cost: 110, growth: 10, sector: "Tech" },
        "E2": { name: "Singtel", risk: 1, cost: 40, growth: 5, sector: "Consumer" },
        "E3": { name: "Johnson & Johnson", risk: 1, cost: 220, growth: 20, sector: "Healthcare" },
        "E4": { name: "DBS Bank", risk: 1, cost: 60, growth: 5, sector: "Financial" },
        "E5": { name: "Coca-Cola", risk: 1, cost: 70, growth: 5, sector: "Consumer" },
        "E6": { name: "Walmart", risk: 1, cost: 110, growth: 10, sector: "Consumer" },
        "E7": { name: "JPMorgan Chase & Co.", risk: 2, cost: 290, growth: 45, sector: "Financial" },
        "E8": { name: "Apple", risk: 2, cost: 310, growth: 45, sector: "Tech" },
        "E9": { name: "Microsoft", risk: 2, cost: 440, growth: 65, sector: "Tech" },
        "E10": { name: "Nike", risk: 2, cost: 40, growth: 5, sector: "Consumer" },
        "E11": { name: "Uber Technologies", risk: 2, cost: 70, growth: 10, sector: "Consumer" },
        "E12": { name: "Alphabet / Google", risk: 3, cost: 380, growth: 75, sector: "Tech" },
        "E13": { name: "Adobe", risk: 3, cost: 250, growth: 50, sector: "Tech" },
        "E14": { name: "Roblox", risk: 3, cost: 40, growth: 10, sector: "Tech" },
        "E15": { name: "Tesla", risk: 3, cost: 430, growth: 85, sector: "Energy" },
        "E16": { name: "NVIDIA", risk: 3, cost: 210, growth: 40, sector: "Tech" },
        "F1": { name: "SPDR Gold Shares (GLD)", risk: 1, cost: 400, growth: 40, sector: "Financial" },
        "F2": { name: "Vanguard S&P 500 ETF", risk: 2, cost: 340, growth: 50, sector: "Financial" },
        "F3": { name: "iShares Clean Energy ETF", risk: 3, cost: 220, growth: 45, sector: "Energy" },
        "P1": { name: "United SGD Money Market", risk: 1, cost: 120, growth: 5, sector: "Financial" },
        "P2": { name: "United SGD Fund", risk: 1, cost: 120, growth: 5, sector: "Financial" },
        "P3": { name: "United CIO Income Fund", risk: 2, cost: 120, growth: 10, sector: "Financial" },
        "P4": { name: "United CIO Growth Fund", risk: 3, cost: 120, growth: 15, sector: "Financial" },
        "P5": { name: "SaveUp Portfolio", risk: 1, cost: 120, growth: 5, sector: "Financial" },
        "P6": { name: "Asia Portfolio", risk: 2, cost: 120, growth: 20, sector: "Financial" },
        "P7": { name: "Global Portfolio", risk: 2, cost: 120, growth: 25, sector: "Financial" },
        "P8": { name: "Global Portfolio Plus", risk: 3, cost: 120, growth: 15, sector: "Financial" },
        "B1": { name: "Singapore Gov Bonds", risk: 1, cost: 100, growth: 3, sector: "Financial" },
        "B2": { name: "Astrea 8 PE Bond", risk: 2, cost: 100, growth: 5, sector: "Financial" },
        "B3": { name: "Frasers Property Bond", risk: 2, cost: 100, growth: 5, sector: "Financial" },
        "B4": { name: "iShares Asia High Yield Bond", risk: 3, cost: 100, growth: 8, sector: "Financial" }
    };

    const SCENARIO_DB = {
        "S1": { title: "US Fed Reserve Rate Hikes", rules: { "B1": 10, "P1": 10, "P2": 10, "P5": 10, "E7": -30, "E8": -30, "E9": -30, "E10": -30, "E11": -30, "B2": -10, "B3": -10, "F2": -25, "P3": -20, "P6": -20, "P7": -20, "E12": -65, "E13": -65, "E15": -65, "E16": -65, "E14": -15, "P4": -25, "P8": -25, "F3": -45 }, desc: "Low Risk bonds grow. Tech, Growth equities, and mixed portfolios crash heavily due to aggressive QT." },
        "S2": { title: "China Economic Stimulus", rules: { "E1": 10, "E4": 10, "F2": 30, "P6": 35, "B2": 15, "B3": 15, "E15": 50, "E16": 50, "B4": 25, "F3": 45 }, desc: "Beijing injects 4 trillion yuan. Regional Asian portfolios, corporate bonds, and hardware supply nodes surge." },
        "S3": { title: "Global Recession Fear", rules: { "P1": 15, "P5": 15, "E3": 15, "E5": 15, "E6": 15, "F2": -40, "E8": -30, "E9": -30, "E10": -30, "E11": -30, "E12": -70, "E13": -70, "E15": -70, "E16": -70, "E14": -20, "F1": 60 }, desc: "Stagflation scare. Growth items drop while physical Gold safe havens (F1) and standard staple equities move up." },
        "S4": { title: "Global Interest Rate Cuts", rules: { "B1": -10, "P1": -10, "P5": -10, "E8": 45, "E9": 45, "E10": 45, "F2": 40, "E12": 75, "E13": 75, "E16": 75, "E14": 20, "E15": 20, "P4": 30, "P8": 30 }, desc: "Lockdowns force emergency cuts nearing 0%. Cash yields contract while software architectures and hyper-growth options pop." },
        "S5": { title: "Supply Chain Chaos", rules: { "E1": -10, "E8": -35, "E10": -35, "E11": -20, "E15": -85, "E16": -40 }, desc: "Semiconductor bottlenecks heavily penalize tech hardware lines, electronics infrastructures, and EV manufacturing pipelines." },
        "S6": { title: "Inflation Shock", rules: { "E3": 10, "E5": 10, "E6": 10, "B1": -5, "E10": -30, "E11": -30, "F2": -40, "E13": -50, "E16": -45, "F1": 50 }, desc: "Valuations face compression. Consumer staple monopolies maintain strength while Gold hedges fiat debasement." },
        "S7": { title: "AI Technology Boom", rules: { "E1": 10, "E9": 65, "E8": 40, "F2": 35, "E16": 95, "E12": 75, "E13": 50, "E14": 15 }, desc: "Generative AI boom. Hardware GPU architectures, cloud titans, and advanced software layers accelerate dramatically." },
        "S8": { title: "Oil Price Spike", rules: { "E1": -15, "E5": -10, "E6": -10, "E11": -25, "P7": -15, "P8": -15, "F1": 40, "F3": 35, "E15": 45 }, desc: "Geopolitical conflict spikes energy. Squeezes global transit logistics while funding alternative transitions and Clean Energy elements." },
        "S9": { title: "Post-Pandemic Property Boom", rules: { "E4": 15, "B3": 15, "P3": 25, "P6": 20, "P7": 20, "P8": 30, "B4": 15 }, desc: "Liquidity influx into real estate. Yield portfolios, asset allocations, and property debt baskets experience large gains." },
        "S10": { title: "Green Energy Surge", rules: { "E1": 10, "P7": 15, "F3": 65, "E15": 85, "E9": 25 }, desc: "Direct federal tax credits and production grants unleash massive upward valuation support for clean energy structures." },
        "S11": { title: "Banking Crisis", rules: { "E4": -15, "B1": 15, "P1": 10, "P2": 10, "P5": 10, "E7": -60, "B3": -15, "B2": -15, "P6": -25, "B4": -30, "F2": -35 }, desc: "SVB liquidity run triggers regional contagion risks. Institutional financial elements drop while capital escapes to sovereign debt." },
        "S12": { title: "Healthcare Boom", rules: { "E3": 45, "E5": -10, "E6": -10, "E11": -30, "P3": 10, "E14": -15, "E15": -65 }, desc: "Pandemic vaccine and therapeutic production cycles generate high health sector expansion." },
        "S13": { title: "Consumer Spending Boom", rules: { "E2": 5, "E6": 15, "E10": 20, "E11": 25, "F2": 30, "B4": 15 }, desc: "Post-lockdown revenge spending spikes transaction and distribution volumes across retail apparel and mobility networks." },
        "S14": { title: "Energy Sector Collapse", rules: { "E5": 10, "E6": 10, "E9": 35, "E11": -25, "F1": 45, "B4": -30, "F3": -25 }, desc: "Lockdowns freeze travel. Oil hits negative values, breaking old fossil high-yield energy bonds while software structures stay safe." }
    };

    // --- ACTION CARD INFO LOOKUP ---
    const ACTION_DB_INFO = {
        "A3":  "A3: Diversification — Halves the loss value of your current round or last triggered Scenario round.",
        "A4":  "A4: Expert Advice — Peek at upcoming market trends.",
        "A6":  "A6: Safe Haven — Grants a single owned asset instance full immunity from the next Scenario value drop.",
        "A8":  "A8: Rebalance Portfolio — Swap one owned asset instance for any market card at current market price. Pay or collect the difference.",
        "A9":  "A9: Hedge Funds — After the next Scenario calculation, your single worst-performing holding's loss is cancelled to zero.",
        "A10": "A10: Investment Strategy — Select one owned asset. Its base passive growth yield is permanently doubled for all future scenarios.",
        "A11": "A11: Bad Advice — Penalty modifier. Your next Scenario round gain returns are halved.",
        "A12": "A12: Overconfidence — Double-edged risk modifier. Both your gains AND losses are doubled in the next Scenario.",
        "A15": "A15: Greed — Penalty modifier. Your total Scenario losses are doubled in the next triggered round.",
        "A16": "A16: Market Rumour — Choose a sector. All your holdings in that sector take double losses in the next Scenario.",
        "A19": "A19: FOMO — Forces rapid sector entry investments.",
        "A11_TARGET": "Attack Target with Bad Advice: Halves their next scenario round gains.",
        "A12_TARGET": "Attack Target with Overconfidence: Doubles their next scenario gains and losses.",
        "A15_TARGET": "Attack Target with Greed: Doubles their next total scenario losses.",
        "A16_TARGET": "Attack Target with Market Rumour: Target takes double losses inside a selected sector."
    };

    // --- TRACKER RUNTIME VARIABLES ---
    let lobbyRoomCode = "";
    let playerUsername = "";
    let globalMarketPrices = {}; 
    let ownedAssetInstances = [];     
    let instanceIdCounter = 1001;
    let chosenProfile = null;
    let lastExecutedScenarioKey = "";

    let activePlayerModifiers = { diversification: false, hedgeFunds: false, badAdvice: false, overconfidence: false, greed: false, marketRumourSector: null };
    let activeTransactionStaging = { type: "", cardId: "", instanceId: null, executionPrice: 0 };

    window.onload = function() {
        populateScenarioOptions();
        initializeLocalMarketPrices();
    };

    function populateScenarioOptions() {
        const select = document.getElementById("scenario-select");
        for (let key in SCENARIO_DB) {
            let opt = document.createElement("option");
            opt.value = key; opt.innerText = `${key}: ${SCENARIO_DB[key].title}`;
            select.appendChild(opt);
        }
    }

    function initializeLocalMarketPrices() {
        for (let key in ASSET_TEMPLATES) { globalMarketPrices[key] = ASSET_TEMPLATES[key].cost; }
    }

    function showScreen(screenId) {
        document.querySelectorAll('.view-panel').forEach(view => view.classList.remove('active-view'));
        document.getElementById(screenId).classList.add('active-view');
    }

    // --- INSTANT VIEW TRANSITION & HANDSHAKE ---
    function connectToLobbyRoom() {
        let code = document.getElementById("input-lobby-code").value.trim().toUpperCase();
        let name = document.getElementById("input-user-name").value.trim();
        
        if (!code) { openCustomModal("Input Error", "Please provide a valid Room ID code.", false); return; }
        if (!name) { openCustomModal("Input Error", "Please provide a game username to join.", false); return; }
        
        lobbyRoomCode = code;
        playerUsername = name;
        
        document.getElementById("lobby-status-pill").innerText = "LIVE SYNC";
        document.getElementById("lobby-status-pill").style.backgroundColor = "var(--success-color)";
        document.getElementById("room-code-banner").innerText = `Room: ${lobbyRoomCode} (${playerUsername})`;

        showScreen("view-setup");

        // Register profile username in room listing
        rtdb.ref(`rooms/${lobbyRoomCode}/players/${playerUsername}`).set({
            activeModifiers: { badAdvice: false, overconfidence: false, greed: false, marketRumourSector: "" }
        });

        // Initialize general market data values if needed
        rtdb.ref(`rooms/${lobbyRoomCode}/marketState`).once('value', (snapshot) => {
            if (!snapshot.exists()) {
                let initialPrices = {};
                for (let k in ASSET_TEMPLATES) { initialPrices[k] = ASSET_TEMPLATES[k].cost; }
                rtdb.ref(`rooms/${lobbyRoomCode}`).update({ marketState: initialPrices, activeScenarioTrigger: "" });
            }
        });

        // Listen for attacked external action modifiers targeting this user live
        rtdb.ref(`rooms/${lobbyRoomCode}/players/${playerUsername}/activeModifiers`).on('value', (snap) => {
            if (snap.exists()) {
                let remoteMods = snap.val();
                if (remoteMods.badAdvice) { activePlayerModifiers.badAdvice = true; rtdb.ref(`rooms/${lobbyRoomCode}/players/${playerUsername}/activeModifiers/badAdvice`).set(false); openCustomModal("Target Alert", "Another player targeted you with Bad Advice! (A11 applied)", false); }
                if (remoteMods.overconfidence) { activePlayerModifiers.overconfidence = true; rtdb.ref(`rooms/${lobbyRoomCode}/players/${playerUsername}/activeModifiers/overconfidence`).set(false); openCustomModal("Target Alert", "Another player targeted you with Overconfidence! (A12 applied)", false); }
                if (remoteMods.greed) { activePlayerModifiers.greed = true; rtdb.ref(`rooms/${lobbyRoomCode}/players/${playerUsername}/activeModifiers/greed`).set(false); openCustomModal("Target Alert", "Another player targeted you with Greed! (A15 applied)", false); }
                if (remoteMods.marketRumourSector) { activePlayerModifiers.marketRumourSector = remoteMods.marketRumourSector; rtdb.ref(`rooms/${lobbyRoomCode}/players/${playerUsername}/activeModifiers/marketRumourSector`).set(""); openCustomModal("Target Alert", `Another player targeted you with Market Rumour on sector: ${remoteMods.marketRumourSector}! (A16 applied)`, false); }
                renderPortfolioTable();
            }
        });

        // Fetch user tracking list dropdown context rules
        rtdb.ref(`rooms/${lobbyRoomCode}/players`).on('value', (snap) => {
            if (snap.exists()) { updateTargetDropdown(snap.val()); }
        });

        // Continuous market monitoring networks
        rtdb.ref(`rooms/${lobbyRoomCode}/marketState`).on('value', (snap) => {
            if (snap.exists()) {
                globalMarketPrices = snap.val();
                renderPortfolioTable();
                checkGoalCompliance();
            }
        });

        rtdb.ref(`rooms/${lobbyRoomCode}/activeScenarioTrigger`).on('value', (snap) => {
            let val = snap.val();
            if (val) { executeScenarioLogicLocally(val); }
        });
    }

    function updateTargetDropdown(playersList) {
        let select = document.getElementById("target-player-select");
        select.innerHTML = "";
        let count = 0;
        for (let pName in playersList) {
            if (pName !== playerUsername) {
                let opt = document.createElement("option");
                opt.value = pName;
                opt.innerText = pName;
                select.appendChild(opt);
                count++;
            }
        }
        // Toggle interface group container context
        let actionVal = document.getElementById("action-select").value;
        if (actionVal.includes("_TARGET") && count > 0) {
            document.getElementById("target-player-group").style.display = "block";
        } else {
            document.getElementById("target-player-group").style.display = "none";
        }
    }

    function initializeTrackerDashboard() {
        let pId = document.getElementById("player-profile-select").value;
        chosenProfile = PROFILE_DB[pId];
        document.getElementById("profile-text-desc").innerText = chosenProfile.desc;
        
        renderPortfolioTable();
        checkGoalCompliance();
        showScreen("view-overview");
    }

    function backToProfileSelection() { showScreen("view-setup"); }
    
    function previewScenarioInfo() {
        let key = document.getElementById("scenario-select").value;
        document.getElementById("scenario-preview-text").innerText = (key && SCENARIO_DB[key]) ? SCENARIO_DB[key].desc : "";
    }
    
    function previewActionInfo() {
        let key = document.getElementById("action-select").value;
        document.getElementById("action-preview-text").innerText = (key && ACTION_DB_INFO[key]) ? ACTION_DB_INFO[key] : "";
        
        // Dynamic target block displaying layout switches
        if (key.includes("_TARGET")) {
            document.getElementById("target-player-group").style.display = "block";
        } else {
            document.getElementById("target-player-group").style.display = "none";
        }
    }

    function openCustomModal(title, text, isConfirm, onConfirmCallback) {
        document.getElementById("custom-modal-title").innerText = title;
        document.getElementById("custom-modal-body").innerText = text;
        const btnCancel = document.getElementById("modal-btn-cancel");
        const btnConfirm = document.getElementById("modal-btn-confirm");
        const overlay = document.getElementById("custom-modal-overlay");
        btnCancel.style.display = isConfirm ? "inline-block" : "none";
        btnConfirm.innerText = isConfirm ? "Confirm" : "OK";

        let newConfirm = btnConfirm.cloneNode(true);
        let newCancel = btnCancel.cloneNode(true);
        btnConfirm.parentNode.replaceChild(newConfirm, btnConfirm);
        btnCancel.parentNode.replaceChild(newCancel, btnCancel);

        newConfirm.addEventListener("click", () => { overlay.classList.remove("active-modal"); if (onConfirmCallback) onConfirmCallback(); });
        newCancel.addEventListener("click", () => { overlay.classList.remove("active-modal"); });
        overlay.classList.add("active-modal");
    }

    // --- TERMINATE ROOM DATA DISCARD ROUTINES ---
    function triggerEndGameDiscard() {
        openCustomModal(
            "Wipe & Discard Room ID?", 
            `CRITICAL WARNING:\nConfirming this action deletes the shared Room ID [${lobbyRoomCode}] from the servers.\n\nThis immediately resets ALL active players. Proceed?`, 
            true, 
            () => {
                rtdb.ref(`rooms/${lobbyRoomCode}`).remove().then(() => {
                    location.reload();
                });
            }
        );
    }

    // --- RENDERING CORE MATRIX LAYERS ---
    function renderPortfolioTable() {
        const tbody = document.getElementById("portfolio-table-body"); tbody.innerHTML = "";
        let netTotalPortfolioValue = 0;

        ownedAssetInstances.forEach(inst => {
            netTotalPortfolioValue += inst.currentValue;
            let changeCell = `<span class="change-none">-</span>`;
            if (inst.netChange > 0) changeCell = `<span class="change-positive">+$${inst.netChange}</span>`;
            else if (inst.netChange < 0) changeCell = `<span class="change-negative">-$${Math.abs(inst.netChange)}</span>`;

            let badgeTags = "";
            if (inst.tags.immune) badgeTags += `<span class="active-mod-tag">Immune (A6)</span>`;
            if (inst.tags.doubleGrowth) badgeTags += `<span class="active-mod-tag">x2 Growth (A10)</span>`;
            if (activePlayerModifiers.marketRumourSector === inst.sector) badgeTags += `<span class="active-mod-tag">x2 Sector Loss (A16)</span>`;

            // Evaluate highlight colors based on Purchase versus Current values
            let buyPriceClass = "";
            if (inst.currentValue > inst.boughtPrice) buyPriceClass = "bought-profit";
            else if (inst.currentValue < inst.boughtPrice) buyPriceClass = "bought-loss";

            tbody.innerHTML += `
                <tr>
                    <td><small style="font-family:monospace; color:#94a3b8;">#${inst.instanceId}</small></td>
                    <td><strong>${inst.cardId}</strong></td>
                    <td>${inst.name} ${badgeTags}</td>
                    <td><span class="risk-badge risk-${inst.risk}">Risk ${inst.risk}</span></td>
                    <td class="${buyPriceClass}">$${inst.boughtPrice}</td>
                    <td style="font-size: 1.1rem; font-weight: bold; color: var(--success-color);">$${inst.currentValue}</td>
                    <td>${changeCell}</td>
                </tr>
            `;
        });

        if (ownedAssetInstances.length === 0) {
            tbody.innerHTML = `<tr><td colspan="7" style="text-align: center; color: #64748b; font-style: italic;">No investment assets currently held. click Buy Asset above to explore market items.</td></tr>`;
        }
        document.getElementById("total-portfolio-display").innerText = `$${netTotalPortfolioValue}`;
    }

    function openBuyMarketScreen() {
        const tbody = document.getElementById("buy-market-table-body"); tbody.innerHTML = "";
        for (let code in ASSET_TEMPLATES) {
            let template = ASSET_TEMPLATES[code];
            let currentMarketCostPrice = globalMarketPrices[code] || template.cost; 
            tbody.innerHTML += `
                <tr>
                    <td><strong>${code}</strong></td>
                    <td>${template.name}</td>
                    <td><span class="risk-badge risk-${template.risk}">Risk ${template.risk}</span></td>
                    <td>${template.sector}</td>
                    <td style="font-size: 1.1rem; font-weight: bold; color: var(--warning-color);">$${currentMarketCostPrice}</td>
                    <td><button class="btn-success" style="padding:6px 12px; font-size:0.9rem; width:auto;" onclick="stageBuyConfirmation('${code}')">Select Buy</button></td>
                </tr>
            `;
        }
        showScreen("view-buy-market");
    }

    function stageBuyConfirmation(cardId) {
        let template = ASSET_TEMPLATES[cardId]; let currentMarketPrice = globalMarketPrices[cardId] || template.cost;
        activeTransactionStaging = { type: "BUY", cardId: cardId, instanceId: null, executionPrice: currentMarketPrice };
        document.getElementById("confirm-action-type").innerText = "CONFIRM PURCHASE REGISTRATION";
        document.getElementById("confirm-asset-details").innerText = `[${cardId}] ${template.name} (${template.sector} Sector)`;
        document.getElementById("confirm-price-readout").innerText = `$${currentMarketPrice}`;
        document.getElementById("confirm-price-readout").style.color = "var(--warning-color)";
        document.getElementById("confirm-cancel-btn").setAttribute("onclick", "openBuyMarketScreen()");
        showScreen("view-confirm-transaction");
    }

    function openSellPortfolioScreen() {
        const tbody = document.getElementById("sell-portfolio-table-body"); tbody.innerHTML = "";
        if (ownedAssetInstances.length === 0) tbody.innerHTML = `<tr><td colspan="6" style="text-align: center; color: #64748b; font-style: italic; padding: 20px 10px;">Your portfolio contains no holdings to sell.</td></tr>`;
        ownedAssetInstances.forEach(inst => {
            tbody.innerHTML += `
                <tr>
                    <td><small style="font-family:monospace; color:#94a3b8;">#${inst.instanceId}</small></td>
                    <td><strong>${inst.cardId}</strong></td>
                    <td>${inst.name}</td>
                    <td><span class="risk-badge risk-${inst.risk}">Risk ${inst.risk}</span></td>
                    <td style="font-size: 1.1rem; font-weight: bold; color: var(--success-color);">$${inst.currentValue}</td>
                    <td><button class="btn-danger" style="padding:6px 12px; font-size:0.9rem; width:auto;" onclick="stageSellConfirmation(${inst.instanceId})">Select Sell</button></td>
                </tr>
            `;
        });
        showScreen("view-sell-portfolio");
    }

    function stageSellConfirmation(instanceId) {
        let inst = ownedAssetInstances.find(x => x.instanceId === instanceId); if (!inst) return;
        activeTransactionStaging = { type: "SELL", cardId: inst.cardId, instanceId: instanceId, executionPrice: inst.currentValue };
        document.getElementById("confirm-action-type").innerText = "CONFIRM LIQUIDATION SALE REGISTRATION";
        document.getElementById("confirm-asset-details").innerText = `Instance #${inst.instanceId} - [${inst.cardId}] ${inst.name}`;
        document.getElementById("confirm-price-readout").innerText = `$${inst.currentValue}`;
        document.getElementById("confirm-price-readout").style.color = "var(--success-color)";
        document.getElementById("confirm-cancel-btn").setAttribute("onclick", "openSellPortfolioScreen()");
        showScreen("view-confirm-transaction");
    }

    function commitConfirmedTransaction(wantsToBuyAnother) {
        let cardId = activeTransactionStaging.cardId; let price = activeTransactionStaging.executionPrice;
        if (activeTransactionStaging.type === "BUY") {
            ownedAssetInstances.push({ instanceId: instanceIdCounter++, cardId: cardId, name: ASSET_TEMPLATES[cardId].name, risk: ASSET_TEMPLATES[cardId].risk, boughtPrice: price, currentValue: price, netChange: 0, sector: ASSET_TEMPLATES[cardId].sector, tags: { immune: false, doubleGrowth: false } });
            document.getElementById("inv-type").innerText = "ASSET PURCHASE SECURED (BUY)";
            document.getElementById("inv-cash-flow").innerText = `-$${price}`; document.getElementById("inv-cash-flow").style.color = "var(--danger-color)";
            document.getElementById("inv-instruction").innerText = `BANK NOTIFICATION: Pay $${price} cash to banker. Tokens go UNDER the physical layout card.`;
        } else {
            let targetIdx = ownedAssetInstances.findIndex(x => x.instanceId === activeTransactionStaging.instanceId); if (targetIdx !== -1) ownedAssetInstances.splice(targetIdx, 1);
            document.getElementById("inv-type").innerText = "ASSET PORTFOLIO LIQUIDATION (SELL)";
            document.getElementById("inv-cash-flow").innerText = `+$${price}`; document.getElementById("inv-cash-flow").style.color = "var(--success-color)";
            document.getElementById("inv-instruction").innerText = `BANK NOTIFICATION: Return physical card layout. Banker pays player back $${price} from card cache notes.`;
        }
        document.getElementById("inv-asset").innerText = cardId;
        
        // Handle routing toggle conditional loops for multi-buys
        if (wantsToBuyAnother && activeTransactionStaging.type === "BUY") {
            document.getElementById("invoice-return-btn").setAttribute("onclick", "openBuyMarketScreen(); renderPortfolioTable(); checkGoalCompliance();");
        } else {
            document.getElementById("invoice-return-btn").setAttribute("onclick", "returnToOverviewAfterInvoice()");
        }
        
        showScreen("view-invoice");
    }

    function returnToOverviewAfterInvoice() { renderPortfolioTable(); checkGoalCompliance(); showScreen("view-overview"); }

    function openInputModal(title, body, placeholder, onConfirm) {
        document.getElementById("input-modal-title").innerText = title;
        document.getElementById("input-modal-body").innerText = body;
        const field = document.getElementById("input-modal-field");
        field.value = "";
        field.placeholder = placeholder || "";
        field.type = (placeholder && placeholder.toLowerCase().includes("id")) ? "number" : "text";
        const overlay = document.getElementById("input-modal-overlay");
        const btnConfirm = document.getElementById("input-modal-confirm");
        const btnCancel = document.getElementById("input-modal-cancel");
        const newConfirm = btnConfirm.cloneNode(true);
        const newCancel = btnCancel.cloneNode(true);
        btnConfirm.parentNode.replaceChild(newConfirm, btnConfirm);
        btnCancel.parentNode.replaceChild(newCancel, btnCancel);
        newConfirm.addEventListener("click", () => { overlay.classList.remove("active-modal"); onConfirm(field.value.trim()); });
        newCancel.addEventListener("click", () => { overlay.classList.remove("active-modal"); resetActionSelectionFields(); });
        overlay.classList.add("active-modal");
        setTimeout(() => field.focus(), 100);
    }

    function resetActionSelectionFields() {
        document.getElementById("action-select").value = ""; 
        document.getElementById("action-preview-text").innerText = "";
        document.getElementById("target-player-group").style.display = "none";
    }

    function executeActionCardDirect() {
        let cardKey = document.getElementById("action-select").value; if (!cardKey) return;
        
        // Handle targeted peer attacks dynamically using Firebase paths without requiring card entry actions
        if (cardKey.includes("_TARGET")) {
            let targetedPlayer = document.getElementById("target-player-select").value;
            if (!targetedPlayer) { openCustomModal("Selection Error", "No other player found in room list to target.", false); return; }
            
            let baseKey = cardKey.split("_")[0]; // extraction string (e.g. A11)
            
            if (baseKey === "A16") {
                openInputModal("A16: Target Sector Attack", "Type the target sector for your opponent's holdings:", "Tech / Consumer / Healthcare / Financial / Energy", (val) => {
                    let sect = val.trim(); if (!sect) return;
                    rtdb.ref(`rooms/${lobbyRoomCode}/players/${targetedPlayer}/activeModifiers`).update({ marketRumourSector: sect });
                    openCustomModal("Attack Deployed", `Sent Market Rumour (${sect}) directly to player ${targetedPlayer}!`, false);
                    resetActionSelectionFields();
                });
            } else {
                let nodeUpdate = {};
                if (baseKey === "A11") nodeUpdate = { badAdvice: true };
                if (baseKey === "A12") nodeUpdate = { overconfidence: true };
                if (baseKey === "A15") nodeUpdate = { greed: true };
                
                rtdb.ref(`rooms/${lobbyRoomCode}/players/${targetedPlayer}/activeModifiers`).update(nodeUpdate);
                openCustomModal("Attack Deployed", `Successfully casted Action ${baseKey} against player ${targetedPlayer}!`, false);
                resetActionSelectionFields();
            }
            return;
        }

        // Standard local execution card logic flows
        if (cardKey === "A3") { 
            activePlayerModifiers.diversification = true; 
            // Run A3 effect instantly on the current or active round calculation state
            if (lastExecutedScenarioKey) {
                openCustomModal("A3 Activated Retroactively", "A3 Diversification logged! Modifying value points on current scenario retroactively.", false);
                recomputeScenarioWithA3(lastExecutedScenarioKey);
            } else {
                openCustomModal("Action Card Logged", "A3 Diversification active. Next round scenario loss structures halved.", false); 
            }
        }
        else if (cardKey === "A4") { openCustomModal("A4: Expert Advice Logged", "Action profile set. You peek at upcoming market trendlines.", false); }
        else if (cardKey === "A19") { openCustomModal("A19: FOMO Logged", "Action parameter set. Rapid sector allocation required.", false); }
        else if (cardKey === "A6") {
            if (ownedAssetInstances.length === 0) { openCustomModal("Action Refused", "No active holding instances present to protect.", false); return; }
            let t = "Type the Instance ID to protect:\n\n"; ownedAssetInstances.forEach(i => { t += `#${i.instanceId}: [${i.cardId}] ${i.name}\n`; });
            openInputModal("A6: Safe Haven", t, "e.g. 1001", (val) => {
                let tid = parseInt(val); let m = ownedAssetInstances.find(x => x.instanceId === tid);
                if (m) { m.tags.immune = true; openCustomModal("Action Card Logged", `Instance #${tid} is now immune from the next value shock drop.`, false); }
                else { openCustomModal("Invalid ID", "No matching instance found. Action cancelled.", false); }
                resetActionSelectionFields();
                renderPortfolioTable();
            }); return;
        }
        else if (cardKey === "A8") {
            if (ownedAssetInstances.length === 0) return;
            let t = "Type the Instance ID to swap out:\n\n"; ownedAssetInstances.forEach(i => { t += `ID #${i.instanceId} : [${i.cardId}] ($${i.currentValue})\n`; });
            openInputModal("A8: Rebalance — Step 1", t, "e.g. 1001", (idVal) => {
                let oldId = parseInt(idVal); let oldInst = ownedAssetInstances.find(x => x.instanceId === oldId); if (!oldInst) { openCustomModal("Invalid ID", "No matching instance found.", false); return; }
                openInputModal("A8: Rebalance — Step 2", `Swapping out #${oldId} [${oldInst.cardId}]\n\nEnter replacement Market Card Code:`, "e.g. E9", (codeVal) => {
                    let newCode = codeVal.toUpperCase(); if (!ASSET_TEMPLATES.hasOwnProperty(newCode)) { openCustomModal("Invalid Code", `'${newCode}' is not a valid asset code.`, false); return; }
                    let diff = oldInst.currentValue - (globalMarketPrices[newCode] || ASSET_TEMPLATES[newCode].cost);
                    ownedAssetInstances.splice(ownedAssetInstances.findIndex(x => x.instanceId === oldId), 1);
                    ownedAssetInstances.push({ instanceId: instanceIdCounter++, cardId: newCode, name: ASSET_TEMPLATES[newCode].name, risk: ASSET_TEMPLATES[newCode].risk, boughtPrice: (globalMarketPrices[newCode] || ASSET_TEMPLATES[newCode].cost), currentValue: (globalMarketPrices[newCode] || ASSET_TEMPLATES[newCode].cost), netChange: 0, sector: ASSET_TEMPLATES[newCode].sector, tags: { immune: false, doubleGrowth: false } });
                    document.getElementById("inv-type").innerText = "PORTFOLIO REBALANCE SWAP (A8)";
                    document.getElementById("inv-asset").innerText = `Traded #${oldId} away for a new copy of [${newCode}]`;
                    document.getElementById("inv-cash-flow").innerText = (diff >= 0 ? "+" : "-") + `$${Math.abs(diff)}`;
                    document.getElementById("inv-cash-flow").style.color = diff >= 0 ? "var(--success-color)" : "var(--danger-color)";
                    document.getElementById("inv-instruction").innerText = diff >= 0 ? `Collect exactly +$${diff} from banker.` : `Hand exactly $${Math.abs(diff)} to banker.`;
                    resetActionSelectionFields();
                    showScreen("view-invoice");
                });
            }); return;
        }
        else if (cardKey === "A9") { activePlayerModifiers.hedgeFunds = true; openCustomModal("Action Card Logged", "Hedge funds active.", false); }
        else if (cardKey === "A10") {
            if (ownedAssetInstances.length === 0) return;
            let t = "Type the Instance ID to apply double growth:\n\n"; ownedAssetInstances.forEach(i => { t += `ID #${i.instanceId} : [${i.cardId}]\n`; });
            openInputModal("A10: Investment Strategy", t, "e.g. 1001", (val) => {
                let tid = parseInt(val); let m = ownedAssetInstances.find(x => x.instanceId === tid);
                if (m) { m.tags.doubleGrowth = true; openCustomModal("Action Card Logged", "Instance set to generate double growth round speeds.", false); }
                else { openCustomModal("Invalid ID", "No matching instance found. Action cancelled.", false); }
                resetActionSelectionFields();
                renderPortfolioTable();
            }); return;
        }
        else if (cardKey === "A11") { activePlayerModifiers.badAdvice = true; openCustomModal("Action Card Logged", "Bad advice logged.", false); }
        else if (cardKey === "A12") { activePlayerModifiers.overconfidence = true; openCustomModal("Action Card Logged", "Overconfidence logged.", false); }
        else if (cardKey === "A15") { activePlayerModifiers.greed = true; openCustomModal("Action Card Logged", "Greed logged.", false); }
        else if (cardKey === "A16") { 
            openInputModal("A16: Market Rumour", "Type the target sector:", "Tech / Consumer / Healthcare / Financial / Energy", (val) => {
                let sIn = val.trim(); if (!sIn) return;
                activePlayerModifiers.marketRumourSector = sIn; 
                openCustomModal("Action Card Logged", `Rumours targeting ${sIn}.`, false);
                resetActionSelectionFields();
                renderPortfolioTable();
            }); return;
        }

        resetActionSelectionFields();
        renderPortfolioTable();
    }

    function triggerScenarioConfirmation() {
        let key = document.getElementById("scenario-select").value;
        if (!key) { openCustomModal("Missing Selection", "Please select an active scenario card first.", false); return; }
        
        openCustomModal(`Confirm Broadcast: ${key}`, `Confirm execution for ${key}? This updates the database and triggers updates across ALL connected devices simultaneously.`, true, () => {
            let scenario = SCENARIO_DB[key];
            let nextMarketPriceState = { ...globalMarketPrices };
            for (let code in ASSET_TEMPLATES) {
                if (scenario.rules.hasOwnProperty(code)) {
                    nextMarketPriceState[code] += scenario.rules[code];
                } else {
                    nextMarketPriceState[code] += ASSET_TEMPLATES[code].growth;
                }
                if (nextMarketPriceState[code] < 0) nextMarketPriceState[code] = 0;
            }

            rtdb.ref(`rooms/${lobbyRoomCode}`).update({
                marketState: nextMarketPriceState,
                activeScenarioTrigger: key + "_" + Date.now()
            });
        });
    }

    function executeScenarioLogicLocally(triggerString) {
        let scenarioKey = triggerString.split("_")[0]; let scenario = SCENARIO_DB[scenarioKey];
        lastExecutedScenarioKey = scenarioKey; // Store instance signature for retroactive execution properties
        let instanceDeltaRegistry = {};

        ownedAssetInstances.forEach(inst => {
            let code = inst.cardId; let hasScenarioRule = scenario.rules.hasOwnProperty(code); let change = 0;
            if (hasScenarioRule) {
                change = scenario.rules[code];
                if (change < 0) {
                    if (inst.tags.immune) { change = 0; } else {
                        if (activePlayerModifiers.overconfidence) change *= 2; if (activePlayerModifiers.greed) change *= 2;
                        if (activePlayerModifiers.diversification) change = Math.floor(change * 0.5);
                        if (activePlayerModifiers.marketRumourSector === inst.sector) change *= 2;
                    }
                } else {
                    if (activePlayerModifiers.overconfidence) change *= 2;
                    if (activePlayerModifiers.badAdvice) change = Math.floor(change * 0.5);
                }
            } else {
                change = ASSET_TEMPLATES[code].growth;
                if (inst.tags.doubleGrowth) change *= 2;
                if (activePlayerModifiers.badAdvice) change = Math.floor(change * 0.5);
            }
            instanceDeltaRegistry[inst.instanceId] = change;
        });

        if (activePlayerModifiers.hedgeFunds) {
            let worstId = null; let worstAmt = 0;
            ownedAssetInstances.forEach(inst => {
                let d = instanceDeltaRegistry[inst.instanceId];
                if (d < worstAmt) { worstAmt = d; worstId = inst.instanceId; }
            });
            if (worstId) instanceDeltaRegistry[worstId] = 0;
        }

        ownedAssetInstances.forEach(inst => {
            let d = instanceDeltaRegistry[inst.instanceId];
            inst.netChange = d; inst.currentValue += d;
            if (inst.currentValue < 0) inst.currentValue = 0;
            inst.tags.immune = false; 
        });

        activePlayerModifiers.diversification = false; activePlayerModifiers.hedgeFunds = false;
        activePlayerModifiers.badAdvice = false; activePlayerModifiers.overconfidence = false;
        activePlayerModifiers.greed = false; activePlayerModifiers.marketRumourSector = null;

        document.getElementById("scenario-select").value = "";
        document.getElementById("scenario-preview-text").innerText = "";

        renderPortfolioTable();
        checkGoalCompliance();

        openCustomModal("Scenario Notification", `Scenario executed inside room:\n[${scenarioKey}] ${scenario.title}\n\nYour numbers have updated automatically. Check Net Change flags.`, false);
    }

    // Retroactive mitigation adjustment computation engine for A3 Diversification
    function recomputeScenarioWithA3(scenarioKey) {
        let scenario = SCENARIO_DB[scenarioKey];
        ownedAssetInstances.forEach(inst => {
            // Check if this card code suffered a drop during the current active session
            if (scenario.rules.hasOwnProperty(inst.cardId) && scenario.rules[inst.cardId] < 0) {
                let originalLoss = inst.netChange;
                let mitigatedLoss = Math.floor(originalLoss * 0.5);
                let recoveryAdjustment = mitigatedLoss - originalLoss; // Positive delta points back
                
                inst.currentValue += recoveryAdjustment;
                inst.netChange = mitigatedLoss;
                if (inst.currentValue < 0) inst.currentValue = 0;
            }
        });
        activePlayerModifiers.diversification = false;
        renderPortfolioTable();
        checkGoalCompliance();
    }

    function checkGoalCompliance() {
        if (!chosenProfile) return;
        let totVal = ownedAssetInstances.reduce((sum, i) => sum + i.currentValue, 0);
        let low = 0; let mid = 0; let high = 0;
        ownedAssetInstances.forEach(i => { if (i.risk === 1) low++; if (i.risk === 2) mid++; if (i.risk === 3) high++; });

        let met = false;
        // Updated investor goals targeting updated net worth calibrations
        if (chosenProfile.id === "Z1") met = (totVal >= 1100 && high >= 4);
        else if (chosenProfile.id === "Z2") met = (totVal >= 800 && ownedAssetInstances.length >= 5 && high === 0);
        else if (chosenProfile.id === "Z3") met = (ownedAssetInstances.length >= 6 && low >= 2 && mid >= 2 && high >= 2);

        const ind = document.getElementById("goal-status-box");
        if (met) {
            ind.innerText = "Target Objective Achieved! 🎉"; ind.className = "goal-indicator goal-met";
            document.body.classList.add("goal-achieved");
        } else {
            ind.innerText = "Objective Parameters Unmet"; ind.className = "goal-indicator goal-not-met";
            document.body.classList.remove("goal-achieved");
        }
    }
</script>
</body>
</html>
