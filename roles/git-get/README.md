# git-get 
This role will fecth the required git repo and create a zip archive on the Ansible server. 
This archive can be then accessed by other roles for upload to destination.
_*This could have been done the target servers but then it would introduce the dependency of git being installed on the target server.*_ 

Variables expected by the role. 
```
git_url: 'https://some_url/some_repo.git'
git_branch: 'master'
upload_location: '/roles/cp_code/files/code.zip 
```

## To-do 
The name of the archive being created is hard coded to `code.zip` look into making this a variable with register and passing this to the playbook so that we dont have to hard code the location and file name to other pass palybooks.
Use date and time to create a tmp file name and store in /tmp other roles to use this variable file name. 
