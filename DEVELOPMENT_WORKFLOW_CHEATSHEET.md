# 🚀 Development Workflow Cheat Sheet

## **🎯 Core Setup Summary**
- **VS Code:** Optimized with 6 essential extensions
- **PowerShell:** 7.5.2 Core with perfect shell integration
- **Git:** Full version control with GitHub backup
- **Projects:** Organized in `cline-projects/` directory

---

## **🔧 Essential Extensions & Usage**

### **Automatic Extensions (No Action Required)**
- **🤖 Cline** - AI Development Partner (just talk naturally)
- **🎨 Prettier** - Auto-formats code on save (Ctrl+S)
- **📖 GitLens** - Shows Git history visually (just observe)

### **Interactive Extensions (Occasional Use)**
- **📁 Project Manager** - `Ctrl+Alt+P` to switch projects
- **🌐 Live Server** - Right-click HTML → "Open with Live Server"
- **🔌 REST Client** - AI-managed API testing

---

## **🤖 AI Collaboration Best Practices**

### **Starting New Projects**
```
"Create a [type] project with [requirements]"
Example: "Create a portfolio website with dark theme and contact form"
```

### **Getting Project Status**
```
"Give me a project status: what's incomplete, what needs attention, 
what improvements do you see, and what questions do you have?"
```

### **Making Changes**
```
"Add [feature] to the [component]"
"Fix the [issue] in [location]"
"Optimize [specific area] for better [performance/UX/etc]"
```

### **When to Use Plan Mode vs Act Mode**
- **Plan Mode:** Discussing approach, brainstorming, planning
- **Act Mode:** Actually building, coding, implementing

---

## **💾 Version Control & Backup**

### **Quick Repository Status Check**
```powershell
# Run from cline-projects/ directory
Get-ChildItem -Directory | ForEach-Object { 
    Write-Host $_.Name -ForegroundColor Yellow; 
    cd $_.FullName; 
    git status --porcelain; 
    cd .. 
}
```

### **Standard Git Workflow (VS Code)**
1. **Make changes** to your project
2. **Open Source Control** (`Ctrl+Shift+G`)
3. **Stage changes** (click + next to files)
4. **Write commit message** (describe what you did)
5. **Commit** (click checkmark)
6. **Sync Changes** (push to GitHub)

### **Your GitHub Repositories**
- `dev-setup-docs` - Setup documentation and guides
- `hello-cline-demo` - Basic demo project template
- `workflow-test` - Testing repository
- `setup-verification-test` - Completed setup verification

---

## **🚦 Project Startup Routine**

### **New Project Checklist**
1. **Create directory** in `cline-projects/`
2. **Open in VS Code** (or use Project Manager)
3. **Tell AI your project goals** clearly
4. **Initialize Git** when ready (`git init`)
5. **Create GitHub repo** when you want backup
6. **Set up Live Server** for web projects

### **Switching Between Projects**
- **Quick Switch:** `Ctrl+Alt+P` → Select project
- **New Terminal:** Projects use separate terminals automatically
- **Git Context:** Each project has independent Git status

---

## **⚡ Key Shortcuts & Commands**

### **Essential VS Code Shortcuts**
- `Ctrl+Alt+P` - Project Manager (switch projects)
- `Ctrl+Shift+G` - Source Control (Git)
- `Ctrl+S` - Save (triggers auto-formatting)
- `Ctrl+Shift+X` - Extensions panel
- `Ctrl+`` - Toggle terminal

### **File Management**
- **Auto-save:** Enabled (1 second delay)
- **Format on save:** Enabled (code cleans up automatically)
- **Git tracking:** Automatic (shows file changes)

---

## **🎨 Web Development Workflow**

### **HTML/CSS/JS Projects**
1. **Create files** via AI or manually
2. **Right-click HTML file** → "Open with Live Server"
3. **Make changes** → Browser auto-refreshes
4. **Code auto-formats** when you save

### **API Development**
1. **Create backend** via AI assistance
2. **Use REST Client** for testing endpoints
3. **Test via browser** or Live Server for frontend

---

## **🔍 Troubleshooting & Maintenance**

### **If Something Breaks**
1. **Check Git status** first (might be uncommitted changes)
2. **Ask AI:** "What's wrong with [specific issue]?"
3. **Restart VS Code** if extensions acting up
4. **Check terminal output** for error messages

### **Regular Maintenance**
- **Weekly:** Run backup status check command
- **Monthly:** Review and clean up old test projects
- **As needed:** Update extensions (VS Code handles automatically)

---

## **💡 Pro Tips**

### **AI Communication**
- **Be specific** about requirements and goals
- **Ask for status updates** regularly during development
- **Use "new task" tool** when context gets heavy (50-70% full)
- **Describe problems clearly** rather than trying to fix code yourself

### **Project Organization**
- **One project = One directory** in cline-projects/
- **Use descriptive names** for easy Project Manager navigation
- **Keep test/demo projects** separate from real work
- **Regular GitHub sync** prevents data loss

---

## **🏁 Ready to Build!**

**Your setup is production-ready. Start your first project by saying:**

*"Create a [project type] with [your requirements]. Set up the basic structure and let me know what questions you have."*

**Remember:** You're the architect - give high-level direction and let the AI handle the technical implementation!
