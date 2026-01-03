<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <title>Tra cứu điểm thi</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f6f8;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .container {
      background: white;
      padding: 28px 36px;
      border-radius: 14px;
      box-shadow: 0 6px 16px rgba(0,0,0,0.12);
      width: 480px;
    }
    .header {
      text-align: center;
      margin-bottom: 20px;
    }
    .logo {
      max-width: 120px;
      margin-bottom: 8px;
    }
    h1 {
      margin: 6px 0;
      color: #0f172a;
    }
    .subtitle {
      font-size: 14px;
      color: #475569;
      margin-bottom: 12px;
    }
    input {
      width: 100%;
      padding: 10px;
      margin-bottom: 12px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }
    button {
      width: 100%;
      padding: 10px;
      border: none;
      border-radius: 6px;
      background: #16a34a;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }
    button:hover {
      background: #15803d;
    }
    .result {
      margin-top: 16px;
      background: #f0fdf4;
      padding: 14px;
      border-radius: 8px;
      display: none;
    }
    .error {
      color: red;
      text-align: center;
      margin-top: 12px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="header">
      <img src="logo.png" alt="Logo Đỉnh cao Toán học" class="logo" />
      <h1>ĐỈNH CAO TOÁN HỌC</h1>
      <div class="subtitle">Tra cứu điểm thi</div>
    </div>

    <input type="text" id="ten" placeholder="Nhập họ và tên" />
    <input type="date" id="ngaysinh" />
    <button onclick="traCuuDiem()">Tra cứu điểm</button>

    <div class="result" id="result"></div>
    <div class="error" id="error"></div>
  </div>

  <script>
    const thiSinh = {
      hoTen: "Dương Mạnh Tân",
      ngaySinh: "2014-09-19",
      lop: "6",
      diem: {
        toan: 6.5,
        logic: 9.0,
        tuDuy: 9.25
      },
      tongDiem: 24.75,
      xepLoai: "Giỏi"
    };

    function traCuuDiem() {
      const ten = document.getElementById("ten").value.trim().toLowerCase();
      const ngaySinh = document.getElementById("ngaysinh").value;
      const resultDiv = document.getElementById("result");
      const errorDiv = document.getElementById("error");

      resultDiv.style.display = "none";
      errorDiv.innerText = "";

      if (ten === thiSinh.hoTen.toLowerCase() && ngaySinh === thiSinh.ngaySinh) {
        resultDiv.innerHTML = `
          <strong>Họ tên:</strong> ${thiSinh.hoTen}<br>
          <strong>Lớp:</strong> ${thiSinh.lop}<br><br>
          <strong>Điểm thi:</strong><br>
          - Toán: ${thiSinh.diem.toan}<br>
          - Logic: ${thiSinh.diem.logic}<br>
          - Tư duy: ${thiSinh.diem.tuDuy}<br><br>
          <strong>Tổng điểm:</strong> ${thiSinh.tongDiem}<br>
          <strong>Xếp loại:</strong> ${thiSinh.xepLoai}
        `;
        resultDiv.style.display = "block";
      } else {
        errorDiv.innerText = "Thông tin không chính xác hoặc không tìm thấy thí sinh.";
      }
    }
  </script>
</body>
</html>
