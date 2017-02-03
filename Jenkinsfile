node {
    stage 'build'
        echo 'Building....'
        sh 'git pull'
    stage 'test'
        echo 'Testing....'
    stage 'deploy'
        echo 'Deploying....'
        sh 'git fetch upstream'
        sh 'git checkout upstream/master'
        sh 'git merge master'
        sh 'git push upstream'
}
