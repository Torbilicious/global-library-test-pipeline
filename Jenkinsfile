#!groovy

@Library('Script-test@master')
import net.steinberg.AkamaiUploader

node("master") {

    stage("cleanup") {

        deleteDir()
    }

    stage("print test message") {

        AkamaiUploader uploader = new AkamaiUploader(this)

        String testText = "This is a test message!"
        String fileName = "test.txt"

        writeFile file: fileName, text: testText

        stash includes: fileName, name: "test"

        uploader.deployToAkamai(fileName, false, "test",  "these", "are", "test", "directories")
    }
}
