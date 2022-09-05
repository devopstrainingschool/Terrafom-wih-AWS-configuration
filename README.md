# Terrafom-wih-AWS-configuration
## I- AWS CLI installation instructions
### Using Linux
```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
```
```
unzip awscliv2.zip
```
```
sudo ./aws/install
```
#### Check if it is installed
```
aws --version
```
### Using Mac Book
```
curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
```
```
sudo installer -pkg AWSCLIV2.pkg -target /
```
#### Check if it is installed
```
aws --version
```
### Usin Windows
```
msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
```
#### Check if it is installed
```
aws --version
```
## II- Configure AWS CLI
### Creating a key pair
Access keys consist of an access key ID and secret access key, which are used to sign programmatic requests that you make to AWS. If you don't have access keys, you can create them from the AWS Management Console. As a best practice, do not use the AWS account root user access keys for any task where it's not required. Instead, create a new administrator IAM user with access keys for yourself.

The only time that you can view or download the secret access key is when you create the keys. You cannot recover them later. However, you can create new access keys at any time. You must also have permissions to perform the required IAM actions. For more information, see Permissions required to access IAM resources in the IAM User Guide.

To create access keys for an IAM user

Sign in to the AWS Management Console and open the IAM console at https://console.aws.amazon.com/iam/.

In the navigation pane, choose Users.

Choose the name of the user whose access keys you want to create, and then choose the Security credentials tab.

In the Access keys section, choose Create access key.

To view the new access key pair, choose Show. You will not have access to the secret access key again after this dialog box closes. Your credentials will look something like this:

Access key ID: AKIAIOSFODNN7EXAMPLE

Secret access key: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY

To download the key pair, choose Download .csv file. Store the keys in a secure location. You will not have access to the secret access key again after this dialog box closes.

Keep the keys confidential in order to protect your AWS account and never email them. Do not share them outside your organization, even if an inquiry appears to come from AWS or Amazon.com. No one who legitimately represents Amazon will ever ask you for your secret key.

After you download the .csv file, choose Close. When you create an access key, the key pair is active by default, and you can use the pair right away.

### Connect my PC to AWS through AWS CLI
```
aws configure
```
```
AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE ( put your here)
AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY  ( put your here)
Default region name [None]: us-east-2
Default output format [None]:
```


