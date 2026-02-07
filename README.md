 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
new file mode 100644
index 0000000000000000000000000000000000000000..0f1c4573e6296bf5b141068f8de0cc5a64ef3e37
--- /dev/null
+++ b/README.md
@@ -0,0 +1,55 @@
+# AI Calculator
+
+Simple static calculator app with a local "AI Math Helper".
+
+## Push this project to GitHub
+
+If you already created an empty repo on GitHub, run these commands from this folder.
+
+### 1) Check your branch
+
+```bash
+git branch --show-current
+```
+
+### 2) Add your GitHub repo as remote
+
+Replace `<YOUR_GITHUB_USERNAME>` and `<YOUR_REPO_NAME>`:
+
+```bash
+git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO_NAME>.git
+```
+
+If `origin` already exists, update it instead:
+
+```bash
+git remote set-url origin https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO_NAME>.git
+```
+
+### 3) Push your current branch
+
+```bash
+git push -u origin work
+```
+
+If your main branch is `main`, use:
+
+```bash
+git push -u origin main
+```
+
+### 4) Authenticate
+
+When prompted:
+- Username: your GitHub username
+- Password: use a **GitHub Personal Access Token** (not your GitHub password)
+
+Create token: GitHub → Settings → Developer settings → Personal access tokens.
+
+## Optional: deploy quickly with GitHub Pages
+
+After pushing:
+1. Open your GitHub repo.
+2. Go to **Settings → Pages**.
+3. Set **Source** to your branch (`work` or `main`) and folder to `/ (root)`.
+4. Save, then share the generated URL.
 
EOF
)
