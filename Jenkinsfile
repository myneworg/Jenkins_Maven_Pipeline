node ("Windows") {
   // Mark the code checkout 'stage'....
   stage 'Checkout'

   // Get some code from a GitHub repository
   checkout(
     [$class: 'GitSCM',
      branches: [[name: '*/master']],
      browser: [$class: 'GithubWeb', repoUrl: 'https://github.com/myneworg/Jenkins_Maven_Pipeline.git'],
      doGenerateSubmoduleConfigurations: false,
      extensions: [
        [$class: 'CloneOption', depth: 0, noTags: false, reference: '/var/lib/git/mwaite/jenkins/git-plugin.git', shallow: false, timeout: 1],
        [$class: 'CleanBeforeCheckout'],
        [$class: 'PruneStaleBranch'],
        [$class: 'AuthorInChangelog']
      ],
      gitTool: 'Default',
      submoduleCfg: [],
      userRemoteConfigs: [[url: 'https://github.com/myneworg/Jenkins_Maven_Pipeline.git']]
     ]
   )

   }
