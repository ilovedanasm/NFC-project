# NFC-project<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>تصريح الخروج - بطاقة ذكية</title>
  <style>
    body {
      font-family: Tahoma;
      background-color: #f0f8ff;
      text-align: center;
      padding-top: 50px;
    }
    h1 {
      color: #0d47a1;
    }
    button {
      padding: 15px 30px;
      font-size: 17px;
      background-color: #1565c0;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    #info {
      margin-top: 40px;
      font-size: 20px;
      color: #333;
      line-height: 1.8;
    }
  </style>
</head>
<body>

  <h1>نظام البطاقة الذكية - تصريح خروج</h1>
  <p>اضغطي الزر لمحاكاة تمرير بطاقة الخروج</p>
  <button onclick="passCard()">تم تمرير البطاقة</button>

  <div id="info"></div>

  <script>
    function passCard() {
      let teacherName = "المعلمة حصة العليقي";
      let subject = "معلمة الرياضيات";
      let status = "تم منح تصريح الخروج للطالبة";
      let time = new Date().toLocaleTimeString('ar-EG');

      document.getElementById("info").innerHTML = `
        <p><strong>اسم المعلمة:</strong> ${teacherName}</p>
        <p><strong>المادة:</strong> ${subject}</p>
        <p><strong>نوع البطاقة:</strong> ${status}</p>
        <p><strong>الوقت:</strong> ${time}</p>
      `;
    }
  </script>

</body>
</html>
