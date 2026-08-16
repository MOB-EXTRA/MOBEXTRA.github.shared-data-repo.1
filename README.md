# MOBEXTRA.github.shared-data

Centralized shared configuration and data repository for PTB Hub and SlimeSpace. This repository utilizes a multi-push remote configuration to automatically synchronize and update across three separate mirrored GitHub repositories simultaneously, ensuring high availability and protection against bandwidth or rate limits.

---

## Workflow Instructions

1. **Edit Your Files:** Open and modify your code inside your preferred code editor app (saving changes to your local `/storage/emulated/0/Download/MOBEXTRA.github.shared-data` folder).
2. **Push via Termux:** Open Termux and run the following command sequence to stage, commit, and push updates to all three mirrored repositories at once:

```bash
# Navigate to shared data folder
cd /storage/emulated/0/Download/MOBEXTRA.github.shared-data

# Stage all updated files
git add .

# Commit your changes with a descriptive message
git commit -m "Update shared config"

# Push to all 3 repositories simultaneously
git push origin main
