# AWS 5주차 :cloud:  

## PHP와 아파치 서버의 연동, RDS 생성    

-PHP5.6을 설치해 아파치 서버와 연동하고, MySql 기반의 RDS를 생성한다.     

-----------------------------------------------------------------------      
-php 5.6을 설치한다.       
![php설치](https://user-images.githubusercontent.com/66204538/121376252-5559ac80-c97c-11eb-9437-7535b7ce28e4.JPG)            
![2 apt update](https://user-images.githubusercontent.com/66204538/121376398-75896b80-c97c-11eb-867e-ab08b2084dfb.JPG)              
![3 php 5 6설치JPG](https://user-images.githubusercontent.com/66204538/121376430-7e7a3d00-c97c-11eb-8c80-5c9aff2337e2.JPG)            
          
잘 설치되었는지 버전을 확인한다.        

![4 php 버전확인](https://user-images.githubusercontent.com/66204538/121376553-98b41b00-c97c-11eb-9cc0-23f83d2166a3.JPG)            

-잘 설치된 것을 확인했다면 /var/www/html/로 들어가 index.php 파일을 생성한다.        
           
![5 index php 파일 생성](https://user-images.githubusercontent.com/66204538/121376654-a8336400-c97c-11eb-8e5d-0eb9c13d1337.JPG)           
         
해당 파일은 phpinfo를 통해 php 정보를 페이지에 출력한다.       
           
![6 php 인포페이지 생성](https://user-images.githubusercontent.com/66204538/121376986-f5173a80-c97c-11eb-95f3-f6e4cc3dedc2.JPG)           
![7 페이지생성확인](https://user-images.githubusercontent.com/66204538/121377048-03655680-c97d-11eb-9663-9ac92d43891b.JPG)           
        
php 페이지가 정상적으로 출력되는 것을 확인할 수 있다.         
             
-------------------------------------------------------------------------------                
         
-RDS 생성       
![8 rds콘솔창](https://user-images.githubusercontent.com/66204538/121377316-33acf500-c97d-11eb-8f6b-87f938288789.JPG)        
          
RDS 콘솔창으로 접속해 데이터베이스 생성을 클릭한다.         
      
-데이터베이스 생성을 진행한다.        
![9 데이터베이스 표준생성,mysql, 프리티어](https://user-images.githubusercontent.com/66204538/121377514-5ccd8580-c97d-11eb-996a-d408c93480b6.JPG)          
표준생성으로 진행하며, 엔진은 Mysql, 프리티어로 설정한다.        
        
![10 인스턴스식별자,마스터이름,암호 인스턴스 크기설정](https://user-images.githubusercontent.com/66204538/121377745-91414180-c97d-11eb-9ea6-486d477e20aa.JPG)             
인스턴스 식별자와 마스터 이름, 암호를 설정한다.         
         
![11 퍼블릭엑세스 설정](https://user-images.githubusercontent.com/66204538/121377903-b2099700-c97d-11eb-8d40-52201b68827b.JPG)                
웹 서비스를 위한 데이터베이스이기 때문에 퍼블릭 엑세스가 가능하도록 설정한다.        
           
![12 데이터베이스 생성](https://user-images.githubusercontent.com/66204538/121378088-d82f3700-c97d-11eb-8808-45a410bb41de.JPG)           
그대로 데이터베이스를 생성한다.        
            
![13 데이터베이스생성완료](https://user-images.githubusercontent.com/66204538/121378200-f301ab80-c97d-11eb-97e0-6808fc930358.JPG)            
몇 분 후에 정상적으로 생성이 완료된다.          
            
-생성된 데이터베이스의 엔드포인트를 확인하고 콘솔창으로 데이터베이스에 접속한다.        
![14 엔드포인트 확인](https://user-images.githubusercontent.com/66204538/121378425-280dfe00-c97e-11eb-8fba-f7be442ce07f.JPG)                 
![15 테라텀으로 데이터베이스 접속](https://user-images.githubusercontent.com/66204538/121378456-2e9c7580-c97e-11eb-8a60-1b82236503ed.JPG)               
          
![16 잘들어가있다](https://user-images.githubusercontent.com/66204538/121378512-3c51fb00-c97e-11eb-99a7-5e5fd82f3293.JPG)               
간단한 쿼리문으로 확인한다.         
            
-Toad로 데이터베이스에 접속한다.        
![17 toad로 접속](https://user-images.githubusercontent.com/66204538/121378665-5c81ba00-c97e-11eb-97b5-5d7abec80286.JPG)                 
Host에는 엔드포인트를 붙여 놓는다.          
            
![18 toad 확인](https://user-images.githubusercontent.com/66204538/121378714-65728b80-c97e-11eb-8425-bacd584d8ab3.JPG)           
간단한 쿼리문을 통해 정상적으로 연결되었음을 확인한다.             
                    
                    
                    

 
