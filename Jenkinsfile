pipeline {
agent any
environment {
dotnet = 'C:\\Program Files\\dotnet\\dotnet.exe'
}
stages {
stage('Restore PACKAGES') {
steps {
bat "dotnet restore"
}
}
stage('Clean') {
steps {
bat 'dotnet clean'
}
}
stage('Build') {
steps {
bat 'dotnet build'
}
}
stage('Pack') {
steps {
bat 'dotnet pack --no-build --output nupkgs'
}
}
