@Library('shlib')_
pipeline{
agent any



stages{
stage('read Json'){
steps{
def props = readJSON file: './sample.json '
def jobname=props.ci.jobs.job.job_name
println(jobname) 




}
}








stage('Create job'){
steps{
dsl_script
}




}
}
}
