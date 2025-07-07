pipeline {
    agent any

    parameters {
        string(name: 'PERSON_NAME', defaultValue: 'Khách', description: 'Tên người cần chào?')
        choice(name: 'GREETING_TYPE', choices: ['Thân mật', 'Trang trọng'], description: 'Kiểu chào?')
    }

    stages {
        stage('Personalized Greeting') {
            steps {
                script { // Cần khối 'script' để dùng if/else
                    if (params.GREETING_TYPE == 'Thân mật') {
                        echo "Yo, ${params.PERSON_NAME}!"
                    } else {
                        echo "Xin kính chào quý ngài ${params.PERSON_NAME}."
                    }
                }
            }
        }
    }
}