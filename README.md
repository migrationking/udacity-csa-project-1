**Udacity CSA Project 1**

**Corrections/Amendments to the Udacity Instructions for things that were missing and I had to figure out on my own:**

SSH to the instance and connect to the read replica database. (*Highly suggest learning on your own but this is what I learned when I got stuck and it is a general guide only. Don't cheat.)

3a. Example ssh command for Amazon Linux 2: ssh -i "kp-udacity-p1.pem" ec2-user@ec2-34-224-80-144.compute-1.amazonaws.com Note: Make sure you in the same directory of the key file or you type the path.

3b. MySql is not installed by default. Enable MySql by running "sudo yum install mysql -y"

3c. mysql -h udacity.ctx2m04ir1m9.us-east-1.rds.amazonaws.com -u admin -p (type the password that you created) The udacity.ctx... dns name is found under RDS connectivity and security. What a bugger this was if you don't know.

Verify if you are not able to insert data into the database but are able to read from the database. 4a. Super Helpful YouTube video: https://www.youtube.com/watch?v=XJ7dlwHuVUk 4b. Read the Docs! https://dev.mysql.com/doc/refman/8.0/en/creating-tables.html

You have now demonstrated that you can only read from the read replica database.

Also, on the S3 Bucket. You have to use the Object Lock option or just deleting the object will not allow it to be recovered from versioning.
