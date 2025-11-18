# Terraform state

## Delete all ressources of a ressource

` terraform state rm -dry-run $(terraform state list | grep ressource-to-delete\") `
