# iloveyou
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Một hỏi nhỏ dành cho cậu</title>
    <style>
        body {
            background-color: pink;
            font-family: Arial, sans-serif;
            padding: 20px;
        }
        h1 {
            color: #333;
        }
        .question {
            margin: 20px 0;
        }
        a {
            text-decoration: none;
            color: white;
            background-color: #007BFF;
            padding: 10px 15px;
            border-radius: 5px;
            margin-right: 10px;
        }
        #response {
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <h1>Câu hỏi Có/Không</h1>
    
    <div class="question">
        <p>Vui lòng trả lời câu hỏi dưới đây:</p>
        <p>Ngay bây giờ, một người nào đó đang chờ cậu trước cổng trên tay là một bông hoa, cậu có dám gặp hông?</p>
        <button onclick="recordResponse('Có')">Có</button>
        <button onclick="recordResponse('Không')">Không</button>
    </div>

    <div id="response"></div>

    <script>
        function recordResponse(answer) {
            const responseDiv = document.getElementById('response');
            responseDiv.innerHTML = `Bạn đã chọn: <strong>${answer}</strong>`;
            // Ở đây, bạn có thể thêm mã để ghi nhận câu trả lời vào cơ sở dữ liệu hoặc API nếu cần.
        }
    </script>

</body>
</html>

