# Aurimas.github.io
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Will You Be My Valentine?</title>
<style>
    body {
        font-family: 'Arial', sans-serif;
        text-align: center;
        background-color: #ffe6eb;
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    h1 {
        color: #d6336c;
        font-size: 2.5rem;
    }
    button {
        padding: 12px 25px;
        font-size: 1.2rem;
        border: none;
        border-radius: 8px;
        cursor: pointer;
        margin: 10px;
        transition: 0.3s;
    }
    #yesBtn {
        background-color: #ff4d6d;
        color: white;
    }
    #noBtn {
        background-color: #ccc;
        position: absolute;
    }
</style>
</head>
<body>

<h1>Will you be my Valentine? ❤️</h1>
<div>
    <button id="yesBtn">Yes</button>
    <button id="noBtn">No</button>
</div>

<script>
    const noBtn = document.getElementById('noBtn');
    const yesBtn = document.getElementById('yesBtn');

    noBtn.addEventListener('mouseover', () => {
        const x = Math.random() * (window.innerWidth - noBtn.clientWidth);
        const y = Math.random() * (window.innerHeight - noBtn.clientHeight);
        noBtn.style.left = `${x}px`;
        noBtn.style.top = `${y}px`;
    });

    yesBtn.addEventListener('click', () => {
        document.body.innerHTML = "<h1>Yay! ❤️ You made me the happiest!</h1>";
        document.body.style.backgroundColor = "#ffccd5";
    });
</script>

</body>
</html>
