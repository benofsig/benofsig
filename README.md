<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<title>암호 기반 링크 접근</title>
<script>
  function checkPassword() {
    var password = document.getElementById('password').value;
    var correctPassword = '4149494dpawidw12391';
    var link = 'https://www.dropbox.com/scl/fi/7iid8y0n91kko96k3pycy/5.m4a?rlkey=96oq6swl37yzyj4jmbrsozl8q&st=hrfv5prk&dl=0';

    if(password === correctPassword) {
      window.location.href = link;
    } else {
      alert('잘못된 암호입니다.');
    }
  }
</script>
</head>
<body>
  <input type="password" id="password" placeholder="암호를 입력하세요">
  <button onclick="checkPassword()">제출</button>
</body>
</html>
