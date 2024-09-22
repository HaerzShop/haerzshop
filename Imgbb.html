<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Upload Gambar ke ImgBB</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f0f2f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            position: relative;
            background-color: #fff;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            text-align: center;
            max-width: 450px;
            width: 100%;
            border: 2px solid #007bff;
        }
        h1 {
            font-size: 26px;
            margin-bottom: 25px;
            color: #333;
            border-bottom: 2px solid #007bff;
            padding-bottom: 10px;
        }
        input[type="file"] {
            display: none;
        }
        label {
            background-color: #007bff;
            color: white;
            padding: 12px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s ease;
            border: 2px solid #0056b3;
        }
        label:hover {
            background-color: #0056b3;
        }
        #uploadBtn {
            margin-top: 20px;
            background-color: #28a745;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s ease;
            border: 2px solid #218838;
        }
        #uploadBtn:hover {
            background-color: #218838;
        }
        #overlay {
            display: none;
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(255, 255, 255, 0.8);
            justify-content: center;
            align-items: center;
            border-radius: 12px;
        }
        #overlay img {
            width: 50px;
        }
        #result {
            margin-top: 30px;
            padding: 20px;
            border-radius: 10px;
            border: 2px solid #ccc;
            background-color: #f9f9f9;
        }
        #result img {
            margin-top: 20px;
            max-width: 100%;
            border-radius: 8px;
            border: 2px solid #ddd;
        }
        .error {
            color: red;
            margin-top: 10px;
            font-weight: bold;
        }
        #copyBtn {
            background-color: #007bff;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 14px;
            transition: background-color 0.3s ease;
            margin-top: 10px;
            border: 2px solid #0056b3;
        }
        #copyBtn:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Upload Gambar ke ImgBB</h1>
        <input type="file" id="fileInput" accept="image/*">
        <label for="fileInput">Pilih Gambar</label>
        <button id="uploadBtn" onclick="uploadImage()">Upload</button>
        <div id="overlay">
            <img src="https://i.imgur.com/llF5iyg.gif" alt="Loading">
        </div>
        <div id="result"></div>
    </div>

    <script>
        async function uploadImage() {
            const fileInput = document.getElementById('fileInput');
            const file = fileInput.files[0];
            const formData = new FormData();
            formData.append("image", file);

            const overlay = document.getElementById('overlay');
            overlay.style.display = 'flex';

            try {
                const response = await fetch("https://api.imgbb.com/1/upload?key=d3d6c684e0d03873aedcf2a0e88ea57a", {
                    method: "POST",
                    body: formData
                });
                const result = await response.json();
                overlay.style.display = 'none';
                console.log(result); // Menampilkan hasil di konsol
                if (result.success) {
                    const uploadedUrl = result.data.url;
                    document.getElementById('result').innerHTML = `
                        <h2>Upload Sukses! Terimakasih Telah Pakai Website By Haerzz</h2>
                        <p>URL Gambar: <a href="${uploadedUrl}" target="_blank">${uploadedUrl}</a></p>
                        <img src="${uploadedUrl}" alt="Uploaded Image">
                        <button id="copyBtn" onclick="copyToClipboard()">Salin URL Gambar</button>
                    `;
                } else {
                    document.getElementById('result').innerHTML = `<p class="error">Upload gagal. Silakan coba lagi.</p>`;
                }
            } catch (error) {
                overlay.style.display = 'none';
                console.error("Error uploading image:", error);
                document.getElementById('result').innerHTML = `<p class="error">Terjadi kesalahan. Silakan coba lagi.</p>`;
            }
        }

        function copyToClipboard() {
            const uploadedUrl = document.querySelector('#result a').href;
            navigator.clipboard.writeText(uploadedUrl).then(() => {
                alert('URL Gambar berhasil disalin ke clipboard!');
            }).catch(err => {
                console.error('Gagal menyalin URL:', err);
            });
        }
    </script>
</body>
</html>
