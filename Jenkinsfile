@Library('shlib')_
pipeline{
agent any



stages{
stage('Import Data from JSON'){
steps{
fetchvalues()


}
}
stage('Test'){
steps{
rungroovy("${dsl}")
test()
	}}
}
}
