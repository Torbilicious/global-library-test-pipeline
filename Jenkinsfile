#!groovy

node("master") {

    stage("print test message") {
        new YamlExtractor(this)

        YamlExtractor.printTest("This is a test message")
    }
}