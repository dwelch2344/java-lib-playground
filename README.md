


# Iterating on build

git commit --amend --no-edit -a; git push -f; gh workflow run --ref spring_boot_lib publish.yml;  sleep 2; gh run list --json url --workflow=publish.yml | jq -r '.[0].url' | xargs open  
