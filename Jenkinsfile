// pipeline{
//     agent any
//     stages{
//         stage("Hello") {
//             steps{
//                 sh "robot mytest.robot"
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
        stage("Hello") {
            steps {
                // เพิ่ม PATH ให้ Jenkins หา robot command เจอ
                sh '''
                    export PATH=$PATH:/Library/Frameworks/Python.framework/Versions/3.13/bin
                    robot mytest.robot
                '''
            }
        }
    }
}