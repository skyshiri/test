## HER Messenger - 정세진

### 취약점
- HER 메신저는 접속시 별도의 인증절차가 없음
- 헐 메신저에서 누구나 원하는 누군가인 척 할 수 있음

---
### 공격 모델
![attack](images/attack.jpg)

---
### 문제점
- 기존 key protocol을 수정하지 않을 경우 공격 불가
  - 낙준은 가짜 세진과 채팅할 때, 진짜 세진의 아이디로 암호화(enc)
  - 가짜 세진은 복호화(dec) 불가로 오류 발생하고, 해당파일에 있는 code 수정 필요  
- key protocol 수정
  - 기존 메신저 아이디로 암/복호화 -> 아이디별 fingerprint로 암/복호화

---
### 실행방법
- attacker는 githubA로 접속하여 채팅 리스트에서 공격 대상자를 확인
- 채팅 리스트에서 공격하고자 하는 대상의 아이디 가짜 세진의 키를 생성
- 공격자용 Her Messenger 프로그램 만들기
- attacker는 진짜 세진이 채팅 리스트에서 나갈 때까지 기다림
- 가짜 세진은 nakjun(victim)에게 피싱공격

---
### DEMO
![Video](https://youtu.be/embed/3HkWb2PC_z8)
