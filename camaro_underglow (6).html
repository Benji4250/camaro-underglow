<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>UNDERGLOW // CAMARO</title>
<style>
  :root {
    --bg:#080a0f; --bg2:#0d1018; --bg3:#121620; --panel:#0f1319;
    --border:#1e2530; --border2:#252d3a;
    --accent:#e8312a; --accent2:#ff5a52;
    --amber:#f5a623; --green:#2ecc71; --blue:#3498db;
    --text:#c8d0dc; --text2:#6b7585; --text3:#3a4252; --white:#eef2f8;
  }
  *{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
  body{background:var(--bg);color:var(--text);font-family:-apple-system,'Helvetica Neue',Arial,sans-serif;min-height:100vh;overflow-x:hidden;}

  header{background:var(--bg2);border-bottom:2px solid var(--accent);padding:0 16px;display:flex;align-items:center;justify-content:space-between;height:54px;position:sticky;top:0;z-index:100;}
  .logo{font-size:20px;font-weight:800;letter-spacing:4px;color:var(--white);text-transform:uppercase;}
  .logo span{color:var(--accent);}
  .conn-badge{display:flex;align-items:center;gap:7px;padding:6px 14px;border-radius:20px;border:1px solid var(--border2);background:var(--bg3);font-size:11px;font-weight:700;letter-spacing:1.5px;cursor:pointer;user-select:none;}
  .dot{width:8px;height:8px;border-radius:50%;background:var(--text3);transition:background .5s,box-shadow .5s;}
  .dot.on{background:var(--green);box-shadow:0 0 8px var(--green);animation:blink 2s infinite;}
  .dot.err{background:var(--accent);box-shadow:0 0 8px var(--accent);}
  @keyframes blink{0%,100%{opacity:1}50%{opacity:.35}}

  .tabs{display:flex;background:var(--bg2);border-bottom:1px solid var(--border);position:sticky;top:54px;z-index:99;}
  .tab{flex:1;padding:13px 8px;text-align:center;font-size:12px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--text2);cursor:pointer;border-bottom:3px solid transparent;transition:all .2s;user-select:none;}
  .tab.active{color:var(--accent);border-bottom-color:var(--accent);}

  .page{display:none;padding:14px;max-width:900px;margin:0 auto;}
  .page.active{display:block;}

  /* SLAVE STATUS */
  .slave-panel{background:var(--panel);border:1px solid var(--border);border-radius:10px;padding:12px 14px;margin-bottom:14px;}
  .slave-hdr{font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--text2);margin-bottom:10px;}
  .slave-row{display:flex;gap:8px;}
  .slave-pill{flex:1;border-radius:8px;border:1px solid var(--border2);background:var(--bg3);padding:10px 4px;display:flex;flex-direction:column;align-items:center;gap:5px;transition:all .5s;}
  .slave-pill.online{border-color:var(--green);background:rgba(46,204,113,.07);box-shadow:0 0 10px rgba(46,204,113,.12);}
  .slave-pill.offline{border-color:var(--accent);background:rgba(232,49,42,.07);}
  .slave-num{font-size:12px;font-weight:800;letter-spacing:1px;color:var(--text3);transition:color .5s;}
  .slave-pill.online .slave-num{color:var(--green);}
  .slave-pill.offline .slave-num{color:var(--accent2);}
  .slave-dot{width:8px;height:8px;border-radius:50%;background:var(--text3);transition:all .5s;}
  .slave-pill.online .slave-dot{background:var(--green);box-shadow:0 0 6px var(--green);animation:blink 2s infinite;}
  .slave-pill.offline .slave-dot{background:var(--accent);}
  .slave-zones{font-size:9px;color:var(--text3);font-weight:600;letter-spacing:.3px;text-align:center;line-height:1.4;transition:color .5s;}
  .slave-pill.online .slave-zones{color:var(--text2);}
  .slave-pill.offline .slave-zones{color:rgba(232,49,42,.6);}

  /* STATUS CARDS */
  .sgrid{display:grid;grid-template-columns:repeat(3,1fr);gap:9px;margin-bottom:14px;}
  .scard{background:var(--panel);border:1px solid var(--border);border-radius:10px;padding:14px 8px 12px;display:flex;flex-direction:column;align-items:center;gap:7px;transition:border-color .3s,background .3s,box-shadow .3s;}
  .scard.on{border-color:var(--accent);background:rgba(232,49,42,.08);box-shadow:0 0 16px rgba(232,49,42,.2);}
  .sicon{font-size:22px;transition:filter .3s;filter:grayscale(1) opacity(.35);}
  .scard.on .sicon{filter:none;}
  .slbl{font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--text2);text-align:center;transition:color .3s;}
  .scard.on .slbl{color:var(--accent2);}

  .lpanel{background:var(--panel);border:1px solid var(--border);border-radius:10px;padding:14px 16px;margin-bottom:14px;}
  .lhdr{display:flex;justify-content:space-between;align-items:center;margin-bottom:10px;}
  .seclbl{font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--text2);}
  .dnbadge{font-size:11px;font-weight:700;padding:4px 10px;border-radius:12px;border:1px solid var(--border2);letter-spacing:1px;transition:all .4s;}
  .dnbadge.night{color:var(--blue);border-color:var(--blue);background:rgba(52,152,219,.1);}
  .dnbadge.day{color:var(--amber);border-color:var(--amber);background:rgba(245,166,35,.1);}
  .ltrack{height:6px;background:var(--bg3);border-radius:3px;overflow:hidden;}
  .lfill{height:100%;border-radius:3px;background:linear-gradient(90deg,#3498db,#f5a623,#fff);transition:width .4s;width:0;}
  .lval{font-size:10px;color:var(--text2);margin-top:5px;text-align:right;font-weight:600;}
  .ticker{font-size:10px;color:var(--text3);text-align:center;padding:10px;letter-spacing:1px;font-weight:600;}

  /* CONFIG */
  .sechdr{font-size:11px;font-weight:700;letter-spacing:3px;text-transform:uppercase;color:var(--text2);margin-bottom:10px;padding-bottom:8px;border-bottom:1px solid var(--border);display:flex;align-items:center;gap:8px;}
  .sechdr::before{content:'';width:3px;height:14px;background:var(--accent);border-radius:2px;}
  .ggrid{display:grid;grid-template-columns:repeat(2,1fr);gap:9px;margin-bottom:22px;}
  .togcard{background:var(--panel);border:1px solid var(--border);border-radius:10px;padding:14px;display:flex;align-items:center;justify-content:space-between;gap:10px;cursor:pointer;user-select:none;transition:all .2s;}
  .togcard.on{border-color:rgba(232,49,42,.5);background:rgba(232,49,42,.05);}
  .togname{font-size:13px;font-weight:700;color:var(--white);}
  .togdesc{font-size:11px;color:var(--text2);margin-top:2px;}
  .sw{width:42px;height:24px;border-radius:12px;background:var(--bg3);border:1px solid var(--border2);position:relative;flex-shrink:0;transition:all .25s;}
  .sw::after{content:'';position:absolute;width:18px;height:18px;border-radius:50%;background:var(--text3);top:2px;left:2px;transition:all .25s;}
  .sw.on{background:rgba(232,49,42,.2);border-color:var(--accent);}
  .sw.on::after{left:20px;background:var(--accent);box-shadow:0 0 8px rgba(232,49,42,.5);}

  /* CHANGE ALL */
  .chgall-card{background:var(--panel);border:1px solid var(--border2);border-radius:10px;margin-bottom:14px;overflow:hidden;}
  .chgall-hdr{padding:14px;display:flex;align-items:center;justify-content:space-between;cursor:pointer;user-select:none;}
  .chgall-title{font-size:14px;font-weight:700;color:var(--white);}
  .chgall-sub{font-size:11px;color:var(--text2);margin-top:2px;}
  .chgall-swatch{width:30px;height:30px;border-radius:7px;border:1px solid var(--border2);flex-shrink:0;}
  .chgall-body{display:none;padding:0 14px 14px;border-top:1px solid var(--border);}
  .chgall-card.open .chgall-body{display:block;}
  .chgall-card.open .chev2{transform:rotate(180deg);}
  .chev2{color:var(--text3);font-size:14px;transition:transform .2s;}
  .chgall-apply{width:100%;margin-top:14px;padding:12px;border:none;border-radius:8px;background:var(--accent);color:#fff;font-size:13px;font-weight:800;letter-spacing:2px;text-transform:uppercase;cursor:pointer;transition:all .15s;}
  .chgall-apply:active{transform:scale(.97);}
  .scope-row{display:flex;gap:7px;margin-top:12px;flex-wrap:wrap;}
  .scope-btn{flex:1;min-width:70px;padding:8px 4px;border-radius:7px;border:1px solid var(--border);background:var(--bg3);text-align:center;cursor:pointer;font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--text2);transition:all .2s;user-select:none;}
  .scope-btn.on{border-color:var(--accent);background:rgba(232,49,42,.1);color:var(--accent2);}

  /* ZONE CARDS */
  .zcard{background:var(--panel);border:1px solid var(--border);border-radius:10px;margin-bottom:9px;overflow:hidden;}
  .zhdr{padding:13px 14px;display:flex;align-items:center;gap:12px;cursor:pointer;user-select:none;}
  .zswatch{width:30px;height:30px;border-radius:7px;border:1px solid var(--border2);flex-shrink:0;transition:background .3s;}
  .zname{font-size:14px;font-weight:700;color:var(--white);}
  .zmeta{font-size:10px;color:var(--text2);margin-top:2px;letter-spacing:.5px;font-weight:600;}
  .chev{color:var(--text3);font-size:14px;transition:transform .2s;margin-left:auto;}
  .zcard.open .chev{transform:rotate(180deg);}
  .zbody{display:none;padding:0 14px 14px;border-top:1px solid var(--border);}
  .zcard.open .zbody{display:block;}
  .slrow{display:flex;align-items:center;gap:10px;margin-top:11px;}
  .sllbl{font-size:11px;font-weight:700;color:var(--text2);width:26px;}
  .slwrap{flex:1;}
  input[type=range]{width:100%;height:4px;appearance:none;-webkit-appearance:none;background:var(--bg3);border-radius:2px;outline:none;cursor:pointer;}
  input[type=range]::-webkit-slider-thumb{-webkit-appearance:none;width:18px;height:18px;border-radius:50%;background:var(--white);border:2px solid var(--border2);cursor:pointer;}
  .slval{font-size:11px;font-weight:700;color:var(--text);width:30px;text-align:right;}
  .clrprev{display:flex;align-items:center;gap:10px;margin-top:12px;padding:10px;background:var(--bg3);border-radius:8px;border:1px solid var(--border);}
  .clrsw{width:42px;height:42px;border-radius:8px;border:1px solid var(--border2);flex-shrink:0;}
  .clrvals{font-size:11px;color:var(--text2);line-height:1.9;font-weight:600;}
  .zopts{display:flex;gap:8px;margin-top:12px;}
  .zopt{flex:1;padding:9px 4px;border-radius:7px;border:1px solid var(--border);background:var(--bg3);text-align:center;cursor:pointer;font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--text2);transition:all .2s;user-select:none;}
  .zopt.on{border-color:var(--accent);background:rgba(232,49,42,.1);color:var(--accent2);}

  .unsaved{background:rgba(245,166,35,.1);border:1px solid rgba(245,166,35,.4);border-radius:8px;padding:9px 14px;margin-bottom:14px;font-size:11px;font-weight:700;color:var(--amber);letter-spacing:.5px;display:none;align-items:center;justify-content:space-between;}
  .unsaved.show{display:flex;}

  /* POLICE MODE BUTTON */
  .police-btn{width:100%;padding:16px;border:none;border-radius:10px;font-size:14px;font-weight:800;letter-spacing:3px;text-transform:uppercase;cursor:pointer;transition:all .2s;margin-bottom:14px;display:flex;align-items:center;justify-content:center;gap:10px;background:var(--panel);color:var(--text2);border:1px solid var(--border2);}
  .police-btn.active{background:linear-gradient(135deg,rgba(0,60,255,.25),rgba(200,0,0,.25));border-color:#6666ff;color:#fff;box-shadow:0 0 20px rgba(100,100,255,.3),0 0 40px rgba(200,0,0,.2);animation:policeGlow 0.16s infinite alternate;}
  @keyframes policeGlow{from{box-shadow:0 0 20px rgba(0,60,255,.5),0 0 40px rgba(0,60,255,.2);}to{box-shadow:0 0 20px rgba(200,0,0,.5),0 0 40px rgba(200,0,0,.2);}}
  .police-light{width:10px;height:10px;border-radius:50%;animation:policeDot 0.16s infinite alternate;}
  @keyframes policeDot{from{background:#3366ff;box-shadow:0 0 8px #3366ff;}to{background:#ff2200;box-shadow:0 0 8px #ff2200;}}

  /* BREATHING MODE BUTTON */
  .breathe-btn{width:100%;padding:16px;border:none;border-radius:10px;font-size:14px;font-weight:800;letter-spacing:3px;text-transform:uppercase;cursor:pointer;transition:all .4s;margin-bottom:10px;display:flex;align-items:center;justify-content:center;gap:10px;background:var(--panel);color:var(--text2);border:1px solid var(--border2);}
  .breathe-btn.active{border-color:rgba(46,204,113,.5);color:var(--green);animation:breathePulse 3s ease-in-out infinite;}
  @keyframes breathePulse{0%,100%{background:rgba(46,204,113,.04);box-shadow:0 0 8px rgba(46,204,113,.1);}50%{background:rgba(46,204,113,.12);box-shadow:0 0 24px rgba(46,204,113,.3);}}

  /* PIN MODAL */
  .pin-display{font-size:32px;font-weight:800;letter-spacing:8px;color:var(--white);text-align:center;padding:14px;background:var(--bg3);border-radius:10px;border:1px solid var(--border2);margin-bottom:16px;min-height:58px;}
  .pin-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-bottom:8px;}
  .pin-btn{padding:16px;border:none;border-radius:9px;background:var(--bg3);border:1px solid var(--border2);font-size:20px;font-weight:800;color:var(--white);cursor:pointer;transition:all .15s;user-select:none;}
  .pin-btn:active{background:var(--border2);transform:scale(.93);}
  .pin-err{color:var(--accent2);font-size:12px;font-weight:700;text-align:center;margin-top:6px;min-height:18px;letter-spacing:1px;}
  .zone-toggle-panel{background:var(--panel);border:1px solid var(--border);border-radius:10px;padding:12px 14px;margin-bottom:14px;}
  .zone-toggle-hdr{font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--text2);margin-bottom:10px;display:flex;align-items:center;justify-content:space-between;}
  .zone-all-btns{display:flex;gap:7px;}
  .zone-all-btn{padding:5px 12px;border-radius:6px;border:1px solid var(--border2);background:var(--bg3);font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--text2);cursor:pointer;transition:all .15s;}
  .zone-all-btn:active{transform:scale(.95);}
  .zone-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:7px;}
  .ztog{display:flex;align-items:center;justify-content:space-between;background:var(--bg3);border:1px solid var(--border);border-radius:8px;padding:9px 11px;cursor:pointer;user-select:none;transition:all .2s;}
  .ztog.on{border-color:rgba(232,49,42,.4);background:rgba(232,49,42,.06);}
  .ztog-info{display:flex;align-items:center;gap:8px;}
  .ztog-swatch{width:10px;height:10px;border-radius:3px;flex-shrink:0;}
  .ztog-name{font-size:11px;font-weight:700;color:var(--text);line-height:1.2;}
  .ztog-sub{font-size:9px;color:var(--text3);font-weight:600;letter-spacing:.5px;}
  .ztog-sw{width:32px;height:18px;border-radius:9px;background:var(--bg);border:1px solid var(--border2);position:relative;flex-shrink:0;transition:all .2s;}
  .ztog-sw::after{content:'';position:absolute;width:12px;height:12px;border-radius:50%;background:var(--text3);top:2px;left:2px;transition:all .2s;}
  .ztog.on .ztog-sw{background:rgba(232,49,42,.2);border-color:var(--accent);}
  .ztog.on .ztog-sw::after{left:16px;background:var(--accent);}

  .savebar{position:sticky;bottom:0;background:var(--bg2);border-top:1px solid var(--border);padding:12px 14px;display:flex;gap:10px;z-index:90;}
  .btn{flex:1;padding:14px;border:none;border-radius:9px;font-size:13px;font-weight:800;letter-spacing:2px;text-transform:uppercase;cursor:pointer;transition:all .15s;}
  .btnp{background:var(--accent);color:#fff;}
  .btnp:active{transform:scale(.97);}
  .btns{background:var(--bg3);color:var(--text);border:1px solid var(--border2);}
  .toast{position:fixed;bottom:80px;left:50%;transform:translateX(-50%) translateY(16px);background:var(--bg3);border:1px solid var(--border2);border-radius:9px;padding:10px 22px;font-size:13px;font-weight:700;letter-spacing:1px;opacity:0;transition:all .3s;z-index:200;white-space:nowrap;pointer-events:none;}
  .toast.show{opacity:1;transform:translateX(-50%) translateY(0);}
  .toast.ok{border-color:var(--green);color:var(--green);}
  .toast.err{border-color:var(--accent);color:var(--accent2);}
  .overlay{position:fixed;inset:0;background:rgba(0,0,0,.85);z-index:300;display:flex;align-items:center;justify-content:center;padding:20px;}
  .modal{background:var(--bg2);border:1px solid var(--border2);border-radius:14px;padding:26px;width:100%;max-width:360px;}
  .mtitle{font-size:18px;font-weight:800;letter-spacing:2px;color:var(--white);margin-bottom:6px;}
  .msub{font-size:12px;color:var(--text2);margin-bottom:20px;line-height:1.6;}
  .msub strong{color:var(--accent);}
  .minput{width:100%;background:var(--bg3);border:1px solid var(--border2);border-radius:9px;padding:13px 14px;font-size:15px;font-weight:700;color:var(--white);outline:none;margin-bottom:16px;letter-spacing:1px;}
  .minput:focus{border-color:var(--accent);}
  .mbtns{display:flex;gap:10px;}
  .spacer{height:80px;}
</style>
</head>
<body>

<header>
  <div class="logo">UNDER<span>GLOW</span></div>
  <div class="conn-badge" onclick="showModal()">
    <div class="dot" id="dot"></div>
    <span id="connLbl">OFFLINE</span>
  </div>
</header>

<div class="tabs">
  <div class="tab active" onclick="switchTab('status')">&#9711;&nbsp; STATUS</div>
  <div class="tab" onclick="switchTab('config')">&#9881;&nbsp; CONFIG</div>
</div>

<!-- STATUS -->
<div class="page active" id="tab-status">
  <div class="slave-panel">
    <div class="slave-hdr">Slave Controllers</div>
    <div class="slave-row" id="slaveRow"></div>
  </div>

  <div class="sgrid">
    <div class="scard" id="c-ignition"><div class="sicon">&#128273;</div><div class="slbl">Ignition</div></div>
    <div class="scard" id="c-running_lights"><div class="sicon">&#128161;</div><div class="slbl">Running</div></div>
    <div class="scard" id="c-brake"><div class="sicon">&#9940;</div><div class="slbl">Brake</div></div>
    <div class="scard" id="c-left_turn"><div class="sicon">&#9668;</div><div class="slbl">Left Turn</div></div>
    <div class="scard" id="c-right_turn"><div class="sicon">&#9658;</div><div class="slbl">Right Turn</div></div>
    <div class="scard" id="c-reverse"><div class="sicon">&#8592;</div><div class="slbl">Reverse</div></div>
    <div class="scard" id="c-driver_door"><div class="sicon">&#128682;</div><div class="slbl">Driver Door</div></div>
    <div class="scard" id="c-passenger_door"><div class="sicon">&#128682;</div><div class="slbl">Pass Door</div></div>
    <div class="scard" id="c-safe_drive"><div class="sicon">&#128737;</div><div class="slbl">Safe Drive</div></div>
  </div>

  <div class="lpanel">
    <div class="lhdr">
      <div class="seclbl">Ambient Light</div>
      <div class="dnbadge" id="dnbadge">--</div>
    </div>
    <div class="ltrack"><div class="lfill" id="lfill"></div></div>
    <div class="lval" id="lval">-- / 4095</div>
  </div>
  <div class="ticker" id="ticker">CONNECT TO BEGIN</div>

  <!-- Breathing Mode -->
  <button class="breathe-btn" id="breatheBtn" onclick="toggleBreathe()">
    <span id="breatheBtnText">🌿 BREATHING MODE</span>
  </button>

  <!-- Police Mode -->
  <button class="police-btn" id="policeBtn" onclick="onPoliceTap()">
    <span id="policeBtnLight" style="display:none" class="police-light"></span>
    <span id="policeBtnText">🟢 POLICE MODE</span>
  </button>

  <!-- Zone Toggles -->
  <div class="zone-toggle-panel">
    <div class="zone-toggle-hdr">
      Zone Controls
      <div class="zone-all-btns">
        <div class="zone-all-btn" onclick="allZones(true)">ALL ON</div>
        <div class="zone-all-btn" onclick="allZones(false)">ALL OFF</div>
      </div>
    </div>
    <div class="zone-grid" id="zoneToggles"></div>
  </div>
</div>

<!-- CONFIG -->
<div class="page" id="tab-config">
  <div class="unsaved" id="unsavedBanner">
    <span>&#9679; Unsaved changes</span>
    <span style="font-size:10px;opacity:.7">Press SAVE TO CAR to apply</span>
  </div>

  <div class="sechdr">Global Options</div>
  <div class="ggrid">
    <div class="togcard" id="gc-safe" onclick="toggleG('safe')">
      <div><div class="togname">Safe Drive</div><div class="togdesc">Dim at speed</div></div>
      <div class="sw" id="gs-safe"></div>
    </div>
    <div class="togcard" id="gc-dassist" onclick="toggleG('dassist')">
      <div><div class="togname">Door Assist</div><div class="togdesc">Light on open</div></div>
      <div class="sw" id="gs-dassist"></div>
    </div>
    <div class="togcard" id="gc-seqturn" onclick="toggleG('seqturn')">
      <div><div class="togname">Seq Turn</div><div class="togdesc">Sequential signal</div></div>
      <div class="sw" id="gs-seqturn"></div>
    </div>
    <div class="togcard" id="gc-dynstart" onclick="toggleG('dynstart')">
      <div><div class="togname">Dyn Startup</div><div class="togdesc">Animated start</div></div>
      <div class="sw" id="gs-dynstart"></div>
    </div>
    <div class="togcard" id="gc-daytime" onclick="toggleG('daytime')" style="grid-column:span 2">
      <div><div class="togname">Daytime Mode</div><div class="togdesc">Enable lights during daytime</div></div>
      <div class="sw" id="gs-daytime"></div>
    </div>
  </div>

  <div class="sechdr">Zone Colors &amp; Options</div>

  <!-- Change All -->
  <div class="chgall-card" id="chgallCard">
    <div class="chgall-hdr" onclick="toggleChgAll()">
      <div>
        <div class="chgall-title">&#127752; Change All Zones</div>
        <div class="chgall-sub">Apply one color to multiple zones at once</div>
      </div>
      <div style="display:flex;align-items:center;gap:10px;">
        <div class="chgall-swatch" id="chgallSwatch" style="background:#1e2530"></div>
        <div class="chev2">&#9660;</div>
      </div>
    </div>
    <div class="chgall-body">
      <div class="slrow"><div class="sllbl">R</div><div class="slwrap"><input type="range" min="0" max="255" value="255" id="ca-r" oninput="updateCA('r',this.value)"></div><div class="slval" id="cv-r">255</div></div>
      <div class="slrow"><div class="sllbl">G</div><div class="slwrap"><input type="range" min="0" max="255" value="255" id="ca-g" oninput="updateCA('g',this.value)"></div><div class="slval" id="cv-g">255</div></div>
      <div class="slrow"><div class="sllbl">B</div><div class="slwrap"><input type="range" min="0" max="255" value="255" id="ca-b" oninput="updateCA('b',this.value)"></div><div class="slval" id="cv-b">255</div></div>
      <div class="slrow"><div class="sllbl">WW</div><div class="slwrap"><input type="range" min="0" max="255" value="0" id="ca-ww" oninput="updateCA('ww',this.value)"></div><div class="slval" id="cv-ww">0</div></div>
      <div class="slrow"><div class="sllbl">CW</div><div class="slwrap"><input type="range" min="0" max="255" value="0" id="ca-cw" oninput="updateCA('cw',this.value)"></div><div class="slval" id="cv-cw">0</div></div>
      <div style="font-size:10px;font-weight:700;letter-spacing:1.5px;color:var(--text2);margin-top:14px;margin-bottom:6px;">APPLY TO:</div>
      <div class="scope-row">
        <div class="scope-btn on" id="sc-all"       onclick="setScope('all')">All</div>
        <div class="scope-btn"    id="sc-underglow" onclick="setScope('underglow')">Underglow</div>
        <div class="scope-btn"    id="sc-interior"  onclick="setScope('interior')">Interior</div>
        <div class="scope-btn"    id="sc-grills"    onclick="setScope('grills')">Grills</div>
        <div class="scope-btn"    id="sc-louvers"   onclick="setScope('louvers')">Louvers</div>
      </div>
      <button class="chgall-apply" onclick="applyCA()">&#9654;&nbsp; APPLY TO SELECTED ZONES</button>
    </div>
  </div>

  <div id="zoneList"></div>
  <div class="spacer"></div>
</div>

<div class="savebar">
  <button class="btn btns" onclick="reloadConfig()">&#8635;&nbsp; RELOAD</button>
  <button class="btn btnp" onclick="pushAndSave()">&#9654;&nbsp; SAVE TO CAR</button>
</div>

<div class="toast" id="toast"></div>

<div class="overlay" id="modal">
  <div class="modal">
    <div class="mtitle">CONNECT</div>
    <div class="msub">Enter your ESP32 IP. Make sure you are on <strong>Camaro_Underglow</strong> WiFi first.</div>
    <input class="minput" id="ipIn" value="192.168.4.1" type="text" inputmode="decimal">
    <div class="mbtns">
      <button class="btn btns" style="flex:1" onclick="closeModal()">Cancel</button>
      <button class="btn btnp" style="flex:2" onclick="applyIp()">Connect</button>
    </div>
  </div>
</div>

<!-- PIN Modal for Police Mode -->
<div class="overlay" id="pinModal" style="display:none">
  <div class="modal">
    <div class="mtitle">POLICE MODE</div>
    <div class="msub">Enter PIN to activate.</div>
    <div class="pin-display" id="pinDisplay">&#8226;&#8226;&#8226;&#8226;</div>
    <div class="pin-grid">
      <button class="pin-btn" onclick="pinKey('1')">1</button>
      <button class="pin-btn" onclick="pinKey('2')">2</button>
      <button class="pin-btn" onclick="pinKey('3')">3</button>
      <button class="pin-btn" onclick="pinKey('4')">4</button>
      <button class="pin-btn" onclick="pinKey('5')">5</button>
      <button class="pin-btn" onclick="pinKey('6')">6</button>
      <button class="pin-btn" onclick="pinKey('7')">7</button>
      <button class="pin-btn" onclick="pinKey('8')">8</button>
      <button class="pin-btn" onclick="pinKey('9')">9</button>
      <button class="pin-btn" onclick="pinClear()" style="font-size:14px;color:var(--text2)">CLR</button>
      <button class="pin-btn" onclick="pinKey('0')">0</button>
      <button class="pin-btn" onclick="pinCancel()" style="font-size:14px;color:var(--text2)">✕</button>
    </div>
    <div class="pin-err" id="pinErr"></div>
  </div>
</div>

<script>
const ZNAMES = ['Driver Underglow','Rear Underglow','Passenger Underglow','Front Underglow',
  'Top Grill','Bottom Grill','Driver Louver','DS Footwell & Seat','Passenger Louver','PS Footwell & Seat'];

const SLAVE_INFO = [
  null, // index 0 unused
  {label:'S1', zones:'Drv\nUndrglow'},
  {label:'S2', zones:'Pas\nUndrglow'},
  {label:'S3', zones:'Grills'},
  {label:'S4', zones:'DS\nInterior'},
  {label:'S5', zones:'PS\nInterior'}
];

const SCOPE_ZONES = {
  all:       [0,1,2,3,4,5,6,7,8,9],
  underglow: [0,1,2,3],
  interior:  [7,9],
  grills:    [4,5],
  louvers:   [6,8]
};

let IP = localStorage.getItem('esp_ip') || '192.168.4.1';
let statusTimer = null, configTimer = null;
let cfg = null;
let hasUnsaved = false;
let activeScope = 'all';
let caVals = {r:255,g:255,b:255,ww:0,cw:0};

// ---- BUILD SLAVE PILLS ----
function initSlavePills() {
  const row = document.getElementById('slaveRow');
  row.innerHTML = '';
  for (let s = 1; s <= 5; s++) {
    const info = SLAVE_INFO[s];
    row.innerHTML += `
      <div class="slave-pill" id="slave-${s}">
        <div class="slave-num">${info.label}</div>
        <div class="slave-dot"></div>
        <div class="slave-zones">${info.zones}</div>
      </div>`;
  }
}

// Update slave pills from the slaves array in /status response
function updateSlavePills(slavesArr) {
  for (let s = 1; s <= 5; s++) {
    const pill = document.getElementById('slave-'+s);
    if (!pill) continue;
    // Explicitly check for true — anything else (false, 0, undefined, missing) = offline
    const online = Array.isArray(slavesArr) && slavesArr[s-1] === true;
    pill.className = 'slave-pill ' + (online ? 'online' : 'offline');
  }
}

// ---- TABS ----
function switchTab(t) {
  document.querySelectorAll('.tab').forEach((el,i)=>el.classList.toggle('active',['status','config'][i]===t));
  document.querySelectorAll('.page').forEach(el=>el.classList.remove('active'));
  document.getElementById('tab-'+t).classList.add('active');
}

// ---- CONNECTION ----
function setConn(ok) {
  document.getElementById('dot').className = 'dot '+(ok?'on':'err');
  document.getElementById('connLbl').textContent = ok?'LIVE':'ERROR';
  if (!ok) {
    // Mark all slaves offline when master is unreachable
    for (let s=1;s<=5;s++) {
      const p=document.getElementById('slave-'+s);
      if (p) p.className='slave-pill offline';
    }
  }
}

// ---- FETCH ----
async function apiFetch(path, opts={}, ms=3000) {
  const ac = new AbortController();
  const tid = setTimeout(()=>ac.abort(), ms);
  try {
    const r = await fetch('http://'+IP+path, {...opts, signal:ac.signal});
    clearTimeout(tid);
    if (!r.ok) throw new Error('HTTP '+r.status);
    return await r.json();
  } catch(e) { clearTimeout(tid); throw e; }
}

// ---- STATUS POLL ----
async function pollStatus() {
  try {
    const d = await apiFetch('/status');
    setConn(true);
    ['ignition','running_lights','brake','left_turn','right_turn',
     'reverse','driver_door','passenger_door','safe_drive']
      .forEach(k=>{ const c=document.getElementById('c-'+k); if(c) c.classList.toggle('on',!!d[k]); });
    const lv = d.light_level||0;
    document.getElementById('lfill').style.width = Math.min(100,(lv/4095)*100)+'%';
    document.getElementById('lval').textContent = lv+' / 4095';
    const b = document.getElementById('dnbadge');
    b.textContent = d.is_night?'NIGHT':'DAY';
    b.className = 'dnbadge '+(d.is_night?'night':'day');
    document.getElementById('ticker').textContent = 'UPDATED '+new Date().toLocaleTimeString();
    updateSlavePills(d.slaves);
    // Sync police mode button with board state
    if (d.police !== undefined && d.police !== policeOn) setPoliceUI(d.police === true);
    // Sync breathe mode button with board state
    if (d.breathe !== undefined && d.breathe !== breatheOn) setBreatheUI(d.breathe === true);
  } catch(e) {
    setConn(false);
    document.getElementById('ticker').textContent = 'NO RESPONSE FROM '+IP;
  }
}

// ---- CONFIG POLL ----
async function pollConfig() {
  if (hasUnsaved) return;
  try {
    const d = await apiFetch('/config',{},5000);
    cfg = JSON.parse(JSON.stringify(d));
    renderCfg();
    updateZoneSwatches();
  } catch(e) {}
}

function startPolling() {
  if (statusTimer) clearInterval(statusTimer);
  if (configTimer) clearInterval(configTimer);
  pollStatus();
  pollConfig();
  statusTimer = setInterval(pollStatus, 500);
  configTimer = setInterval(pollConfig, 5000);
}

function updateZoneSwatches() {
  if (!cfg) return;
  for (let i = 0; i < 10; i++) {
    const sw = document.getElementById('ztog-sw-'+i);
    if (sw) sw.style.background = zColor(cfg.zones[i]);
  }
}

async function reloadConfig() {
  hasUnsaved = false; markUnsaved(false);
  try {
    const d = await apiFetch('/config',{},5000);
    cfg = JSON.parse(JSON.stringify(d));
    renderCfg();
    initZoneToggles();
    updateZoneSwatches();
    showToast('Reloaded from car','ok');
  } catch(e) { showToast('Failed to reload','err'); }
}

async function pushAndSave() {
  if (!cfg) { showToast('No config loaded','err'); return; }
  try {
    await apiFetch('/set',{method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify(cfg)},5000);
    await apiFetch('/save',{},4000);
    hasUnsaved = false; markUnsaved(false);
    showToast('Saved to car ✓','ok');
  } catch(e) { showToast('Save failed — check connection','err'); }
}

// ---- RENDER CONFIG ----
function renderCfg() {
  if (!cfg) return;
  const openZones = new Set();
  document.querySelectorAll('.zcard.open').forEach(el=>openZones.add(el.id));
  ['safe','dassist','seqturn','dynstart','daytime'].forEach(k=>{
    const on=!!cfg[k];
    document.getElementById('gs-'+k).className='sw'+(on?' on':'');
    document.getElementById('gc-'+k).classList.toggle('on',on);
  });
  const list=document.getElementById('zoneList');
  list.innerHTML='';
  cfg.zones.forEach((z,i)=>{
    const div=document.createElement('div');
    div.className='zcard'+(openZones.has('zc-'+i)?' open':'');
    div.id='zc-'+i;
    const c=zColor(z);
    div.innerHTML=`
      <div class="zhdr" onclick="toggleZ(${i})">
        <div class="zswatch" id="zsw-${i}" style="background:${c}"></div>
        <div><div class="zname">${ZNAMES[i]}</div><div class="zmeta">SLAVE ${z.slave} &bull; CH${z.channel} &bull; ${z.pixels}px</div></div>
        <div class="chev">&#9660;</div>
      </div>
      <div class="zbody">
        ${mksl(i,'r','R',z.r)}${mksl(i,'g','G',z.g)}${mksl(i,'b','B',z.b)}
        ${mksl(i,'ww','WW',z.ww)}${mksl(i,'cw','CW',z.cw)}
        <div class="clrprev">
          <div class="clrsw" id="clrsw-${i}" style="background:${c}"></div>
          <div class="clrvals" id="clrv-${i}">RGB(${z.r}, ${z.g}, ${z.b})<br>WW:${z.ww} &bull; CW:${z.cw}</div>
        </div>
        <div class="zopts">
          <div class="zopt${z.turn?' on':''}" id="zo-turn-${i}" onclick="toggleOpt(${i},'turn')">Turn</div>
          <div class="zopt${z.amber?' on':''}" id="zo-amber-${i}" onclick="toggleOpt(${i},'amber')">Amber</div>
          <div class="zopt${z.door?' on':''}" id="zo-door-${i}" onclick="toggleOpt(${i},'door')">Door</div>
        </div>
      </div>`;
    list.appendChild(div);
  });
}

function mksl(i,k,lbl,v) {
  return `<div class="slrow"><div class="sllbl">${lbl}</div><div class="slwrap">
    <input type="range" min="0" max="255" value="${v}" oninput="upColor(${i},'${k}',this.value)">
    </div><div class="slval" id="sv-${i}-${k}">${v}</div></div>`;
}

function zColor(z) {
  if (z.r===0&&z.g===0&&z.b===0&&(z.ww>0||z.cw>0))
    return `rgb(${Math.round(z.ww*.8+z.cw*.3)},${Math.round(z.ww*.65+z.cw*.3)},${Math.round(z.cw*.9)})`;
  if (z.r===0&&z.g===0&&z.b===0) return '#1e2530';
  return `rgb(${z.r},${z.g},${z.b})`;
}

function markUnsaved(v) {
  hasUnsaved=v;
  document.getElementById('unsavedBanner').classList.toggle('show',v);
}

function toggleZ(i) { document.getElementById('zc-'+i).classList.toggle('open'); }

function toggleG(k) {
  if (!cfg) return;
  cfg[k]=cfg[k]?0:1;
  const on=!!cfg[k];
  document.getElementById('gs-'+k).className='sw'+(on?' on':'');
  document.getElementById('gc-'+k).classList.toggle('on',on);
  markUnsaved(true);
}

function toggleOpt(i,k) {
  if (!cfg) return;
  cfg.zones[i][k]=cfg.zones[i][k]?0:1;
  document.getElementById('zo-'+k+'-'+i).classList.toggle('on',!!cfg.zones[i][k]);
  markUnsaved(true);
}

function upColor(i,k,v) {
  if (!cfg) return;
  cfg.zones[i][k]=parseInt(v);
  document.getElementById('sv-'+i+'-'+k).textContent=v;
  const z=cfg.zones[i], c=zColor(z);
  document.getElementById('zsw-'+i).style.background=c;
  document.getElementById('clrsw-'+i).style.background=c;
  document.getElementById('clrv-'+i).innerHTML=`RGB(${z.r}, ${z.g}, ${z.b})<br>WW:${z.ww} &bull; CW:${z.cw}`;
  markUnsaved(true);
}

// ---- CHANGE ALL ----
function toggleChgAll() { document.getElementById('chgallCard').classList.toggle('open'); }

function updateCA(k,v) {
  caVals[k]=parseInt(v);
  document.getElementById('cv-'+k).textContent=v;
  document.getElementById('chgallSwatch').style.background=zColor({r:caVals.r,g:caVals.g,b:caVals.b,ww:caVals.ww,cw:caVals.cw});
}

function setScope(s) {
  activeScope=s;
  document.querySelectorAll('.scope-btn').forEach(el=>el.classList.remove('on'));
  document.getElementById('sc-'+s).classList.add('on');
}

function applyCA() {
  if (!cfg) { showToast('Load config first','err'); return; }
  (SCOPE_ZONES[activeScope]||SCOPE_ZONES.all).forEach(i=>{
    cfg.zones[i].r=caVals.r; cfg.zones[i].g=caVals.g; cfg.zones[i].b=caVals.b;
    cfg.zones[i].ww=caVals.ww; cfg.zones[i].cw=caVals.cw;
    const c=zColor(cfg.zones[i]);
    const sw=document.getElementById('zsw-'+i);
    const cs=document.getElementById('clrsw-'+i);
    const cv=document.getElementById('clrv-'+i);
    if(sw) sw.style.background=c;
    if(cs) cs.style.background=c;
    if(cv) cv.innerHTML=`RGB(${caVals.r}, ${caVals.g}, ${caVals.b})<br>WW:${caVals.ww} &bull; CW:${caVals.cw}`;
    ['r','g','b','ww','cw'].forEach(k=>{
      const sv=document.getElementById('sv-'+i+'-'+k);
      if(sv) sv.textContent=caVals[k];
      const inp=document.querySelector(`#zc-${i} .zbody input[oninput*="'${k}'"]`);
      if(inp) inp.value=caVals[k];
    });
  });
  markUnsaved(true);
  const names={all:'all zones',underglow:'underglow',interior:'interior',grills:'grills',louvers:'louvers'};
  showToast('Applied to '+names[activeScope],'ok');
}

// ---- MODAL ----
function showModal() { document.getElementById('ipIn').value=IP; document.getElementById('modal').style.display='flex'; }
function closeModal() { document.getElementById('modal').style.display='none'; }
function applyIp() {
  const v=document.getElementById('ipIn').value.trim();
  if(v){IP=v;localStorage.setItem('esp_ip',v);}
  closeModal(); startPolling(); reloadConfig();
}

function showToast(msg,type) {
  const t=document.getElementById('toast');
  t.textContent=msg; t.className='toast show '+type;
  setTimeout(()=>t.className='toast',2500);
}

// ---- POLICE MODE ----
let policeOn = false;
const POLICE_PIN = '1312'; // change this to whatever PIN you want
let pinEntry = '';

function setPoliceUI(on) {
  policeOn = on;
  const btn  = document.getElementById('policeBtn');
  const light = document.getElementById('policeBtnLight');
  const txt   = document.getElementById('policeBtnText');
  btn.className = 'police-btn' + (on ? ' active' : '');
  light.style.display = on ? 'inline-block' : 'none';
  txt.innerHTML = on ? '🚨 POLICE MODE ACTIVE — TAP TO STOP' : '🟢 POLICE MODE';
}

function onPoliceTap() {
  if (policeOn) {
    // No PIN needed to turn off
    togglePolice(false);
  } else {
    // Show PIN modal
    pinEntry = '';
    document.getElementById('pinDisplay').innerHTML = '&bull;&bull;&bull;&bull;';
    document.getElementById('pinErr').textContent = '';
    document.getElementById('pinModal').style.display = 'flex';
  }
}

function pinKey(k) {
  if (pinEntry.length >= 8) return;
  pinEntry += k;
  document.getElementById('pinDisplay').textContent = '•'.repeat(pinEntry.length);
  document.getElementById('pinErr').textContent = '';
  // Auto-submit when enough digits entered
  if (pinEntry.length === POLICE_PIN.length) {
    setTimeout(pinSubmit, 120);
  }
}

function pinClear() {
  pinEntry = '';
  document.getElementById('pinDisplay').innerHTML = '&bull;&bull;&bull;&bull;';
  document.getElementById('pinErr').textContent = '';
}

function pinCancel() {
  document.getElementById('pinModal').style.display = 'none';
  pinEntry = '';
}

function pinSubmit() {
  if (pinEntry === POLICE_PIN) {
    document.getElementById('pinModal').style.display = 'none';
    pinEntry = '';
    togglePolice(true);
  } else {
    document.getElementById('pinErr').textContent = 'INCORRECT PIN';
    document.getElementById('pinDisplay').innerHTML = '&bull;&bull;&bull;&bull;';
    pinEntry = '';
    // Shake animation
    const d = document.getElementById('pinDisplay');
    d.style.borderColor = 'var(--accent)';
    setTimeout(()=>d.style.borderColor='', 600);
  }
}

async function togglePolice(on) {
  // Also turn off breathing if activating police
  if (on && breatheOn) toggleBreathe();
  try {
    await apiFetch('/police?state='+(on?'on':'off'), {}, 3000);
    setPoliceUI(on);
    showToast(on ? 'Police mode ON' : 'Police mode OFF', 'ok');
  } catch(e) {
    showToast('Failed to toggle police mode','err');
  }
}

// ---- BREATHING MODE ----
let breatheOn = false;

function setBreatheUI(on) {
  breatheOn = on;
  const btn = document.getElementById('breatheBtn');
  const txt = document.getElementById('breatheBtnText');
  btn.className = 'breathe-btn' + (on ? ' active' : '');
  txt.innerHTML = on ? '🌿 BREATHING — TAP TO STOP' : '🌿 BREATHING MODE';
}

async function toggleBreathe() {
  const next = !breatheOn;
  // Turn off police if breathing activated
  if (next && policeOn) togglePolice(false);
  try {
    await apiFetch('/breathe?state='+(next?'on':'off'), {}, 3000);
    setBreatheUI(next);
    showToast(next ? 'Breathing mode ON' : 'Breathing mode OFF', 'ok');
  } catch(e) {
    showToast('Failed to toggle breathing','err');
  }
}

// ---- ZONE TOGGLES ----
const ZONE_STATE = new Array(10).fill(true); // local on/off state
const ZONE_SHORT = ['Drv UG','Rear UG','Pas UG','Frnt UG','Top Grill','Bot Grill','Drv Louver','DS Ftwell','Pas Louver','PS Ftwell'];
const ZONE_GROUPS = ['Underglow','Underglow','Underglow','Underglow','Grill','Grill','Louver','Interior','Louver','Interior'];

function initZoneToggles() {
  const grid = document.getElementById('zoneToggles');
  if (!grid) return;
  grid.innerHTML = '';
  for (let i = 0; i < 10; i++) {
    const on = ZONE_STATE[i];
    const color = cfg ? zColor(cfg.zones[i]) : '#1e2530';
    grid.innerHTML += `
      <div class="ztog ${on?'on':''}" id="ztog-${i}" onclick="toggleZone(${i})">
        <div class="ztog-info">
          <div class="ztog-swatch" id="ztog-sw-${i}" style="background:${color}"></div>
          <div><div class="ztog-name">${ZONE_SHORT[i]}</div><div class="ztog-sub">${ZONE_GROUPS[i]}</div></div>
        </div>
        <div class="ztog-sw"></div>
      </div>`;
  }
}

async function toggleZone(i) {
  const next = !ZONE_STATE[i];
  ZONE_STATE[i] = next;
  const el = document.getElementById('ztog-'+i);
  if (el) el.className = 'ztog' + (next?' on':'');
  try {
    await apiFetch(`/zone?z=${i}&state=${next?'on':'off'}`, {}, 2000);
  } catch(e) {
    showToast('Zone toggle failed','err');
    // Revert
    ZONE_STATE[i] = !next;
    if (el) el.className = 'ztog' + (!next?' on':'');
  }
}

async function allZones(on) {
  for (let i = 0; i < 10; i++) {
    ZONE_STATE[i] = on;
    const el = document.getElementById('ztog-'+i);
    if (el) el.className = 'ztog' + (on?' on':'');
  }
  try {
    // Fire all 10 in parallel
    await Promise.all([...Array(10).keys()].map(i =>
      apiFetch(`/zone?z=${i}&state=${on?'on':'off'}`, {}, 2000)
    ));
    showToast(on ? 'All zones ON' : 'All zones OFF', 'ok');
  } catch(e) {
    showToast('Some zones failed','err');
  }
}

document.addEventListener('DOMContentLoaded',()=>{
  initSlavePills();
  initZoneToggles();
  if (localStorage.getItem('esp_ip')) {
    document.getElementById('modal').style.display='none';
    startPolling(); reloadConfig();
  }
});
</script>
</body>
</html>
