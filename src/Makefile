#
# This is a psuedo implementation.
# Modify to suit your needs.
#
ami/create:
	cd modules/ec2 && terraform apply

ami/provision: ami/create
	cd playbooks && ansible-playbook ami.yaml

ami/delete:
	cs modules/ec2 && terraform apply

vpc/create:
	cd modules/vpc && terraform apply

vpc/delete:
	cd modules/vpc && terraform destroy

# add additional targets as needed..