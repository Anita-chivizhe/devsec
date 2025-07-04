l - soft links
d - directory
"-" - files
write to hard disk - from ram to hard disk
Ramasamy - Amazon Windows
sudo yum install httpd
sudo service httpd status
sudo service httpd start
cd /var/www/html
sudo vi index.html
esc
type message
esc
sudo chkconfig httpd on

How to check load
top
dd if=/dev/zero of=/dev/null & - increase load (dummy load)

SNS Topic
Create cloud watch alarm
Install cloudwatch agent
Create Lambda function with S3 trigger
