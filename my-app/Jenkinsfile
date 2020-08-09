node {
        stage('Checkout') {
            git url: 'https://github.com/rajthak/SOAP_Project_Batch2_Rajat_IBM.git',  branch: 'master'
            echo '****************CHECKOUT SUCCESSFUL****************'
        }
       

       
			
	stage('Build') {
		def mvn_version = 'MAVEN_HOME'
		withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"]) {
			sh 'mvn site'
			}
		}
}
