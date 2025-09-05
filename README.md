<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aimlock Control</title>
  <style>
    body { display:flex; flex-direction:column; justify-content:center; align-items:center;
           height:100vh; margin:0; background:#111; color:#fff; font-family:sans-serif; }
    button { margin:15px; padding:15px 25px; font-size:18px; border:none; border-radius:8px; cursor:pointer; }
    #aimlockBtn { background:#ff4444; color:#fff; }
    #runBtn { background:#44aa44; color:#fff; }
  </style>
</head>
<body>
  <button id="aimlockBtn">🔘 Aimlock: OFF</button>
  <button id="runBtn">🚀 Chạy Lệnh</button>

  <script>
    let aimlockOn = false;
    document.getElementById("aimlockBtn").onclick = function(){
      aimlockOn = !aimlockOn;
      this.textContent = "🔘 Aimlock: " + (aimlockOn ? "ON" : "OFF");
      alert("Aimlock " + (aimlockOn ? "Đã Bật" : "Đã Tắt"));
    };
    document.getElementById("runBtn").onclick = function(){
      // Không làm gì hết khi bấm
    };
  </script>
</body>
</html>
