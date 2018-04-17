## HER Messenger-정세진

### 취약점
- HER 메신저는 접속시 별도의 인증절차가 없음
- 누구나 원하는 누군가인 척 할 수 있음

---
### 공격 모델
![attack](images/attack.jpg){: width="5%" height="7%"}

---
### 문제점
- 기존 key protocol을 수정하지 않을 경우 공격 불가
   - nakjun은 sejin(fake)과 채팅할 때, sejin(real)  
   아이디로 암호화(enc)
   - sejin(fake)은 복호화(dec) 불가로 채팅 불가
- key protocol 수정
   - 메신저 아이디로 암/복호화  
    -> 아이디별 fingerprint로 암/복호화

---
### 실행방법
1. attacker는 githubA로 접속할 때, 채팅 리스트에서  
공격 대상자 확인
2. 채팅 리스트에서 공격 대상인 sejin(fake)의 키 생성
3. 공격자용 메신저 프로그램 만들어서 Docker 실행
4. attacker는 sejin(real)이 채팅 리스트에서  
나갈 때까지 기다림
5. sejin(fake)은 nakjun에게 피싱공격 가능

---
### DEMO
![Video](https://youtube.com/embed/3HkWb2PC_z8)
