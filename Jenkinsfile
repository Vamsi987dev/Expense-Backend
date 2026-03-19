@Library('Jenkins-shared-library') _

def configMap = [
    Project  : "expense",
    Component: "backend",
    GitRepo  : "https://github.com/Vamsi987dev/Expense-Backend.git",
    Branch   : "${env.BRANCH_NAME}"
]

if(env.BRANCH_NAME != 'main'){   // feature branch pipeline
    nodejsPipeline(configMap)
}
else{
    echo "Follow the process of PROD release"
}