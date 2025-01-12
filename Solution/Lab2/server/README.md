if using EE
sam build --use-container && sam package  --output-template-file packaged.yaml --s3-bucket serverless-saas-lab2 --region us-west-2
sam deploy --template-file packaged.yaml --config-file samconfig.toml


Normally
sam build -t template.yaml --use-container
sam deploy --config-file samconfig.toml