@Library("public@demo") _
import com.microchip.Utilities
precheck                     = [:]
precheck.skip                = false
precheck.linux               = [:]
precheck.linux.server        = "MyLinuxServer"
def utils = new Utilities(this)
pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                 script {
                    utils.notifyPR()
                    utils.pwd()
                    
                    //sendMail("Hello World","ravi.salamani@microchip.com")
                 }
            }
        }
    }
}
