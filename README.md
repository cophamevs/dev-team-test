# 🚀 Project Repo

Main repository for dev team collaboration.

## 👥 Team

| Role | Member | Tool |
|------|--------|------|
| Senior Architect | Claude | Claude Code (native GitHub) |
| Full-stack Dev | Opencode | Opencode (native GitHub) |
| Tech Lead/CTO | Bố | Review & Approve |

## 🔄 Development Workflow

### 1. Opencode Implement
```bash
git checkout -b feature/xxx
# Opencode code (trong repo hoặc local)
git push origin feature/xxx
```

### 2. Mở PR
Tạo PR trên GitHub với description rõ ràng.

### 3. Claude Review (Native)
**Comment trong PR:**
```
@claude please review this PR
```
Hoặc:
```
/code-review
```

Claude sẽ:
- ✅ Auto-review với 4 parallel agents
- ✅ Score confidence (≥80% mới comment)
- ✅ Security analysis tự động
- ✅ Suggest fixes hoặc auto-implement

### 4. Fix & Merge
```bash
# Opencode fix hoặc @claude implement
git push
# Bố approve → merge
```

## 🛠️ Native Commands

### Trong GitHub PR:
- `@claude` - Trigger review, answer questions, implement fixes
- `/code-review` - Comprehensive review (4 agents)
- `/security` - Security analysis

### Local Development:
```bash
# Claude Code
claude ~/dev-team/shared/repo

# Opencode  
opencode ~/dev-team/shared/repo
# hoặc
opencode ~/dev-team/opencode
```

## 📋 Guidelines

1. **Opencode:** Focus on implementation (features, bugs, tests)
2. **Claude:** Focus on architecture, review, security
3. **Bố:** Approve PRs khi cả hai đều satisfied

## 🚀 Quick Start

```bash
# Clone repo
cd ~/dev-team/shared/repo
git remote add origin https://github.com/{owner}/{repo}.git

# Làm feature
git checkout -b feature/my-feature
# Code...
git push origin feature/my-feature

# Mở PR và mention @claude để review
```
