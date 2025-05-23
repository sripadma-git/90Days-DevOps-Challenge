Day 26 Task: Jenkins Declarative Pipeline

One of the most important parts of your DevOps and CICD journey is a Declarative Pipeline Syntax of Jenkins

Some terms for your Knowledge

What is Pipeline - A pipeline is a collection of steps or jobs interlinked in a sequence.

Declarative: Declarative is a more recent and advanced implementation of a pipeline as a code.

Scripted: Scripted was the first and most traditional implementation of the pipeline as a code in Jenkins. It was designed as a general-purpose DSL (Domain Specific Language) built with Groovy.

Why you should have a Pipeline

The definition of a Jenkins Pipeline is written into a text file (called a Jenkinsfile) which in turn can be committed to a project’s source control repository.
This is the foundation of "Pipeline-as-code"; treating the CD pipeline as a part of the application to be versioned and reviewed like any other code.

Creating a Jenkinsfile and committing it to source control provides a number of immediate benefits:

Automatically creates a Pipeline build process for all branches and pull requests.
Code review/iteration on the Pipeline (along with the remaining source code).
Pipeline syntax
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                //
            }
        }
        stage('Test') {
            steps {
                //
            }
        }
        stage('Deploy') {
            steps {
                //
            }
        }
    }
}
Task-01
- Create a New Job, this time select Pipeline instead of Freestyle Project.
- Follow the Official Jenkins Hello world example
- Complete the example using the Declarative pipeline