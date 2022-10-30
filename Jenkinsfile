#! Clone your GitHub repository
git clone https://github.com/Celnet-hub/aws_codedeploy_using_github.git
cd aws_codedeploy_using_github

#! Create a Jenkinsfile
#! Replace the label as per your Node label
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
#! Push the changes to your GitHub repository
git add Jenkinsfile
git commit -m "pipeline def added"
git push
