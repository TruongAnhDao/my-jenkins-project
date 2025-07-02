pipeline {
    agent any // Chạy trên bất kỳ agent nào

    stages {
        stage('Checkout Code') {
            steps {
                // Tự động lấy mã nguồn từ kho chứa Git mà job này được cấu hình
                checkout scm
                echo 'Đã lấy mã nguồn thành công!'
            }
        }
        stage('Build') {
            steps {
                echo 'Bắt đầu quá trình build...'
                sh 'ls -la' // Liệt kê các file trong thư mục làm việc để xem code đã được lấy về chưa
            }
        }
        stage('Test') {
            steps {
                echo 'Giả lập việc chạy test...'
            }
        }
    }
}