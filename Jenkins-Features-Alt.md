# Jenkins-Features-Alt.md

# Jenkins Features, Alternatives, and Job Types

## Features

- **Free & Open Source:** Jenkins is community driven and free.
- **Automated CI/CD:** Automate building, testing, and deployment.
- **Plugins:** 1800+ plugins for tool integration (Git, Docker, AWS, etc.)
- **Pipeline as Code:** Use Jenkinsfile to describe your pipelines, version controlled.
- **User-Friendly GUI:** Visual job creation and tracking.
- **Master-Slave/Agent Architecture:** Distributed builds for scalability.
- **Security:** Role-based access, user login, authentication, and authorization.
- **Ecosystem:** Connects with popular tools (GitHub, Docker, AWS, Kubernetes…)

---

## Alternatives to Jenkins

| Tool          | Highlights                          |
|---------------|-------------------------------------|
| GitHub Actions| Part of GitHub, workflows in YAML   |
| GitLab CI/CD  | Built-in for GitLab                 |
| TeamCity      | JetBrains, easy/UI based            |
| CircleCI      | Cloud-based, fast                   |
| Bamboo        | By Atlassian, Jira/Bitbucket native |
| Travis CI     | Cloud-first, popular for open source|

---

## Jobs in Jenkins

**Job:** A set of automated steps (like build, test, deploy).

**Freestyle Project:**
- Simplest job type
- GUI based, select SCM, configure build/test/deploy without code

**How to Create Freestyle Job**
1. Jenkins Dashboard → New Item
2. Name job, select "Freestyle Project"
3. Add description, configure Git URL, build step (shell or batch command for build)
4. Save and "Build Now" to run

---

**Maven in Jenkins Freestyle**

- Install Maven Integration Plugin (Manage Jenkins > Plugins)
- Global Tool Configuration > Add Maven
- In job, build step: invoke "clean install" or other Maven goals

| Type         | Steps                |
|--------------|----------------------|
| Freestyle    | Manual build scripts |
| Maven        | Direct Maven (pom.xml)|
