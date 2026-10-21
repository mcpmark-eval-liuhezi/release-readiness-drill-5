# Release Sign-Off Audit Checklist

This checklist is walked through by the release manager before any release is shipped.
Every item must be verified and initialed by the responsible owner.

## 1. Scope and Contents
- [ ] Release version tag identified and matches the release plan
- [ ] Scope of included changes documented in the release notes draft
- [ ] Breaking changes called out explicitly and migration steps written

## 2. Code and Change Management
- [ ] All planned pull requests merged into the release branch
- [ ] No unreviewed or unapproved commits on the release branch
- [ ] Release branch is forked from a known-good commit of the default branch

## 3. Build and Quality Gates
- [ ] CI pipeline green on the release commit SHA
- [ ] Test suite passed, including integration and smoke tests
- [ ] Static analysis / lint checks reported no new findings
- [ ] No open critical or high severity code scanning alerts

## 4. Security Review
- [ ] No open critical or high severity Dependabot alerts
- [ ] Secret scanning shows no unresolved alerts
- [ ] Security review sign-off obtained from the security owner

## 5. Release Readiness
- [ ] Release notes drafted, reviewed, and ready to publish
- [ ] Rollback / revert plan documented and tested
- [ ] On-call and support teams notified of the release window
- [ ] Communications plan for customers agreed (if applicable)

## 6. Sign-Off
- [ ] Release manager sign-off recorded in this checklist
- [ ] Engineering lead sign-off recorded
- [ ] Final decision (ship / hold / abort) logged with rationale and timestamp
