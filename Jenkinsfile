pipeline {
    agent any
    
    stages {
        stage('拉取git-hub 程式') {
            steps {
                git 'https://github.com/TanNeil/Jenkins-Test.git'
            }
        }
        stage('通過maven構建項目') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('通過sonarqube做代碼檢測') {
            steps {
                // 添加SonarQube检测步骤指令
            }
        }
        stage('通過Docker構建image') {
            steps {
                // 添加Docker构建步骤指令
            }
        }
        stage('將image推送到harbor') {
            steps {
                // 添加推送到Harbor的步骤指令
            }
        }
    }
}
