# docker-slack-invite-automation
Dockerfiles for building a slack-invite-automation image.

## Installation from source
```bash
git clone https://github.com/pilsprog/docker-slack-invite-automation.git
cd docker-slack-invite-automation
docker build -it docker-slack-invite .
vim docker-compose.yml
docker-compose up -d
```

## docker-compose.yml
Very simple docker-compose.yml file to run the container. It contains three
important environment variables that you need to provide in order to run the
slack-invite-automation node application:
```
environment:
  - COMMUNITY_NAME=<your community name>
  - SLACK_URL=<communitysubdomain>.slack.com
  - SLACK_TOKEN=<slack api token>
```
You should obviously replace the `<abc>` with their proper values.
More information can be found in the [slack-invite-automation repo]
(https://github.com/outsideris/slack-invite-automation)


## Bug reports and development

Please create an issue in the [issue tracker](https://github.com/Snorremd/docker-slack-invite-automation/issues)
if you experience any issues with the Dockerfile or docker-compose.yml config file.

Submit a [pull request](https://github.com/Snorremd/docker-slack-invite-automation/pulls)
if you want to contribute code.

## License
The Dockerfile and it's assorted files are licensed under the
