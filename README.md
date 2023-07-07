# ZimPay Documentation: Pull Requests

## Introduction
This documentation provides an overview of how Pull Requests (PRs) work in the collaborative project called ZimPay. ZimPay is a project where we use Slack for communication and collaboration. We follow a specific naming convention for branches related to features and bugs.

## What is a Pull Request?
A Pull Request is a feature provided by version control systems like Git, which allows developers to propose and review changes made to a codebase. It serves as a mechanism for collaboration and code review before merging changes into the main branch.

## Using Pull Requests in ZimPay
In ZimPay, we utilize Pull Requests to manage the process of proposing, reviewing, and integrating changes. The following guidelines outline how we use Pull Requests effectively:

## Branch Naming Convention
For features, we create branches using the format feature/#ticketid. For example, feature/#123 would be used for a feature related to ticket number 123.
For bug fixes, we create branches using the format bugfix/#ticketid. For instance, bugfix/#456 would be used for fixing the issue mentioned in ticket number 456.

## Creating a Pull Request
1. When working on a new feature or addressing a bug, create a new branch from the main branch using the following command:
   ```bash
    git checkout -b feature/#ticketid
   ```
   Replace #ticketid with the actual ticket number.
   
2.Commit your changes to the branch regularly, providing meaningful commit messages that describe the purpose of each change. Use the following commands:
   ```bash
    git add .
    git commit -m "Add feature implementation"
   ```
3.Once you have completed the work on the branch, push it to the remote repository using the following command:
   ```bash
    git push origin feature/#ticketid
   ```
4.On GitHub, navigate to the repository and click on the "Pull Requests" tab.

5. Click on the "New pull request" button and specify the source branch (the one containing your changes) and the target branch (usually the main branch).
6. Provide a descriptive title and description for the Pull Request, highlighting the changes made and any relevant information.

 ## Reviewing a Pull Request
 Slack Integration: A notification will be sent to the designated Slack channel whenever a new Pull Request is created.
 
 Reviewers can access the Pull Request on GitHub, review the code changes, and provide comments or feedback directly in the Pull Request's conversation thread.
 
 Reviewers should ensure that the proposed changes conform to coding conventions, best practices, and requirements outlined by the project.
 
 If necessary, reviewers can request modifications or further clarification from the author of the Pull Request.
 
## Merge and Close
Once the Pull Request has been reviewed, approved, and all discussions are resolved, it can be merged into the main branch.

The author of the Pull Request is responsible for merging the changes after ensuring that the branch is up to date with the target branch. Use the following commands:
```bash
git checkout main
git pull origin main
git merge feature/#ticketid
```
After merging, the Pull Request can be closed, indicating that the changes have been successfully integrated into the codebase.

By following this process, we ensure that changes introduced to ZimPay undergo thorough review and verification before being merged, thereby maintaining code quality and minimizing the risk of introducing errors or regressions.

Please refer to the ZimPay Contribution Guidelines for more details on our collaborative development process.

For any further questions or assistance, feel free to reach out to the team on Slack or consult with the project maintainers. Happy coding!





