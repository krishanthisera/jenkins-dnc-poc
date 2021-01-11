node('DOTNETCORE'){
	stage('SCM'){
		checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/krishanthisera/jenkins-dnc-poc.git']]]);
	}
	stage('build'){
		sh 'dotnet build ConsoleApp1'
	}
	stage('push'){
		echo 'Pushing....'
		}
	}
}