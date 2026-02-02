<html>
<head>
  <title>Polling Status</title>
  <style>
    *{
        box-sizing:border-box;
    }
    body{
        margin:0;
        padding:40px;
        font-family:system-ui,-apple-system,"Calibri",sans-serif;
        background:#f4f6f8;
        color:#1f2933;
    }
    .poll-wrapper{
        max-width:720px;
        margin:auto;
        background:#ffffff;
        padding:26px;
        border-radius:10px;
        box-shadow:0 10px 25px rgba(0,0,0,0.08);
        border-top:6px solid #1A3263;
        position: relative;
    }
    h2{
        margin:0 0 18px;
        font-size:1.25rem;
        text-align:center;
        color:#1A3263;
        font-weight:700;
    }
    .to-win-label{
        text-align:center;
        font-weight:600;
        color:#1A3263;
        font-size:0.85rem;
        margin-bottom:6px;
        user-select:none;
    }
    .poll-bar{
        position: relative;
        display:flex;
        height:36px;
        border-radius:6px;
        overflow:hidden;
        background:#e5e7eb;
    }
    .segment{
	height:100%;
    }
    .republican{
        background:#E11D2E;
    }
    .democrat{
        background:#1D4ED8;
    }
    .other {
        background:#9CA3AF;
    }
    .labels{
        margin-top:16px;
        display:flex;
        justify-content:space-between;
        font-size:0.9rem;
    }
    .label{
        display:flex;
        align-items:center;
        gap:8px;
        color:#374151;
    }
    .dot{
        width:10px;
        height:10px;
        border-radius:50%;
    }
    .dot.republican{background:#E11D2E;}
    .dot.democrat{background:#1D4ED8;}
    .dot.other{background:#9CA3AF;}
    .meta{
        margin-top:14px;
        font-size:0.8rem;
        color:#6b7280;
        display:flex;
        justify-content:space-between;
    }
    .win-line {
        position:absolute;
        top:0;
        width:0;
        height: 36px;
        border-left:2px dotted #1A3263;
        left:56.25%; 
    }
  </style>
</head>
<body>
  <div class="poll-wrapper">
    <h2>Live Election Status</h2>
    <div class="to-win-label">To Win</div>
    <div class="poll-bar">
      <div class="segment republican" style="width:47%"></div>
      <div class="segment democrat" style="width:40%"></div>
      <div class="segment other" style="width:13%"></div>
      <div class="win-line" style="left:56.25%;"></div>
    </div>
    <div class="labels">
      <div class="label">
        <span class="dot republican"></span>
        <span>Republicans—47%</span>
      </div>
      <div class="label">
        <span class="dot democrat"></span>
        <span>Democrats—40%</span>
      </div>
      <div class="label">
        <span class="dot other"></span>
        <span>Others—13%</span>
      </div>
    </div>
    <div class="meta">
      <span>Votes counted: 69%</span>
      <span>Ongoing count</span>
    </div>
  </div>
</body>
</html>





