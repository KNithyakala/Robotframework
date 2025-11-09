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
                bat '"C:\\Users\\CK NITHYAKALA\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" -m pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                bat '"C:\\Users\\CK NITHYAKALA\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe" -m robot TestCodes'
            }
        }
    }
}

