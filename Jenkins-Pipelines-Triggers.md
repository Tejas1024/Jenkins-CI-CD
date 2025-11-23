# Jenkins-Pipelines-Triggers.md

# Jenkins Pipeline & Build Triggers – Beginner DevOps

## Pipelines in Jenkins

**Pipeline:** Automated workflow as Groovy code (Jenkinsfile).

**Why?** Repeatable, versioned, less room for manual error.

## Types of Pipeline

### 1️⃣ Declarative Pipeline (Beginner Friendly)

pipeline {
agent any
stages {
stage('Build') {
steps {
echo 'Building...'
}
}
stage('Test') {
steps {
echo 'Testing...'
}
}
stage('Deploy') {
steps {
echo 'Deploying...'
}
}
}
}

 
- `pipeline`: Main block
- `agent any`: Any node/agent can run pipeline
- `stages`: phases (Build, Test, Deploy)
- `steps`: CLI/script steps in a phase (echo = print)

### 2️⃣ Scripted Pipeline (Advanced)

node {
stage('Build') {
echo 'Building...'
}
stage('Test') {
echo 'Testing...'
}
stage('Deploy') {
echo 'Deploying...'
}
}

 

---

## Build Triggers in Jenkins

### **Build Periodically:**
- Use time schedule (like cron) to run builds even if code doesn't change
- Example: Every 5 min:  
  `H/5 * * * *`

### **Poll SCM:**
- Jenkins checks your repo for changes at interval; builds only if code is updated
- Example: Every 5 min:  
  `H/5 * * * *`

**Cron Syntax Recap (Jenkins):**  
( `MIN HOUR DAYMONTH MONTH DAYOFWEEK` )

- `H/5 * * * *` = every 5 minutes (distributed start time)
- `H 0 * * *`  = at midnight

---

## Difference Table

| Trigger Type    | When Runs?              | Condition    |
|-----------------|------------------------|--------------|
| Periodically    | On schedule             | Always runs  |
| Poll SCM        | On schedule if code changes| Code change only |

---

## Key Terms & Summary

- **Pipeline:** Build → test → deploy as code (Jenkinsfile)
- **Declarative:** Beginner-friendly syntax
- **Scripted:** Advanced, more Groovy logic
- **Build Periodically:** Scheduled builds
- **Poll SCM:** Builds only on repo changes