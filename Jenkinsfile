  node {
     git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'
     def mvnHome = tool 'M3'
     env.PATH = "${mvnHome}/bin:${env.PATH}"
     bat "'${mvnHome}\\bin\\mvn' -B verify"
  }
