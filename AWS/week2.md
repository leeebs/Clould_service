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
     
    
    
## 2. 웹 페이지 수정
       
apt-get install apache2를 통해 파일을 설치하고, apt-get update를 통해 설치 파일을 최신화한다.       
      
apache가 설치되었다면, 생성된 인스턴스의 퍼블릭 IPv4 주소를 주소창에 입력해보자. 초기 apache 페이지가 나온다.     

해당 초기 화면은 /var/www/html에 있는 index.html 파일이다.      
cd를 통해 디렉토리를 변경하고 index.html이 있는지 확인한다.     

파일을 수정할 때 초기 파일은 남겨 두는 것이 좋으므로 index_org.html로 옮기고 index.html을 작성한다.     
nano 에디터를 통해 내용을 수정한다.     

다시 퍼블릭 주소를 입력하면 작성한 index 파일 내용이 나온다.

