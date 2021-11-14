# python-monitor-failed-ec2-autoscaling
script  AWS Outputs failed Autoscaling Groups, can be used with Nagios supporting systems like opsview or Zabbix, likely with many more , as it is just a python script

check_aws_autoscalling --help
usage: check_aws_autoscalling [-h] [--filepath FILEPATH] [--profile PROFILE] [--region REGION] --asg ASG [--time TIME] [--failover FAILOVER] [--multiplier MULTIPLIER]

optional arguments:</br>
  -h, --help            show this help message and exit</br>
  --filepath FILEPATH, -f FILEPATH</br>
                        full path to credentials file</br>
  --profile PROFILE, -p PROFILE</br>
                        AWS Profile Name</br>
  --region REGION, -r REGION</br>
                        AWS Region Name</br>
  --asg ASG, -g ASG     Name of Auto Scaling Group</br>
  --time TIME, -t TIME  minutes back from now</br>
  --failover FAILOVER, -o FAILOVER</br>
                        Failover to ASG</br>
  --multiplier MULTIPLIER, -m MULTIPLIER</br>
                        calculate how many instances of the fail-over ASG will be needed</br>
