# Ansible_AWS-Infra-Samples

# Using the AWS CLI to Connect Ansible

sudo apt update sudo apt install python3-pip pip3 install awscli

# Once the CLI is installed, run aws configure and enter your AWS access key ID and secret access key.

aws configure cat .aws/credentials

You can get keys from the Your Security Credentials page in the AWS Management Console. Here's how those keys will look (don't get any naughty ideas, these aren't valid):

AccessKeyId: AKIALNZTQW6H3EFBRLHQ SecretAccessKey: f26B8touguUBELGpdyCyc9o0ZDzP2MEUWNC0JNwA

# We're now ready to install ansible
pip3 install ansible

# I'll confirm that it's properly installed by running 
ansible --version. ansible --version

# As I mentioned earlier, Ansible will connect to AWS using the boto SDK.

pip3 install boto boto3

First off, I'll use any plain text editor to create a hosts file.

[local] localhost

There you Go!
