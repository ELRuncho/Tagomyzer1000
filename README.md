# Tagomyzer1000
script for managing aws resources

first install pipenv, then:

```
pipenv install
pipenv run "python Meteors/findMeteors.py"
```

##Snapshotalyzer-3000

Demo script, uses boto3 to manage aws ec2 instances snapshots

###Config

Shotty uses the aws-cli config file. create a profile for shotty:

`aws configure --profile shotty`

###Running

`pipenv run python Snapshotalyzer-3000/shotty.py <command> <subcomand> --project=Project`

*command* is instnaces, volumes or snapshots
*subcommand* - depends on command, use  <command> --help for a list of subcomands
*--project* is optional