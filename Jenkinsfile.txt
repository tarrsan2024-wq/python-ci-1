pipeline
{
agent any
stages{

stage('Checkout Code'){
steps{
git 'https://github.com/tarrsan2024-wq/python-ci-1'
}
}

stage('Build'){
steps{
sh 'echo "10\n20" | python3 app.py'
}
}
}
}