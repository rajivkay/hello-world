  node {
     git url: 'https://github.com/rajivkay/simple-maven-project-with-tests.git'
     def mvnHome = tool 'M3'
     env.PATH = "${mvnHome}/bin:${env.PATH}"
     bat ""${mvnHome}"\\bin\\mvn -B -Dmaven.test.failure.ignore verify"
     archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
     junit '**/target/surefire-reports/TEST-*.xml'
  }
