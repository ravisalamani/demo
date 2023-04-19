@Library("public@demo") _
import com.microchip.Utilities
config            = [:]
config.server     = "MyLinuxServer"
def utils = new Utilities(this)
pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                 script {
                    utils.notifyPR({cred:"PrecheckInRobot"},"Hello","World")
                    utils.pwd()
                    println "Hello World"
                    //sendMail("Hello World","ravi.salamani@microchip.com")
                 }
            }
        }
    }
}
