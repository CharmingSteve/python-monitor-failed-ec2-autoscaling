# python-monitor-failed-ec2-autoscaling
script  AWS Outputs failed Autoscaling Groups, can be used with Nagios supporting systems like opsview or Zabbix, likely with many more , as it is just a python script

check_aws_autoscalling --help
usage: check_aws_autoscalling [-h] [--filepath FILEPATH] [--profile PROFILE] [--region REGION] --asg ASG [--time TIME] [--failover FAILOVER] [--multiplier MULTIPLIER]

optional arguments:
  -h, --help            show this help message and exit
  --filepath FILEPATH, -f FILEPATH
                        full path to credentials file
  --profile PROFILE, -p PROFILE
                        AWS Profile Name
  --region REGION, -r REGION
                        AWS Region Name
  --asg ASG, -g ASG     Name of Auto Scaling Group
  --time TIME, -t TIME  minutes back from now
  --failover FAILOVER, -o FAILOVER
                        Failover to ASG
  --multiplier MULTIPLIER, -m MULTIPLIER
                        calculate how many instances of the fail-over ASG will be needed
