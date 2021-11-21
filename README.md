# ansible-cookbook
Short introduction to Ansible

## Why use Ansible?
- automatizaition repetable task on remote machines, coneccted by ssh protocol
- task or multiple task

## More efficent and less time consuming task
-  execute task from your own machine remotly (instead of ssh into all remote servers one by one)
- Configure/Installation/Deployment steps in a single YAML File (Instead of manual and shell scripts)
- reuse same file multiple times and for different environments
- More reliable and less likley for errors (Instead of human errors)

## Supporting all infrastructure
- from operating system
- cloud provider

## Ansible agentless
- no needed to install anything on remote servers (on which we execute task)
- no agnet/client on remote servers
- manage remote servers remotely by ssh connection
- conclusions:
    - no deployment effort in beginning
    - no upgrade effort

## Ansible modules
- ansible works with modules
- modules equals small programs that do the actual work
- if we have remote servers ansible push module to the target servers, do their work and get removed if done
- module small specific task e.g Install Nginx server, create or copy file
- check module index, list of modules in Ansible Official Documentation

## Modules ar granual and sepcific
- multiple modules
- in a certain sequence
- grouped toghether

## Ansible uses YAML
- ansible uses YAML file for configuration task/modules

## Ansible Playbooks
- configuration in yaml file with module name, arguments, desciprion task
- can be execute multiple modules in a sequence
- host attribute means where shoulde these task executes
- remote_user means with wihich user should the tasks execute
- uses variables for repeating values, with vars atributte
- 'Play' means which task, which host, which user
- 'Playbook' can contain one or more plays
- 'Playbook' orchestrates the module execution
- 'Playbook' describes: how an in which order, at what time and where, what shoulde be executed
- name 'Playes' it's good practice

## Ansible Inventory list
- contain etc. host values from 'Play'
- Inventory means all the machines involved in task execution
- Contain IP address or hostname, cloud servers, virtual or bare metal servers

## Ansible for Docker ?
 

## Ansible Tower
- UI dashbord for REd Hat
- cenytral store automation task
- across teams
- configure permissions
