<!DOCTYPE html>
<html>
<head>
    <title>Will You Be My Valentine?</title>
    <style>
        body { text-align: center; font-family: Arial, sans-serif; padding: 50px; }
        .heart { color: red; font-size: 50px; }
    </style>
</head>
<body>
    <h1>Will You Be My Valentine, <span id="name"></span>? ❤️</h1>
    <button onclick="alert('Yay! Love you! ❤️')">Yes</button>
    <button onclick="alert('Oh no! 😢')">No</button>

    <script>
        // Get name from URL
        const params = new URLSearchParams(window.location.search);
        const name = params.get('name') || 'Love';
        document.getElementById('name').textContent = name;
    </script>
</body>
</html>
