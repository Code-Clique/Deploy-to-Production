# Deploy to Production

### Choose type of deployment:

- [Server](#server)
- [Frontend Service](#frontend-service)


# Server
To deploy an update, simply: 
- Clone the following repo: https://github.com/Code-Clique/Code-Clique-Backend.git
- Make local updates
- Push to the <Strong>main</Strong> branch

Once a push occurs, the code will be automatically deployed to https://code-clique-backend.onrender.com

# Frontend Service

If this is your first time deploying a <Strong>Frontend Service</Strong> please set up <Strong>AWS-CLI</Strong> first.
- Head into your Service's Directory using `cd $YOURPROJECTPATH`
- Run `npm run deploy`
Congratulations, your service has been deployed to production

# AWS CLI
To set up AWS-CLI, simply:
- Download:
  - Windows: https://awscli.amazonaws.com/AWSCLIV2.msi
  - Linux: curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
  - Mac: https://awscli.amazonaws.com/AWSCLIV2.pkg
- To verify your installation: 
  - Run `aws --version` in your shell of choice
  - In case of an Error follow instructions here: https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-troubleshooting.html
- Configure:
  - Run `aws configure` in your shell of choice
  - Fill credentials according to https://github.com/Code-Clique/Secrets/blob/main/.env
  - If a credential does not appear in the file, simply skip it by pressing `Enter`
<b></b>
If you have managed to follow along, congratulations! You have set up AWS-CLI
