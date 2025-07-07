@Library('my-global-library') _

pipeline {
    agent any

    stages {
        stage('Test Shared Library') {
            steps {
                script {
                    // Bây giờ bạn có thể gọi các hàm trong file logUtils.groovy
                    logUtils.info('Pipeline đã bắt đầu.')
                    logUtils.warn('Đây là một cảnh báo thử nghiệm.')

                    // Dòng dưới sẽ gây lỗi và dừng pipeline, bạn có thể thử bỏ comment để xem.
                    // logUtils.error('Đây là một lỗi nghiêm trọng!')
                }
            }
        }
    }
}