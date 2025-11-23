# Jenkins-Maven-Jobs.md

# Jenkins CI/CD with Maven – Freestyle & Maven Project Types

## Maven + Freestyle Project

1. Install Maven plugin in Jenkins.
2. Add Maven (Global Tool Config) with name and path or auto-install option.
3. Create "Freestyle Project" > Build Step: add shell or batch with `mvn clean install` or `mvn package`.
4. Save and "Build Now" to produce build.

- For Git projects, clone in build step or set Git URL in SCM section.

---

## Maven Project in Jenkins (Direct & Smarter)

1. Jenkins Dashboard → New Item → type "Maven project"
2. Set SCM to Git, give repo URL and branch name
3. Set Root POM: `pom.xml`
4. Set Goals: `clean package` or any other Maven targets
5. Save, Build Now

---

## Hands-On Checklist

- Install Jenkins
- Create Freestyle and Maven jobs
- Connect Git repo via SCM
- Automate builds with Maven ("clean install")

---

| When to Use         | Example Command   | How to Set                           |
|---------------------|------------------|--------------------------------------|
| Freestyle Project   | mvn clean install| Add "Execute Shell"/"Batch" step     |
| Maven Project       | clean package    | Set goals directly in Maven project  |
