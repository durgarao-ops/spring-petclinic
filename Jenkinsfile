node
{
stage ('SCM')
{
git 'https://github.com/durgarao-ops/spring-petclinic.git' //git clone
}

stage ('build the packages')
//build the code
{
sh label: '', script: 'mvn package'
}

stage ('archiving the artifacts')
//artifacts
{
archiveArtifacts 'target/*jar'
}
