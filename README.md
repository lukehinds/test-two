# test-one

Contains:
- Dockerfile
- Basic Action `.github/workflows/test.yml`
- Basic Dependabot configuration `.github/dependabot.yml`
```yaml
version: 2
updates:
  - package-ecosystem: "npm"
    directory: "/"
    schedule:
      interval: "weekly"
```

Result should be:

- Dockerfile is flipped
- Basic Action is flipped
- PR is made to add docker and github-action to the dependabot configuration

