# Hugo Amplify Test

This repo contains a simple Hugo site which can be deployed to AWS Amplify - check
out this post for more info on the background.

## Install

Clone:

```
git clone https://github.com/seanrmurphy/hugo-amplify-test.git
```

If you want to work with this and AWS Amplify yourself, you should fork this repo
as you will need to commit changes which will get picked up by Amplify.

## Run locally

Prerequisites:
- go toolchain (1.14+ is fine)
- hugo (1.17+ works)

Running the site locally

```
./run-localhost.sh
```

## Deploy to AWS Amplify - main branch

** FIXME **

- You need your own repository - fork this
- Set up application
- Connect to branch main
- Check the build process - the build should fail
- Set up build instructions
- Rebuild the application with the new build instructions
- The application should now build but it should not be possible to see the website
- Add the environment variables - set `HUGO_ENVIRONMENT` to production for the main branch
- Modify the `baseURL` in the `config/production/config.toml` to use the endpoint Amplify has created for this branch
- Commit and push the changes to main branch
- The build should start automatically, it should be successful and now when you go to the endpoint, you should see the content


## Set up staging branch on AWS Amplify

- Add a new branch in Amplify
- Configure the new branch such that  `HUGO_ENVIRONMENT` is staging
- Make a change to the local repository - for example, change the colour of the heading...

