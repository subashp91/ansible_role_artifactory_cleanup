# ansible_role_artifactory_cleanup

## **Description:**
Ansible tasks for artefacts cleanup in Jfrog artifactory.


### **Roles**
**artifacts_cleanup** - 
Cleanup artifacts from artifactoy older than specified weeks, months, days, etc.

### **Usage**

``` 
- hosts: all

  vars: 
    artifactory_url: http://jfrog.com/artifactory
    artifactory_username: ''
    artifactory_password: ''
    artifactPath1: ''
    artifactPath2: ''
    artifactRepo: ''
    cleanUpOlderThan: 2w
  roles:
    - { role: ansible_role_artifactory_cleanup }
```

### **Variables and their usage**
-----------------------------------------

| S.No.| Variable | Allowed Values |  Default   | Required  | Remarks |
|------|----------|----------------|------------|-----------|-------|
|1|artifactory_url|String||Yes||
|2|artifactory_username|String||Yes||
|3|artifactory_password|String||Yes||
|4|artifactPath1|String||Yes||
|5|artifactPath2|String||Yes||
|6|artifactRepo|String||Yes||
|7|cleanUpOlderThan|String|2w|Yes| This can be mentioned as in weeks, days, hours, months, etc. |