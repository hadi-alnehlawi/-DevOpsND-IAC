* Run The Project *
1- install the required network infrastructure first
` aws cloudformation create-stack  --stack-name network --parameters file://network-params.json --template-body  file://network.yaml --capabilities CAPABILITY_NAMED_IAM   --region us-east-1`
2- install the server ec2
`aws cloudformation create-stack  --stack-name server --parameters file://server-params.json --template-body  file://server.yaml  --capabilities CAPABILITY_NAMED_IAM   --region us-east-1`