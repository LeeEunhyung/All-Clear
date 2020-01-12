# All-Clear
- 2019 2학기 Capstone 창의설계경진대회 - React.js를 활용한 수강 신청 시스템 (Reca+ Team Project)
- 기존의 수강 신청 시스템에 __보기 쉬운 UI__ 와 __편리한 기능__ 을 추가한 서비스  
   ※ 제공되는 DB가 없었기 때문에 test DB를 직접 설계   

### Environment
- OS : Windows 10 Pro
- Tool : Visual Studio Code, Putty
- Server : AWS EC2, nodejs, mySQL
- Language : html, React.js (JavaScript), css

### Issue & Solution
- __Issue.1__ 최신 개발 동향에 맞는 Front-End 서비스 제공   
  __Solution.1__ React.js를 활용한 서비스를 제작 / 배포

- __Issue.2__ Client-Server 모델의 Interaction 가능한 서비스 제공    
  __Solution.2__ 무료로 이용이 가능한 AWS EC2를 이용해 서버를 구축, Public 웹 서비스 제공   

- __Issue.3__ 2020년에 지원이 중단되는 Adobe Flash Player를 대체하여 서비스 제공      
  __Solution.3__ Database에서 정보를 추출해 Flash Player없이 앱 서비스에 띄움   

- __Issue.4__ 기존에 제공되는 딱딱하고 보기 힘든 UI / 유용한 기능의 부재   
  __Solution.4__ 직관적이고 보기 좋은 UI 제공 / 사용자 입장에서의 편리한 기능 추가    

### Menu Diagram
- 학생 메뉴 구성도
![1](https://user-images.githubusercontent.com/48666975/72218678-ea3a5980-3580-11ea-8209-3e1f2a61f402.PNG)

- 교수 메뉴 구성도
 ![2](https://user-images.githubusercontent.com/48666975/72218679-ea3a5980-3580-11ea-8bee-6aad116172d4.PNG)
 
 # Installation / Usage
 1. 웹 서버 환경 구축 (AWS EC2 기준)   
    a. AWS에서 제공되는 EC2 서비스를 사용해 웹 서버를 생성합니다.   
    b. EC2 서비스의 인스턴스 Private 키를 발급받아 Putty와 연결 시킵니다.   
    c. Putty로 서버에 접속해 아래의 명령어를 입력해 필수 패키지를 설치합니다.      
    
    - nodejs, n, npm, yarn 설치 및 버전 업데이트   
    ```cmd
    sudo apt-get update  
    sudo apt-get install nodejs   
    sudo apt-get install npm   
    sudo npm cache clean -f   
    sudo npm install -g n   
    sudo n stable   
    sudo npm install -g npm latest   
    sudo npm install -g yarn   
    ```
    
    - create-react-app 설치   
    ```cmd
    sudo npm install -g create-react-app   
    ```
    
    - express, mysql, axios 설치   
    ```cmd
    sudo install express --save   
    sudo apt-get install mysql-server   
    sudo mysql_secure_installation   
    npm install body-parser --save
    npm install mysql --save   
    npm install axios --save   
    ```
    
    - 추가 모듈 설치 (pdf 뷰어, 모달창, 타이머, 메크로 방지 팝업, 메일 전송)
    ```cmd
    sudo yarn global add react-pdf
    sudo yarn global add moment
    sudo yarn global add node-sass
    sudo yarn global add sass-loader
    sudo npm install --save react-google-recaptcha
    sudo npm install nodemailer --save
    sudo npm install html2canvas --save
    sudo npm install jspdf --save
    ```
    
2. React App 생성 및 실행   
    a. 서버 상에서 아래의 명령어를 입력해 create-react-app 폴더를 생성한 후, 앱을 실행시켜 React 페이지를 확인합니다.
    ```
    sudo create-react-app [폴더 이름]
    cd [폴더 이름]
    yarn start
    ```
    
    b. LeeEunhyung/Assignment4_DataVisualization 을 서버에 다운 받아 __a.__ 에서 생성한 폴더에 적용시킨 후, 앱을 실행시켜 해당 페이지를 확인합니다.
    ```
    yarn start
    ```
   
# Screenshot
- 메인 메뉴 화면   

![image](https://user-images.githubusercontent.com/48666975/72218935-de03cb80-3583-11ea-9a83-39d708bd7e9f.png)
   
- 수강 신청 화면   

![image](https://user-images.githubusercontent.com/48666975/72218946-f5db4f80-3583-11ea-8b8d-054becc2ae66.png)

# "Reca+" Team Info
- [LeeEunhyung](https://github.com/LeeEunhyung)
- [wlals7217](https://github.com/wlals7217)
- [1000peach](https://github.com/1000peach)
- [sxxzin](https://github.com/sxxzin)
