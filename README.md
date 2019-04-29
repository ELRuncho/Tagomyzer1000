# Tagomyzer1000
script for managing aws resources

first install pipenv, then:

```
pipenv install
pipenv run "python Meteors/findMeteors.py"
```

###Config

Tagomyzer uses the aws-cli config file. create a profile for tagomyzer:

`aws configure --profile Tagomyzer`

or use an existing profile

###Running

`pipenv run python tagomyzer/tagomyzer.py <command> <subcomand> --project=Project`

*command* is instances, volumes or snapshots
*subcommand* - depends on command, use  <command> --help for a list of subcomands
*--project* is optional