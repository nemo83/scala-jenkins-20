#!groovy

if (env.BRANCH_NAME == "master") {

    node {

        stage 'Checkout'

        checkout scm

        print "I'm on Master, doing the full she-bang!"

        sleep 5

        stage 'Build'

        sleep 5

        input "Release to Canary?"

        input "Release to Production"

    }

} else {

    node {

        stage 'Checkout'

        checkout scm

        print "I'm on a branch, maybe a PR, only running build and tests"

        sleep 5

        stage 'Build'

        sleep 5

    }

}


