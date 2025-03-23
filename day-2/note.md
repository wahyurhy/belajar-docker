# login docker via terminal (local):
`docker login`

# cara agar image yang ada di local (komputer) dijadikan image repository (docker hub)
`docker tag <local-image>:<tagname> <reponame>:<tagname>`

## lalu push dengan cara:
`docker push <reponame>:<tagname>`