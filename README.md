# LOML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

<div id="custom-content">
    <div class="centered-text">
        <p>Click to open</p>
        <div class="arrow-down"></div>
    </div>
    <div class="envelope" id="envelope">
        <img src="envelope-icon.png" alt="Envelope">
    </div>
</div>

<div id="popup" style="display:none;">
    <div class="popup-content">
        <p>MALIK FASIH UR REHMAN LOVES YOU</p>
    </div>
</div>

<script src="script.js"></script>
</body>
</html>

body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}

#custom-content {
    position: relative;
    text-align: center;
    margin-top: 200px; /* Adjust as needed */
}

.centered-text {
    position: relative;
}

.arrow-down {
    width: 0;
    height: 0;
    border-left: 10px solid transparent;
    border-right: 10px solid transparent;
    border-top: 15px solid #000;
    margin: 10px auto;
}

.envelope {
    margin-top: 20px;
    cursor: pointer;
}

#popup {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.7);
    display: flex;
    justify-content: center;
    align-items: center;
}

.popup-content {
    background-color: #fff;
    padding: 20px;
    border-radius: 5px;
}

document.addEventListener('DOMContentLoaded', function() {
    document.getElementById('envelope').addEventListener('click', function() {
        document.getElementById('popup').style.display = 'flex';
    });
});

