node {
    stage 'build'
        echo 'Building....'
        sh 'git clone http://github.com/jpohlmann/pipelinetest ./'
    stage 'test'
        echo 'Testing....'
    stage 'deploy'
        echo 'Deploying....'
        sh 'git remote add upstream http://github.com/jpohlmann/pipelineprod'
        sh 'git fetch upstream'
        sh 'git checkout upstream/master'
        sh 'git merge master'
        sh 'git push upstream'
}
