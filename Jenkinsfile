#!groovy

@Library('Script-test@master')
import net.steinberg.YamlExtractor

node("master") {

    stage("print test message") {

        YamlExtractor extractor = new YamlExtractor(this)

        YamlExtractor.printSomething("Test")
        YamlExtractor.doSomething()
    }
}