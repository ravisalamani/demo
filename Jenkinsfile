@Library("public@demo1") _
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
                    def conf=[:]
                    conf.cred="PrecheckInRobot"
                    utils.notifyPR(conf,"Hello","World")
                    utils.pwd()
                    println "Hello World"
                    //sendMail("Hello World","ravi.salamani@microchip.com")
                 }
            }
        }
    }
}
