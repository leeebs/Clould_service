# AWS 1주차 :cloud:


### 1. EC2 인스턴스 생성
------------------------
미리 가입한 AWS 계정으로 콘솔에 접속한다.   
   
![1](https://user-images.githubusercontent.com/66204538/114639106-04289600-9d08-11eb-8824-0f93f762f132.png)
  
콘솔창에서 EC2 서비스로 들어가 인스턴스 시작을 누른다.   
지금은 중지된 인스턴스가 하나 있지만 모든 과정을 거치면 실행중인 인스턴스가 생성될 것이다.
   
![2](https://user-images.githubusercontent.com/66204538/114639119-0be83a80-9d08-11eb-8ce4-9aad85993d02.png)    

AMI 선택창에서 운영체제를 선택할 수 있다. 프리티어인 ubuntu server LTS 18.04를 선택한다.   
   
![3](https://user-images.githubusercontent.com/66204538/114639132-14407580-9d08-11eb-8ca2-72343b8ae41b.png)
   
   
상황에 맞는 인스턴스 유형을 선택한다.    
인스턴스 생성을 연습하는 과정이니 과금이 되지 않는 프리티어를 선택한다.

![4](https://user-images.githubusercontent.com/66204538/114639155-1e627400-9d08-11eb-88c5-93a8eae0685a.png)     

인스턴스 세부 정보를 구성한다.    
종료 방식은 중지로 설정한다.

![5](https://user-images.githubusercontent.com/66204538/114639170-24f0eb80-9d08-11eb-9af5-1542108a561d.png)    

사용량에 맞는 스토리지를 설정하고     

![6](https://user-images.githubusercontent.com/66204538/114639194-2b7f6300-9d08-11eb-99af-71da6ab2879a.png)    

적절한 태그를 추가한다.   
태그는 어떤 인스턴스를 만들고, 어떤 용도, 누가 관리 하는지 등의 메모(설명) 기능이라고 볼 수 있다.

![7](https://user-images.githubusercontent.com/66204538/114639211-33d79e00-9d08-11eb-9067-bb22916cf4ac.png)    

보안 그룹을 설정한다.     
리눅스 계열 방식인 SSH와 웹 브라우저로 접속하는 경우인 HTTP를 설정한다.   
웹 서비스를 위한 인스턴스이므로 관리를 위한 SSH는 내 IP로 서비스를 위한 HTTP는 위치 무관으로 설정한다.   


![8](https://user-images.githubusercontent.com/66204538/114639227-3b974280-9d08-11eb-9c43-faecad1c224b.png)     

마지막 검토 단계에서 인스턴스 설정 정보를 모두 확인할 수 있다.     

![9](https://user-images.githubusercontent.com/66204538/114639236-4356e700-9d08-11eb-97ec-f63e95b5eb19.png)
    

새 키페어를 생성해 다운로드 받고 인스턴스를 시작할 수 있다.    

![10](https://user-images.githubusercontent.com/66204538/114639246-4baf2200-9d08-11eb-8551-9594fa6459fa.png)     

![11](https://user-images.githubusercontent.com/66204538/114639260-54075d00-9d08-11eb-9dce-eb5e9a2e7e2d.png)     

인스턴스 보기를 클릭해 넘어가면 인스턴스가 실행 중인 것을 확인할 수 있다.    

![12](https://user-images.githubusercontent.com/66204538/114639278-5c5f9800-9d08-11eb-81a4-66c23a129b6b.png)    
    
    


### 2. 터미널 접속
------------------------
터미널을 통해 접속하기 위해 Tera Term을 이용한다.    

Tera Term을 설치한 뒤에 실행시킨 다음 호스트 IP에 생성한 인스턴스의 퍼블릭 IPv4 주소를 붙여 넣는다.     

![13](https://user-images.githubusercontent.com/66204538/114639288-64b7d300-9d08-11eb-8a82-4a0b697a82b4.png)
     

사용자 이름을 입력하고 키 로그인을 선택해 인스턴스를 생성했을 때 받았던 키페어의 경로를 입력한다.    

![14](https://user-images.githubusercontent.com/66204538/114639299-6bdee100-9d08-11eb-8a68-ca32a1669bba.png)      

모든 과정이 정상적으로 진행되면 터미널과 인스턴스의 연결이 완료된다.     

![15](https://user-images.githubusercontent.com/66204538/114639307-7305ef00-9d08-11eb-99b1-fa089f74913b.png)    


### 3. 느낀점
---------------------------
인스턴스를 생성하고 여러 설정을 통해 서비스에 적합한 인스턴스를 구성하는 법을 알게 되었다. 나중에 쓸 일이 많을 것 같다.
