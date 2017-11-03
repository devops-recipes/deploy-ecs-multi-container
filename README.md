# Deploy a Node.js application to Amazon ECS

[![Run Status](https://api.shippable.com/projects/58f98b298c0a6707003b237a/badge?branch=master)](https://app.shippable.com/github/devops-recipes/deploy-ecs-multi-container) [![Coverage Badge](https://api.shippable.com/projects/58f98b298c0a6707003b237a/coverageBadge?branch=master)](https://app.shippable.com/github/devops-recipes/deploy-ecs-multi-container)

![AyeAye](https://github.com/devops-recipes/deploy-ecs-multi-container/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha
and istanbul. It also does a docker build once CI passes and then pushes the image
to Amazon ECR.

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](wwww.shippable.com)
* Create an [integration](http://docs.shippable.com/platform/integration/aws-keys/) on shippable to your Amazon ECR
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `dr-aws-keys`
* Change the ECR_REPO to point to your repo and aws account
* You should be able to run a manual build or webhook build on commit

## CI Reports on Shippable

### CI Integration View
![CI Integration View](https://github.com/devops-recipes/deploy-ecs-multi-container/blob/master/public/resources/images/integration.jpg)

### CI Console Output
![CI Console Output](https://github.com/devops-recipes/deploy-ecs-multi-container/blob/master/public/resources/images/console.jpg)
