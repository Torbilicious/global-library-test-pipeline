#!groovy

@Library('Script-test') _

node("master") {

    stage("print test message") {

        new YamlExtractor(this)

        YamlExtractor.printSomething("Test")
        YamlExtractor.doSomething()
    }
}