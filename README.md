# Duke Cloud Club Zola Personal Website Template 

## Steps
1. https://www.getzola.org/documentation/getting-started/installation/
2. `mkdir <insert name of folder>` -> `cd` -> `zola init`
3. https://www.getzola.org/themes/ -> run git submodule add "this is the github repository for the theme.git"
4. `zola serve` or `zola build` to confirm contents 
5. Create S3 bucket -> note your bucket name in .env file
6. Enable static website hsoitng in properties 
7. Place url in `config.toml` 
8. Create policy in AWS IAM 
9. Copy policy in helper_files -> use your own bucket name 
10. Create a user in AWS IAM to attach policy too
11. Generate access key id and access key secret and copy to .env file 
12. Add all three .env varaibles in your github actions secret 
13. add, commit, push to deploy 

## Future Work 
1. Register your own domain: https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/getting-started-s3.html and https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/domain-register.html
2. Use Cloudfront for faster serving, caching, and https protocol: https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/domain-register.html
3. Try out other services such as Vercel and Github Pages


## References
1. https://www.getzola.org/documentation/deployment/aws-s3/