/**
* Android Jenkinsfile
*/
node("master"){
  stage("Checkout"){
    checkout scm
  }

  stage("Build"){
    sh 'chmod +x ./gradlew '
    sh " ${params.buildShell} "
  }

 /*stage("Archive"){
    if (params.buildType == 'release') {
        archiveArtifacts artifacts: 'app/build/outputs/apk/release/app-release.apk', excludes: 'app/build/outputs/apk/*-unsigned.apk'
    } else {
        archiveArtifacts artifacts: 'app/build/outputs/apk/debug/app-debug.apk', excludes: 'app/build/outputs/apk/*-unsigned.apk'
    }
  }*/
  
  
}
