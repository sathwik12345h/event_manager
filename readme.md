# Event Manager API

This repository contains the backend API for managing events, developed in Python and designed for seamless Docker deployment and CI/CD automation.

## Features

- Docker image is automatically built and pushed to [Docker Hub](https://hub.docker.com/repository/docker/sathwiks12/wis_club_api/general) using GitHub Actions after every push to the `main` branch.
- All tests pass using `pytest`.
- Code coverage is at 92% using `pytest-cov`.
- GitHub Actions CI pipeline includes:
  - `test`: Executes unit tests with coverage.
  - `build-and-push-docker`: Builds the Docker image and pushes it to Docker Hub if tests pass.

## Development and Contributions

Development was managed using issues, feature branches, and pull requests. All issues and pull requests have been resolved and merged into `main`.

### Issues

- [#1 mismatch-name](https://github.com/sathwik12345h/event_manager/issues/1) – Resolved name mismatch in the API responses.
- [#3 name-validator](https://github.com/sathwik12345h/event_manager/issues/3) – Added validation logic for user names.
- [#5 different names](https://github.com/sathwik12345h/event_manager/issues/5) – Ensured different names are handled properly in user data.
- [#7 data mismatch in API](https://github.com/sathwik12345h/event_manager/issues/7) – Fixed inconsistencies in API data formats.
- [#9 passwords](https://github.com/sathwik12345h/event_manager/issues/9) – Fixed issues related to password handling and security.
- [#11 profile image](https://github.com/sathwik12345h/event_manager/issues/11) – Addressed bugs in profile image processing.

### Pull Requests

- [#2 fixed name mismatch](https://github.com/sathwik12345h/event_manager/pull/2) – Implemented the fix for name mismatches.
- [#4 added name validator](https://github.com/sathwik12345h/event_manager/pull/4) – Introduced a validator for names.
- [#6 making sure we have different names](https://github.com/sathwik12345h/event_manager/pull/6) – Added logic to handle uniqueness in names.
- [#8 api fixes](https://github.com/sathwik12345h/event_manager/pull/8) – Fixed various API-level issues and mismatches.
- [#10 added a password fix](https://github.com/sathwik12345h/event_manager/pull/10) – Implemented secure password fixes.
- [#12 profile image fixes](https://github.com/sathwik12345h/event_manager/pull/12) – Final fixes for profile image logic and endpoint behavior.

## Branches Used

Each pull request was developed on its own branch, including:

- `1-mismatch-name`
- `3-name-validator`
- `5-different-names`
- `7-data-mismatch-in-api`
- `9-passwords`
- `11-profile-image`

These branches have all been merged into `main`.

---

This project demonstrates automated Docker deployments, test-driven development, and structured GitHub workflow using issues and pull requests. All features are live and reflected in the main branch and Docker Hub.

---

## Summary

Working on this assignment from a QA perspective was both challenging and rewarding. Going step by step through the user lifecycle in the event manager application really helped me get a solid understanding of how the system works. Identifying issues and figuring out how to fix them gave me a chance to explore the codebase deeply and either write new functions or make better use of the existing ones.

I also really enjoyed working with Docker Compose. It was interesting to see how different services interact over an internal network and to learn how to resolve internal hostnames—especially when connecting to PostgreSQL through pgAdmin. It gave me a clearer picture of how containerized applications come together.

Writing thorough test cases for new logic and improving the overall test coverage pushed me to explore parts of the code I might have otherwise missed. By the time I wrapped up the assignment, I felt confident navigating the codebase and knew exactly where to make changes when something needed fixing.

