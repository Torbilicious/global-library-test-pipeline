#!groovy

node("master") {

    stage("print test message") {
        new YamlExtractor(this)

        YamlExtractor.doSomething()
    }
}