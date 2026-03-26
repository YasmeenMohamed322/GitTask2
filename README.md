# Lab 2 - Git & GitHub

## Create Local Repository and Push to Remote

```bash
git init
git add .
git commit -m "Initial commit"

git branch -M main
git remote add origin 
git push -u origin main
```

---

## Create Branches and Add Files

### Create `dev` branch

```bash
git checkout -b dev
git add .
git commit -m "Add dev file"
git push origin dev
```

---

### Create `test` branch

```bash
git checkout main
git checkout -b test
git add .
git commit -m "Add test file"
git push origin test
```

---

## Merge Branches into `main`

```bash
git checkout main

git merge dev
git merge test

git push origin main
```

---

## Delete Branches

### Delete locally

```bash
git branch -d dev
git branch -d test
```

### Delete remotely

```bash
git push origin --delete dev
git push origin --delete test
```

---


## Create Annotated Tag

```bash
git tag -a v1.7 -m "Version 1.7 release"
```

---

## Push Tag

```bash
git push origin v1.7
```

---

## List Tags

```bash
git tag
```

---

## Delete Tag

### Delete locally

```bash
git tag -d v1.7
```


```bash
git push origin --delete v1.7
```
---
