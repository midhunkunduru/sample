node("master")
{
    stage("Checkout")
{  
 // properties([
  //parameters([
    //string(name: 'param1', description: 'Possible options: a b c d', defaultValue: ''),
    //string(name: 'param2', description: 'Possible options: e f g h', defaultValue: ''),
    //string(name: 'param3', description: 'Possible options: k l m n', defaultValue: ''),
    //string(name: 'param4', description: 'Possible options: 1 2 3 4', defaultValue: ''),
 // ])
//])  
  echo "Sample checkout project"
    build job: 'parametertest/master', parameters: [string(name: 'Version', value: '1.1'), string(name: 'Application', value: 'html')]
}
    
    stage("Build")
    {
        echo "Sample build"
        build 'multibranch_1/master'
    }

}
