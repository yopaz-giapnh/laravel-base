node {
  stage('ls') {
    sh 'ls -la'
  }

  stage('composer_install') {
    // Run `composer update` as a shell script
    sh './composer.phar update'
  }

  stage('database migration') {
    sh 'php artisan migrate'
  }
}