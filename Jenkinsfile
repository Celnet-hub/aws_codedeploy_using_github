## Clone your GitHub repository
git clone <GitHub_Repo_Clone_URL>
cd <GitHub_Repo_Name>

## Create a Jenkinsfile
## Replace the label as per your Node label
cat <<EOF > Jenkinsfile
pipeline {
         agent {
                label 'pipeline_demo'
               }
         stages {
                 stage('Build') {
                                steps {
                                    echo 'building your app!'
                                }
                 }
                 stage('Test') {
                                steps {
                                    echo 'testing your app!'
                                }
                 }
                 stage('Deploy') {
                                  steps {
                                        echo 'deploying your app!'
                                  }
                 }
              }
}
EOF
## Push the changes to your GitHub repository
git add Jenkinsfile
git commit -m "pipeline def added"
git push
