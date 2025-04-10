# 10Englishsaimhospital
Doctor-Patient Dialogue Simulation
<!DOCTYPE html>
<html>
<head>
  <title>Doctor & Patient Dialogue</title>
  <style>
    .popup {
      display: none;
      position: fixed;
      background-color: white;
      padding: 20px;
      border: 2px solid #333;
      box-shadow: 0 0 10px rgba(0,0,0,0.3);
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 1000;
    }

    .overlay {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.5);
      z-index: 999;
    }

    .close-btn {
      margin-top: 10px;
      cursor: pointer;
      background-color: #f44336;
      color: white;
      border: none;
      padding: 5px 10px;
    }
  </style>
</head>
<body>

<h2>Click below to view the dialogue</h2>
<button onclick="openPopup()">Open Doctor-Patient Dialogue</button>

<div class="overlay" id="overlay" onclick="closePopup()"></div>

<div class="popup" id="popup">
  <h3>Doctor-Patient Dialogue</h3>
  <p><strong>Doctor:</strong> Good morning. What’s wrong?</p>
  <p><strong>Patient:</strong> I have a headache and a fever.</p>
  <p><strong>Doctor:</strong> Let me check your temperature.</p>
  <p><strong>Patient:</strong> Okay, thank you.</p>
  <button class="close-btn" onclick="closePopup()">Close</button>
</div>

<script>
  function openPopup() {
    document.getElementById("popup").style.display = "block";
    document.getElementById("overlay").style.display = "block";
  }

  function closePopup() {
    document.getElementById("popup").style.display = "none";
    document.getElementById("overlay").style.display = "none";
  }
</script>

</body>
</html>
