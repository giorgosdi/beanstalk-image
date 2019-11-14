# Elastic Beanstalk base image

The image is kept plain and simple for people who want to work with AWS Elastic Beanstalk. It also serves as a base image for building your Elastic Beanstalk images.

## What's included ?

You can do an apk info if you wish to know all the packges incluced, but the once that are commonly used are described below

```
- docker
- python3
- pip3
- git
- make
- awscli
- ebcli
- jq
```

## awscli v ebcli

The reason both CLIs are included is that `ebcli` is specific to Elastic Beanstalk and can help do things faster. You can find details [here]([https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3.html])

`awscli` is included for those who might need it to describe resources and configure their profiles


## Usage

The image has an `sh` entrypoint so all you need to run is :

`docker run -it giorgosdi/beanstalk:latest`
