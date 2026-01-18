# district-admin-review
<!DOCTYPE html>
<html>
<head>
  <title>District Administration Review</title>
  <style>
    body { font-family: Arial; background:#f4f6f8; }
    .box {
      background:white;
      width:360px;
      margin:100px auto;
      padding:25px;
      box-shadow:0 0 10px rgba(0,0,0,.1);
    }
    button { width:100%; padding:10px; }
  </style>
</head>
<body>

<div class="box" id="login">
  <h3>District Administration Review</h3>
  <p>Please sign in to acknowledge receipt.</p>
  <input placeholder="School Email"><br><br>
  <input type="password" placeholder="Password"><br><br>
  <button onclick="gotya()">Sign In</button>
</div>

<div class="box" id="gotya" style="display:none; background:#111; color:#0f0;">
  <h1>Got ya 👀</h1>
  <p>No data was saved. Nothing was sent.</p>
  <p>If this were real phishing:</p>
  <ul>
    <li>Your login would be stolen</li>
    <li>Your email could be compromised</li>
    <li>Same password = multiple accounts owned</li>
  </ul>
  <strong>This is how easy phishing works.</strong>
</div>

<script>
function gotya() {
  document.getElementById("login").style.display = "none";
  document.getElementById("gotya").style.display = "block";
}
</script>

</body>
</html>
