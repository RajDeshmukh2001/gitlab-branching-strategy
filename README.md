# GitLab Flow Branching Strategy

This repository demonstrates the **GitLab Flow** branching strategy.
GitLab Flow focuses on **environment-based branching**.

## About the Project
This is a static Library Dashboard built using:
- HTML
- CSS

---

## Branching Model

GitLab Flow uses branches that represent **deployment environments**.

### Environment Branches
- **main**
  - Active development branch
  - All features are merged here first

- **staging (pre-production)**
  - Represents staging or testing environment
  - Used for validation before production

- **production**
  - Represents live production environment
  - Only stable, approved code is merged here

### Other Branches
- **feature/***
  - Created from `main`
  - Used for new features or changes
  - Merged back into `main`

---

## Branch Flow Diagram
```
feature → main → pre-production → production
```


---

## Workflow
1. Develop features on `feature/*` branches
2. Merge features into `main`
3. Promote code from `main` to `pre-production`
4. After validation, promote to `production`

---

## Purpose
- Simulate real-world environment promotion
- Separate development, testing, and production stages
- Reduce risk during deployments

---

## Deployment
Deployments occur from the `production` branch.
