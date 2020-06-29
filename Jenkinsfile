node{
   
   stage('SCM Checkout'){
     git 'https://github.com/vishnu2198/winchester'
   }
   stage('Compile-Package'){
      // Get maven home path
    def mvn_home = 'maven'
    withEnv( ["PATH+MAVEN=${tool mvn_home}/bin"] ) {
     sh "mvn clean install"
    }
   }
}
   
 
