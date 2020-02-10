node {
  stage('clone source code') {
    git url: 'git@gitlab.com:gaha/laravelbase.git'
  }

  stage('composer_install') {
    // Run `composer update` as a shell script
    sh './composer.phar update'
  }

  stage('database migration') {
    sh 'php artisan migrate'
  }
}