node {
    // Ensure the desired Go version is installed
    def root = tool type: 'go', name: 'go-1.16'

    
    withEnv(["GOROOT=${root}", "PATH+GO=${root}/bin"]) {
        sh 'go version'
    }
}
