# AWS > Amazon GuardDuty

## Amazon GuardDuty 활성화


	{
	    "Version": "2012-10-17",
	    "Statement": [
	        {
	            "Effect": "Allow",
	            "Action": [
	                "guardduty:*"
	            ],
	            "Resource": "*"
	        },
	        {
	            "Effect": "Allow",
	            "Action": [
	                "iam:CreateServiceLinkedRole"
	            ],
	            "Resource": "arn:aws:iam::123456789123:role/aws-service-role/guardduty.amazonaws.com/AWSServiceRoleForAmazonGuardDuty",
	            "Condition": {
	                "StringLike": {
	                    "iam:AWSServiceName": "guardduty.amazonaws.com"
	                }
	            }
	        }
	    ]
	}



![Screenshot 2021-02-17 at 15.13.01](C:/Users/Eden/Desktop/Screenshot 2021-02-17 at 15.13.01.png)