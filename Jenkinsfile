pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/KNithyakala/RobotFrameWork.git'
            }
        }
        stage('Install Requirements') {
            steps {
                bat '"C:\\Python313\\python.exe" -m pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                bat '"C:\\Python313\\python.exe" -m robot TestCodes'
            }
        }
    }
}


