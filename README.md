#!/usr/bin/env groovy
   
   /**
    * Sample Jenkinsfile for Jenkins2 Pipeline
    * from https://github.com/karunakar999/k123/edit/master/Jenkinsfile
    */
    
    try {
        node {
            stage '\u2776 Stage 1'
            echo "\u2600 BUILD_URL=${env.BUILD_URL}"
    
            def workspace = pwd()
            echo "\u2600 workspace=${workspace}"
    
            stage '\u2777 Stage 2'
        } // node
    } // try end