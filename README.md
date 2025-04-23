</html># risk-profile-form
投資風險屬性線上問卷
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>投資風險屬性問卷</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      padding: 20px;
      background-color: #f9f9f9;
    }
    h1, h2 {
      color: #2c3e50;
    }
    .question {
      margin-bottom: 25px;
      background: white;
      padding: 15px;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    label {
      display: block;
      margin: 6px 0;
    }
    button {
      padding: 10px 20px;
      background-color: #2980b9;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #3498db;
    }
  </style>
</head>
<body>
  <h1>富邦人壽 投資風險屬性問卷</h1>

  <form id="riskForm">
    <div class="question">
      <h2>一、年齡：</h2>
      <label><input type="radio" name="age" value="18-35">18-35歲</label>
      <label><input type="radio" name="age" value="36-45">36-45歲</label>
      <label><input type="radio" name="age" value="46-55">46-55歲</label>
      <label><input type="radio" name="age" value="56-64">56-64歲</label>
      <label><input type="radio" name="age" value="65以上">65歲以上</label>
    </div>

    <div class="question">
      <h2>二、投資經驗：</h2>
      <label><input type="checkbox" name="experience" value="定存">定存</label>
      <label><input type="checkbox" name="experience" value="基金">基金</label>
      <label><input type="checkbox" name="experience" value="股票/ETF">股票/ETF</label>
      <label><input type="checkbox" name="experience" value="期貨">期貨</label>
      <label><input type="checkbox" name="experience" value="無">無投資經驗</label>
    </div>

    <div class="question">
      <h2>三、投資目標：</h2>
      <label><input type="radio" name="goal" value="保本">保本</label>
      <label><input type="radio" name="goal" value="穩定收益">穩定收益</label>
      <label><input type="radio" name="goal" value="資產增值">資產增值</label>
    </div>

    <div class="question">
      <h2>四、可接受的最大虧損程度：</h2>
      <label><input type="radio" name="loss" value="5%">5%以內</label>
      <label><input type="radio" name="loss" value="10%">10%以內</label>
      <label><input type="radio" name="loss" value="20%">20%以內</label>
      <label><input type="radio" name="loss" value=">20%">超過20%</label>
    </div>

    <div class="question">
      <h2>五、投資期間：</h2>
      <label><input type="radio" name="duration" value="1年以內">1年以內</label>
      <label><input type="radio" name="duration" value="1-3年">1-3年</label>
      <label><input type="radio" name="duration" value="3年以上">3年以上</label>
    </div>

    <div class="question">
      <button type="submit">提交問卷</button>
    </div>
  </form>

  <script>
    document.getElementById(\"riskForm\").addEventListener(\"submit\", function(event) {
      event.preventDefault();
      alert(\"問卷已提交，謝謝您的填寫！\");
    });
  </script>
</body>
