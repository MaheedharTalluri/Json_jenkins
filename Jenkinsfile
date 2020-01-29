@Library('shlib')_
pipeline{
agent any



stages{
stage('Import Data from JSON'){
steps{
script{
	GroovyShell shell = new GroovyShell()
	def tools = shell.parse(new File('a.groovy'))
	xx = tools.dsl
	println(xx) 
}

}
}
stage('Test'){
steps{
//sh 'echo $dsl'
rungroovy("dsltest.groovy")
test()
	}}
}
}
