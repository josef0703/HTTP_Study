# HTTP(HyperText Transfer Protocol) 
- HTTP 메시지에 모든 것을 전송 가능
- 서버간에 데이터 주고 받을 떄도 대부분 HTTP 사용

## Stateful, Stateless 차이
- 상태유지 : 중간에 다른 점원으로 바뀌면 안된다.
- 무상태 : 중간에 다른 점원으로 바뀌어도 된다.
- 무상태는 응답 서버를 쉽게 바꿀 수 있다. -> 무한한 서버 증설 가능

## Stateless 장점
1. 아무 서버나 호출 가능

![image](https://user-images.githubusercontent.com/59104703/167240994-ac81630e-57bf-472c-a6ee-0629902fd1db.png)


2. 수평 확장 유리

![image](https://user-images.githubusercontent.com/59104703/167240999-77f37040-4b1e-4cb3-8021-20911a40d89a.png)

## Stateless 한계
- 모든 것을 무상태로 설계 할 수 없음
- 무상태
  -  예) 로그인이 필요없는 단순한 화면

- 상태 유지
  - Ex) 로그인
- 일반적으로 브라우저 쿠키와 서버 세션등을 사용해서 상태 유지

## 비연결성
![image](https://user-images.githubusercontent.com/59104703/167241090-c4d13c7a-c16d-4fc8-9fc4-f2bb08d34bcb.png)
- HTTP는 기본이 연결을 유지하지 않는 모델
- 서버 자원을 효율적으로 사용

## 비연결성 한계와 극복
- TCP/IP 연결을 새로 맺어야함 - 3 way handshake 시간 추가
- HTTP 지속 연결(Persistent Connection)로 문제 해결

### HTTP 초기
![image](https://user-images.githubusercontent.com/59104703/167241111-d8525c35-c8c3-4652-ab6e-adaf671e792c.png)

### HTTP 지속 연결
![image](https://user-images.githubusercontent.com/59104703/167241124-c9a59bc4-8dc5-4802-b547-93ed94605414.png)


# HTTP 메시지
![image](https://user-images.githubusercontent.com/59104703/167241189-96f7413d-2833-479f-82dd-a39edfabaf61.png)

## 요청 메시지
 ![image](https://user-images.githubusercontent.com/59104703/167241260-896e6a4d-357b-4d22-86ea-4090f960673a.png)
 
 ![image](https://user-images.githubusercontent.com/59104703/167241265-47576a32-4343-4005-aa9f-79415686690f.png)
 
 ![image](https://user-images.githubusercontent.com/59104703/167241269-9b17e78b-524b-4168-9347-8367c0258f6c.png)
 
 ![image](https://user-images.githubusercontent.com/59104703/167241274-dba9c424-f7e6-481b-b5fb-dfdbede93e21.png)

## 시작라인 - 응답 메시지
 ![image](https://user-images.githubusercontent.com/59104703/167241371-c6b21dd7-0dfe-4b0c-94b8-c5f945f1ee8b.png)

## HTTP 헤더
![image](https://user-images.githubusercontent.com/59104703/167241384-436ff986-81ec-4d79-bfa4-a2124eff4bcd.png)

## HTTP 메시지 바디
 ![image](https://user-images.githubusercontent.com/59104703/167241397-ffb8381c-7e13-45cc-9087-3529765ae9df.png)






