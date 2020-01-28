@Library('shlib')_
pipeline{
agent any



stages{
/*stage('read Json'){
steps{

json()




}
}








stage('Create job'){
steps{
dsl_script $jobname
}





}*/

stage('Test'){
sh 'curl -O https://repo.jenkins-ci.org/public/org/jenkins-ci/plugins/job-dsl-core/1.76/job-dsl-core-1.76-standalone.jar'
sh 'java -jar job-dsl-core-1.76-standalone.jar dsltest.groovy'
	}
}
}
