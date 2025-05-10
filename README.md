# -2025-
에듀테크2025학년도수능수학공통
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>성취자아 성장 웹앱</title>
  <style>
    body { font-family: sans-serif; text-align: center; padding: 30px; }
    .avatar { font-size: 2em; margin: 20px; }
    .unit { font-size: 1.5em; margin: 10px; }
    button { padding: 10px 20px; font-size: 1.2em; }
  </style>
</head>
<body>
  <h1>수능 수학 22단계 퀘스트</h1>
  <div class="avatar">📏 성취자아</div>
  <div class="unit" id="unitDisplay">현재: 1 퀰토미터</div>
  <button onclick="nextStep()">다음 문제 풀기</button>

  <script>
    const units = [
      "퀰토미터", "론토미터", "요크토미터", "젭토미터", "앱토미터",
      "펨토미터", "피코미터", "나노미터", "마이크로미터", "밀리미터",
      "센티미터", "데시미터", "미터", "데카미터", "헥토미터",
      "킬로미터", "메가미터", "기가미터", "테라미터", "페타미터",
      "엑사미터", "제타미터", "요타미터"
    ];

    let current = 0;
    function nextStep() {
      if (current < 22) {
        current++;
        document.getElementById('unitDisplay').innerText = `현재: ${current + 1} ${units[current]}`;
      } else {
        alert("모든 문제를 풀었습니다! 🎉");
      }
    }
  </script>
</body>
</html>
