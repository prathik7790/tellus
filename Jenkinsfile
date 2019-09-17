properties([
    parameters([
        gitParameter(branch: '',
                     branchFilter: 'origin/(.*)',
                     defaultValue: 'master',
                     description: 'Parameterizing branch name',
                     name: 'BRANCH',
                     quickFilterEnabled: false,
                     selectedValue: 'NONE',
                     sortMode: 'NONE',
                     tagFilter: '*',
                     type: 'PT_BRANCH')
    ])
])
node {
    git branch: "${BRANCH}", url: 'https://github.com/prathik7790/tellus.git'
}
stage('Code checkout'){
  checkout scm
}
stage('Test'){
  echo 'Hello'
}

//node {
 // echo 'Hello World'
  //stage('Code Checkout')
  //checkout scm
  //stage('Test')
  //echo 'Hello'
//}
