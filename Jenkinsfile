// pipeline{
//     agent any
//     stages{
//         stage("Hello"){
//             steps{
//                 sh "pip list"
//                 // robot (
//                 //     outputPath: './',
//                 //     outputFileName: 'output.xml'
//                 //     reportFileName: 'report.html',
//                 //     logFileName: 'log.html',
//                 //     disableArchiveOutput: false,
//                 //     passThreshold: 100.0,
//                 //     unstableThreshold: 100.0,
//                 //     otherFiles: '*-png,*-jpg',
//                 //     onlyCritical: false
//                 // )
//             }
//         }
//     }
// }

pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Checkout โค้ดจากระบบ SCM (เช่น Git)
                checkout scm
            }
        }
        stage('แสดงรายการแพ็กเกจที่ติดตั้ง') {
            steps {
                // รันคำสั่ง pip list เพื่อแสดงแพ็กเกจที่ติดตั้ง
                sh 'pip list'
            }
        }
    }
}