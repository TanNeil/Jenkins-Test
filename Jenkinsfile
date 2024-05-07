pipeline {
    agent any
    
    stages {
        stage('拉取git-hub 程式') {
            steps {
                script {
                    // 拉取代码
                    git 'https://github.com/TanNeil/Jenkins-Test.git'
                }
            }
        }
        stage('通過maven構建項目') {
            steps {
                script {
                    // 使用Maven构建项目
                    sh 'mvn clean install'
                }
            }
        }
        stage('通過sonarqube做代碼檢測') {
            steps {
                script {
                    // 执行SonarQube代码检测
                    // 添加具体的SonarQube步骤指令
                }
            }
        }
        stage('通過Docker構建image') {
            steps {
                script {
                    // 使用Docker构建镜像
                    // 添加具体的Docker构建步骤指令
                }
            }
        }
        stage('將image推送到harbor') {
            steps {
                script {
                    // 将镜像推送到Harbor
                    // 添加具体的推送到Harbor的步骤指令
                }
            }
        }
    }
}
