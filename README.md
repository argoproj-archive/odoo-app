# HOW TO USE

Repo for example stateful app with odoo and workflows

## ASSUMPTIONS:

You have a kubectl installed and configured. You have argo installed and available

### To run:

cd workflows  
argo submit odoo-workflow.yaml 

### To cleanup just the db and application sets:

argo submit odoo-cleanup-workflow.yaml

This will leave the volumes around which can be reused when redeploying again using:

argo submit odoo-workflow.yaml


### To cleanup volumes:

odoo-volume-cleanup-workflow.yaml
