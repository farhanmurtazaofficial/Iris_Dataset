<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>File Converter and Compressor</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Document and Image Converter & Compressor</h1>
        <div class="upload-section">
            <form id="upload-form" action="/convert" method="POST" enctype="multipart/form-data">
                <div class="input-group">
                    <label for="file">Upload File:</label>
                    <input type="file" id="file" name="file" required>
                </div>
                <div class="buttons">
                    <button type="submit">Convert</button>
                    <button type="button" onclick="compressImage()">Compress Image</button>
                </div>
            </form>
        </div>
        <div class="result">
            <p id="status"></p>
            <a id="download-link" href="#" style="display:none;" download>Download Converted File</a>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
