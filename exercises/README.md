# OpenShift Workshop
## Assumption
- You can access your openshift cluster's docker engine
  If so, then among the list of images present are 
    - bcorpusjr/tomcat
    - wkulhanek/gogs:11.4
- If not, do the ff:
    - get inside your cluster's VM
    - or if you're using minishift, simply call minishift ssh
    - or from your host, with a minishift cluster, simply call eval $(minishift docker-env)
    - Once you have the handle of your openshift cluster's docker engine, simply call docker images
    - If you can't see the images listed above, call the ff
        - docker pull bcorpusjr/tomcat
        - docker pull wkulhanek/gogs:11.4

## Contents
- [How to run a docker image in OpenShift](01_run_a_docker_image.md)
- [Adding a Database Using Templates](02_adding_a_database_using_templates.md)
- [Running your own Git Service](03_running_your_own_git_service.md)
- [Using ConfigMaps](04_using_config_maps.md)
- [Using Jenkins Pipeline](05_using_jenkins_pipeline.md)
- [Configure the CI/CD pipeline](06_configure_cicd.md)
