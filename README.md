# Multiple-Shade-Selector
<!DOCTYPE html>
<html>
<head>
    <title> Shade Selector</title>
</head>
<body>
    <h2>Shade Selection</h2>
    <label>Incisal Shade: <input type="text" id="incisal"></label><br>
    <label>Body/Mid Shade: <input type="text" id="body"></label><br>
    <label>Gingival Shade: <input type="text" id="gingival"></label><br>
    <button onclick="getIncisalShade()">Submit</button>
    <p>Selected Shade: <span id="output"></span></p>

    <script>
        function getIncisalShade() {
            let incisalShade = document.getElementById("incisal").value;
            
            // Output only the incisal shade
            document.getElementById("output").innerText = incisalShade || "No incisal shade entered";
        }
    </script>
</body>
</html>
