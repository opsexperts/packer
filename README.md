# packer
Automate AMI creation with packer for various cloud providers

# Basic packer commands
packer inspect main.json
packer validate main.json
packer build main.json

# Debug packer code 
packer build -debug main.json

packer passing dynamic valiales 
packer build -var 'aws_access_key=XXXXXX'  -var 'aws_secret_key=test-packer' -var 'version=v01'

# We can define all the variables in a file and parse the file while running packer
packer build -var-file=vars.json

