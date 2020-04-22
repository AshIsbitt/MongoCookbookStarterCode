# Mongo Cookbook Starter Code

The purpose of this repo is to be a basic installation of MongoDB within a chef recipe, with all tests passing and preparred for installation to AWS.

## Prerequisites

- gnupg
	- `sudo apt-get install gnupg`
- Chef

## Installation

To download this repo, run `git clone git@github.com:AshIsbitt/MongoCookbookStarterCode.git`

## Chef

**Chef** is a configuration management tool, allowing for creation of instrastructure as code, allowing for creation and deployment of infrastructure such as an Amazon Web Service instance quickly and easily using a recipe. 

This reveals a number of benefits, such as identical servers (decreasing the "this works on my machine" type of errors), as well as speedy deployment and easy maintainence, as multiple servers are all managed by at most a handful of files. 

Chef server configs can be easily tested within a CLI wth only a few commands: `chef exec rspec` can be used to run a spec test on your recipe, double checking that each test written has an analogous line of code within the recipe (an example of Test Driven Development in action), and then `kitchen test` or `kitchen verify` can be used to make sure that each line of code in the recipe actually passes. 