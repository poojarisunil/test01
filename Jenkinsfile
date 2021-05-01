node () {

	stage ('maven-build_01_5 - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/poojarisunil/test01.git']]]) 
	}
	stage ('maven-build_01_5 - Build') {
 			
               sh """ cd $WORKSPACE
                      ls -lrta
                      mvn install 
                     """ 
	}
}
