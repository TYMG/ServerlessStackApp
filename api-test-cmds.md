`serverless invoke local --function list --path mocks/list-event.json`

`serverless invoke local --function create --path mocks/create-event.json `

Test the APIs
`npx aws-api-gateway-cli-test --username='admin@example.com' --password=Pass@123 --user-pool-id='us-east-1_en2sxuj7X' --app-client-id='6pbt6in2fkgaklinclqvva6gpa' --cognito-region='us-east-1' --identity-pool-id='us-east-1:18c472c1-90b3-4f1e-8a22-59dbf62d908d'  --invoke-url='https://9uzo1owvnl.execute-api.us-east-1.amazonaws.com/prod' --api-gateway-region='us-east-1' --path-template='/notes' --method='POST' --body='{"content":"hello world","attachment":"hello.jpg"}'`