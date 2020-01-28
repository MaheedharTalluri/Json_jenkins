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
steps{
sh 'curl -O https://repo.jenkins-ci.org/public/org/jenkins-ci/plugins/job-dsl-core/1.76/job-dsl-core-1.76-standalone.jar'
sh 'java -jar job-dsl-core-1.76-standalone.jar dsltest.groovy'
scripts{
curl -s -XPOST 'http://3.134.110.122:8080/createItem?name=job' -u admin:1166851f05c42cf7f533e59eac3819e43d --data-binary @Test.xml -H "Content-Type:text/xml"
}	}}
}
}
