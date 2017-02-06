node {
    stage 'build'
        echo 'Building....'
        sh 'git pull'
    stage 'test'
        echo 'Testing....'
    stage 'deploy'
        echo 'Deploying....'
        sh 'git fetch upstream'
        sh 'git checkout -b prodmaster upstream/master'
        sh 'git merge master'
        sh 'git add .'
        sh 'git commit -a -m "Merging Version"'
}
