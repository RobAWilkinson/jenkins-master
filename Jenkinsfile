pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        checkout([
					poll: false,
          $class: 'GitSCM',
          branches: [[name: '*/master']],
          doGenerateSubmoduleConfigurations: false,
          extensions: [[
            $class: 'SubmoduleOption',
            disableSubmodules: false,
            parentCredentials: true,
            recursiveSubmodules: true,
            reference: '',
            trackingSubmodules: true
          ],
          ],
          submoduleCfg: [],
          userRemoteConfigs: []
        ])
      }
    }
	}
}
