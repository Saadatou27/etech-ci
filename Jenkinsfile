
 pipeline{
      	agent any 
      	tools{}
      	stages{
      		stage('1-gitclone'){
      			steps{
      				sh ' cat /etc/passwd
      				sh 'ls -l'
      			}
      		}
      		stage('2-maven-build'){
      			steps{
      				sh ' mvn package'
      			}
      		}
      		stage('3-mutation-test'){
      			steps{
      				sh '//mutationtestcodes'
      				sh 'bash /var/lib/jenkins/etech-ci/jenkins.sh'
      			}
      		}
      	}
      }
