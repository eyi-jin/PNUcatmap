# PNUcatmap

4/7
* 기존 로그인 오류 수정
  -> 로그아웃 버튼 추가
  -> 이메일 로그인, 회원가입 버튼 분리
  
* 기존의 drawable activity(Homeactivity) -> empty activity(Homeactivity2)로 수정

---------------동작 방식---------------------
* MainActivity 
- 이메일 로그인
 -> 로그인 버튼, 회원가입 버튼 
- 구글 로그인

* HomeActivity2
- 이메일 로그인 시 이동하는 액티비티

* SignupActivity
 -MainActivity에서 회원가입 버튼 누르면 이동하는 액티비티
 
 ---------------추가 오류발견------------------
 - 여러 개의 액티비티가 밑에 깔려있어서 종료시 계속 닫아야함
 - 이메일 회원가입 register시, 이메일을 확인하라는 토스트메시지 띄운다음 사라지게 만들면 자연스러울 것 같음
 - 구글 로그인 제대로 화면 전환 안함
 - 로그인시 비밀번호 설정창과, 회원가입시 비밀번호 설정창 다름(-> 숫자만 나오는것, 영어입력도 가능한 것)
