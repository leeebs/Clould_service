# 리눅스 명령어 및 웹 페이지 수정

       
## 1. 리눅스 명령어
        
ls -l : 디렉토리에 있는 파일을 나열한다.     
pwd : 현재 디렉토리의 전체 경로를 보여준다.     
sudo : root 사용자가 할 수 있는 작업의 권한을 준다.     
apt-get install : 파일 설치    
apt-get update : 파일 업데이트    
passwd : 사용자 비밀번호 변경    
su : 사용자 바꾸기    
cd : 디렉토리 바꾸기     
mkdir : 디렉토리 생성   
touch : 새 파일 생성    
rm : 파일이나 디렉토리 삭제     
     
![3](https://user-images.githubusercontent.com/66204538/116263203-257f8c80-a7b4-11eb-874b-7654520b75a8.JPG)
       
![12](https://user-images.githubusercontent.com/66204538/116263356-4516b500-a7b4-11eb-90a4-2ace1f0252d0.JPG)
        
![13](https://user-images.githubusercontent.com/66204538/116263420-519b0d80-a7b4-11eb-8d50-2cedc6524bd8.JPG)
      
![14](https://user-images.githubusercontent.com/66204538/116263549-6b3c5500-a7b4-11eb-83d1-6ce315e1e41f.JPG)
    
## 2. 웹 페이지 수정
       
apt-get install apache2를 통해 파일을 설치하고, apt-get update를 통해 설치 파일을 최신화한다.       
      
![15](https://user-images.githubusercontent.com/66204538/116262386-75118880-a7b3-11eb-8294-b1fab2b1fc11.JPG)
![16](https://user-images.githubusercontent.com/66204538/116262531-95414780-a7b3-11eb-9ff9-3632fd4248f5.JPG)
        
apache가 설치되었다면, 생성된 인스턴스의 퍼블릭 IPv4 주소를 주소창에 입력해보자. 초기 apache 페이지가 나온다.     
       
![아파치초기](https://user-images.githubusercontent.com/66204538/116262602-a722ea80-a7b3-11eb-9952-ac8a0b9adf1b.jpg)
       
해당 초기 화면은 /var/www/html에 있는 index.html 파일이다.      
cd를 통해 디렉토리를 변경하고 index.html이 있는지 확인한다.     
          
![18](https://user-images.githubusercontent.com/66204538/116262732-c15cc880-a7b3-11eb-985f-23a0b7629c13.JPG)
         
파일을 수정할 때 초기 파일은 남겨 두는 것이 좋으므로 index_org.html로 옮기고 index.html을 작성한다.     
nano 에디터를 통해 내용을 수정한다.     
       
![아파치파읽수정](https://user-images.githubusercontent.com/66204538/116262941-eb15ef80-a7b3-11eb-96b1-00b9284c3cb5.jpg)
       
다시 퍼블릭 주소를 입력하면 작성한 index 파일 내용이 나온다.

![아파치수정](https://user-images.githubusercontent.com/66204538/116263015-fd902900-a7b3-11eb-9be8-0988d66d86cd.jpg)
