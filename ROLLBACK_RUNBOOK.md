# Kilele Language School — Five-step rollback runbook

**Purpose:** Restore the last known-good GitHub Pages website version after a faulty update.

1. **Detect and record the issue.** Open the live website, confirm the affected page and user-visible failure, note the time and latest change. If sensitive information is exposed, remove or restrict the affected content immediately and alert the site owner.
2. **Identify the last known-good commit.** In the repository, open **Commits** and identify the most recent commit that was verified to work. Record its commit ID and message; do not guess.
3. **Revert the faulty change.** Open the bad commit and choose **Revert**, or create a new commit restoring the previous working files. Prefer a new revert commit to preserve an auditable history; do not force-push or erase history.
4. **Redeploy and test.** Push the revert commit to the configured publishing branch. In **Actions**, wait for the Pages deployment to complete successfully. Test the homepage, registration link, custom 404 URL, mobile layout and affected links.
5. **Document and prevent recurrence.** Record the incident, faulty and rollback commit IDs, recovery time, tests and person notified. Investigate the root cause, review the fix before publishing, and maintain a separate access-controlled backup with tested restoration.

## Safety and operational boundary
GitHub Pages is a public static website host. Do not put student records, uploaded files, credentials or form submissions in this public repository. Store the school's 50 GB student-file workload in private, access-controlled storage with least-privilege access and tested daily backups. Apply an age-appropriate, legally reviewed privacy and guardian-consent process before collecting personal information from learners under 16.
