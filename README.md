# AWS CLI federated (SAML) login tool

based on this https://aws.amazon.com/blogs/security/how-to-implement-federated-api-and-cli-access-using-saml-2-0-and-ad-fs/

## Requirements 

Python 3
The file ~/.aws/credentials must exist and contain a default. For example:

	[default]
	aws_access_key_id = some_stuff
	aws_secret_access_key = some more stuff

## Installation
    pip install -r requirements.txt
-or-   

    pip3 install -r requirements.txt

## Usage
Simplest usage:

    python aws_cli_federation.py
-or-

    python3 aws_cli_federation.py

Alternately define stuff from the cli:

	python aws_cli_federation.py \
	--username your_email@something.org \
	--password your_federated_password_here
	--region us-west-2

## Errata
Bash Completion:
Using the CLI can be frustrating, complete yourself http://docs.aws.amazon.com/cli/latest/userguide/cli-command-completion.html
