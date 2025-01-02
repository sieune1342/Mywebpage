
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Đăng nhập Gmail</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f1f3f4;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #333;
            margin-bottom: 20px;
        }
        .login-container {
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            width: 350px;
        }
        .login-container h2 {
            text-align: center;
            margin-bottom: 20px;
        }
        .input-group {
            margin-bottom: 15px;
        }
        .input-group label {
            display: block;
            font-size: 14px;
            color: #555;
        }
        .input-group input {
            width: 100%;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }
        .input-group input:focus {
            border-color: #4CAF50;
        }
        .login-button {
            width: 100%;
            padding: 10px;
            background-color: #4285f4;
            color: white;
            font-size: 16px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .login-button:hover {
            background-color: #357ae8;
        }
        .forgot-password {
            text-align: right;
            font-size: 14px;
            color: #4285f4;
            cursor: pointer;
        }
        .forgot-password:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!-- Logo Vui lòng đăng nhập bằng tài khoản Gmail hoặc Facebook! -->
    <div class="logo">Vui lòng đăng nhập bằng tài khoản Gmail hoặc FaceBook!</div>

    <div class="login-container">
        <h2>Đăng nhập vào tài khoản của bạn</h2>
        
        <div class="input-group">
            <label for="email">Email hoặc số điện thoại</label>
            <input type="text" id="email" placeholder="Nhập email hoặc số điện thoại">
        </div>
        
        <div class="input-group">
            <label for="password">Mật khẩu</label>
            <input type="password" id="password" placeholder="Nhập mật khẩu">
        </div>
        
        <button class="login-button" onclick="handleLogin()">Đăng nhập</button>
        
        <div class="forgot-password">
            <a href="#">Quên mật khẩu?</a>
        </div>
    </div>

    <script>
        // Hàm xử lý đăng nhập khi nhấn nút
        function handleLogin() {
            const email = document.getElementById('email').value;
            const password = document.getElementById('password').value;

            // Xử lý đăng nhập, ví dụ: hiển thị thông báo hoặc gửi đến server
            alert(`Đăng nhập với Email/Số điện thoại: ${email}\nMật khẩu: ${password}`);

            // Sau khi đăng nhập, có thể làm trống các ô nhập liệu nếu muốn:
            document.getElementById('email').value = '';
            document.getElementById('password').value = '';
        }
    </script>

</body>
</html>
