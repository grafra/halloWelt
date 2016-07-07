#!groovy

stage 'Build it'
node {
   checkout([$class: 'SubversionSCM', 
        additionalCredentials: [], 
        excludedCommitMessages: '', 
        excludedRegions: '', 
        excludedRevprop: '', 
        excludedUsers: '', 
        filterChangelog: false, 
        ignoreDirPropChanges: false, 
        includedRegions: '', 
        locations: [[credentialsId: 'e19aa2f9-56d0-4065-aaa2-3868f08b04c1', 
                      depthOption: 'infinity', 
                      ignoreExternalsOption: true, 
                      local: '.',
                      remote: 'https://absvn.pass-consulting.com/svn/VSF/Libraries/Internal/PASS_Common/branches/r1.4/']], 
                      workspaceUpdater:
                      [$class: 'UpdateUpdater']])
             
                      
   withEnv ([ "PATH+MAVEN= ${tool 'Maven 3.3.9'}/bin" ])
   {
        println "PATH ${env.PATH}"
   }
  
  
}


stage 'XXXX'
node {
 
   echo 'Hello World 2'
}