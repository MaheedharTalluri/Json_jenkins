@Library('shlib')_
pipeline{
agent any



stages{
stage('Import Data from JSON'){
steps{
importjson()


}
}
stage('Test'){
steps{
rungroovy("${dsl}")
test()
	}}
}
}
