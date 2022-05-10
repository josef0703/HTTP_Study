# 2xx(Succeessful)
클라이언트의 요청을 성공적으로 성공

![image](https://user-images.githubusercontent.com/59104703/167559933-f28dbc28-d972-4fa6-b05b-f695b230f163.png)
---
![image](https://user-images.githubusercontent.com/59104703/167560031-2dace419-fa0d-47c7-b72b-06b163fc23c7.png)
---
![image](https://user-images.githubusercontent.com/59104703/167560055-391f11ca-4c16-475c-8e0b-79ecc6661602.png)

---
![image](https://user-images.githubusercontent.com/59104703/167560068-ac244a0f-0623-4e94-9e17-0f8786f2cc03.png)



# 3xx(Redirection)
요청을 완료하기 위해 유저 에이전트의 추가 조치 필요

## 리다이렉션 이해
- 웹 브라우저는 3xx 응답의 결과에 Location 헤더가 있으면, Location 위치로 자동 이동
![image](https://user-images.githubusercontent.com/59104703/167560591-4a1e2f11-6c63-42bb-a409-bbd2664976be.png)

## 리다이렉션 종류
- 영구 리다이렉션 - 특정 리소스의 URI가 영구적으로 이동
  - 예) /event -> /new-event

__영구 리다이렉션 301__
- 리다이렉트시 요청 메서드가 GET으로 변하고, 본문이 제거될 수 있음
![image](https://user-images.githubusercontent.com/59104703/167561368-4d72014c-fdde-42d9-a4f4-aa29032b2c85.png)
  
---

__영구 리다이렉션 308__
- 리다이렉트시 요청 메서드와 본문 유지(처음 POST를 보내면 리다이렉트도 POST 유지)
![image](https://user-images.githubusercontent.com/59104703/167561422-3a8d451b-3255-4fcf-9abc-18fb0d0e1f54.png)

- 일시 리다이렉션 - 일시적인 변경
  - 주문 완료 후 주문 내역 화면으로 이동

**1. 302 Found**

    - 리다이렉트시 요청 메서드가 GET으로 변하고, 본문이 제거될 수 있음(MAY)
    
**2. **307 Temporary Redirect****

    - 302와 기능같음
    - 리다이렉트시 요청 메서드와 본문 유지(요청 메서드를 변경하면 안된다. MUST NOT)
    
**3. **303 See Other****

    - 302와 기능 같음
    - 리다이렉트시 요청 메서드가 GET으로 변경
    
**4. **PRG : Post/Redirect/Get****

    - POST 주문후 브라우저 새로고침하면 중복 주문 방지
    - 주문후 주문 결과 화면으로 리다이렉트

    **PRG 사용전**
    
    ![image](https://user-images.githubusercontent.com/59104703/167565045-1ee6ff2d-c3bb-4ff0-bca0-339947651e37.png)
    ---
    **PRG 사용후**
    
    ![image](https://user-images.githubusercontent.com/59104703/167565196-7f52a191-7334-4e41-bf83-b0b188baf826.png)

**5. 305 Not Modified**

  - 캐시를 목적으로 사용
  - 클라이언트는 로컬PC에 저장된 캐시를 재사용 (캐시로 리다이렉트)

- 특수 리다이렉
  - 결과 대신 캐시를 사용



# 4xx
