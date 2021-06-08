# AWS 6주차 :cloud:  

## 웹 서비스 구현하기    
- DB 생성, User 생성, Table 생성, 데이터 입력       
- PHP 와 Mysql 연동 라이브러리 설치       
- php 파일 생성하여 web page 로 데이터 입력 , Data 생성 확인         
- 현재 구조       
![KakaoTalk_20210602_154218383](https://user-images.githubusercontent.com/66204538/121215493-0730a480-c8bb-11eb-8115-7cfc76b5a828.png)           
----------------------------------------------     
        
- clouddb 생성      
![1-1  클라우드디비 생성 후 권한 부여](https://user-images.githubusercontent.com/66204538/121212732-92f50180-c8b8-11eb-8efa-a6b8a3e962ff.JPG)          

test 유저가 사용하는 clouddb를 생성하고 권한을 부여한다.         
        
- test 유저로 접속하여 clouddb에 topic 테이블을 생성하고 데이터를 입력한다.       
![6 clouddb 커넥트](https://user-images.githubusercontent.com/66204538/121213246-0860d200-c8b9-11eb-9b12-f41057c75aaa.JPG)         
![1-2  클라우드디비에 토픽테이블 생성](https://user-images.githubusercontent.com/66204538/121213301-1282d080-c8b9-11eb-982b-dee4127667b8.JPG)          
           
- php - mysql 연동 모듈을 설치한다.          
![1  php-mysql 연동](https://user-images.githubusercontent.com/66204538/121213576-537ae500-c8b9-11eb-85e7-c6d67d78f8d1.JPG)          
               
- mysql과 apache를 재시작하고 해당 모듈이 잘 설치되었는지 확인한다.         
![2 연동모듈 잘 깔렸는지 확인](https://user-images.githubusercontent.com/66204538/121213759-7dcca280-c8b9-11eb-8789-97e6785306ae.JPG)          
           
- nano 에디터를 통해 create.php와 process_create.php 페이지를 생성한다.      
![4  create php 작성 엔드포인트+유저+비밀번호+디비이름 설정](https://user-images.githubusercontent.com/66204538/121213932-a81e6000-c8b9-11eb-94de-4c54f742961a.JPG)          
         
주소에는 RDS의 엔드포인트를 쓰고, clouddb와 생성한 유저와 비밀번호를 입력한다.       
해당 페이지는 영화 제목, 본문, 저자의 이름을 사용자에게 입력 받고 process_create.php로 전달한다.          
             
![5 process_create php 생성](https://user-images.githubusercontent.com/66204538/121214332-faf81780-c8b9-11eb-972d-a4e265eede41.JPG)          
           
create.php와 똑같은 설정을 process_create.php에도 한다.        
해당 페이지는 사용자가 입력한 정보를 데이터베이스에 업데이트한다.        

- 웹 페이지를 통해 데이터 입력 후 toad로 연동 확인        
![7 create php 접속](https://user-images.githubusercontent.com/66204538/121214743-6215cc00-c8ba-11eb-946c-f1205d18e793.JPG)            
![8 데이터 전송](https://user-images.githubusercontent.com/66204538/121215023-9a1d0f00-c8ba-11eb-932f-a838b237a083.JPG)

create.php에 접속해 정보를 입력한다.          
            
![9 데이터 업데이트 확인](https://user-images.githubusercontent.com/66204538/121215131-b456ed00-c8ba-11eb-8431-c665814e86ba.JPG)           
           
toad로 들어가 데이터가 잘 업데이트 되었는지 select 문을 통해 확인한다.         



