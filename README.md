# Tagomyzer1000
script for managing aws resources

first install pipenv, then:

```
pipenv install
pipenv run "python tagomyzer/tagomyzer.py"
```

###Config

Tagomyzer uses the aws-cli config file. create a profile for tagomyzer:

`aws configure --profile <profile name>`

or use an existing profile

###Running

`pipenv run python tagomyzer/tagomyzer.py <command> <subcomand> --project=Project`

*command* is instances, volumes or snapshots
*subcommand* - depends on command, use  <command> --help for a list of subcomands
*--project* is optional, there are other flags depending on the command/subcomand

###Tagomyzing

You can check first all unused volumes:

`pipenv run python tagomyzer/tagomyzer.py volumes list --unused`

To tagomize volumes use the following command:

`pipenv run python tagomyzer/tagomyzer.py volumes tagomyze`