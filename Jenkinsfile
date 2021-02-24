#!/usr/bin/env groovy

@Library('pipeline-library-demo@master')_ //master or whatever branch

pipeline{

      agent { label 'master' }
        
        stages{        
                 stage ('Check logs') {
                    steps {
                        helloWorld ()
                    }
                }
		
           }	       	     	         
}
