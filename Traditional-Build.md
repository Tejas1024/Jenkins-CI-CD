# Traditional-Build.md

# 🧩 Traditional Build and Release Process

## How It Worked Before Jenkins (Manual Process)

1. Developers wrote code and passed it to the Build Engineer.
2. Build Engineer manually compiled and packaged the code ("build").
3. The build was deployed on a Testing Server for QA/testing.
4. If tests passed, the Release Engineer manually moved the build to Production Server.
5. Bugs or fixes required code to be sent back and the whole cycle repeated (all manually).

### Drawbacks

- Time-consuming (many manual handoffs)
- Lots of manual labor and human error
- Slow delivery and low productivity
- Delayed feedback on build/test failures

**Automation (like Jenkins) was needed to speed up, reduce errors, and give faster feedback.**

