node {
    stage 'build'
        echo 'Building....'
        sh 'cd ../workspace@script'
    stage 'test'
        echo 'Testing....'
    stage 'deploy'
        echo 'Deploying....'
        sh 'git remote add upstream http://github.com/jpohlmann/pipelineprod'
        sh 'git checkout upstream/master'
        sh 'git merge master'
        sh 'git push upstream'
}
