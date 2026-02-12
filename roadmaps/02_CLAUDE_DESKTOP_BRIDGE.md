# 📘 Claude Desktop App Bridge Guide

**Version**: 1.0  
**Last Updated**: February 2, 2026  
**Target Audience**: Non-technical founder transitioning from web-based to desktop development  
**Estimated Time**: 30-45 minutes for complete setup  
**Purpose**: Leverage Claude Desktop App for professional Life Ninja V3 development

---

## 🎯 What You'll Achieve

By the end of this guide, you'll be able to:
- ✅ Use Claude Desktop App with Code capabilities
- ✅ Maintain persistent project memory across sessions
- ✅ Integrate Claude with your GitHub repository
- ✅ Use Plan, Ask, and Code modes effectively
- ✅ Create and use custom skills for Life Ninja
- ✅ Never lose context between development sessions
- ✅ Develop faster with agentic coding assistance

---

## 🤔 Part 1: Understanding Claude Desktop App (10 minutes)

### What Is Claude Desktop App?

**Simple Explanation:**
Claude Desktop App is like having a senior developer sitting next to you on your computer, with the ability to:
- Read and edit your files
- Run commands
- Remember your project across sessions
- Plan complex features before coding
- Execute development tasks autonomously

**Analogy:**

| Web-Based Claude | Claude Desktop App |
|-----------------|-------------------|
| Phone call with developer | Developer working at your desk |
| Must copy/paste code | Directly edits your files |
| Forgets between sessions | Remembers your project |
| One conversation at a time | Persistent workspace |
| Limited to chat | Can Plan, Ask, and Code |

---

### Key Differences from Web-Based Claude

```
┌─────────────────────────────────────────────────────────┐
│  WEB-BASED CLAUDE (claude.ai)                           │
├─────────────────────────────────────────────────────────┤
│  ✓ Great for planning and questions                    │
│  ✓ Good for generating code snippets                   │
│  ✗ Can't edit files directly                           │
│  ✗ You must copy/paste everything                      │
│  ✗ Loses context in new conversations                  │
│  ✗ No direct GitHub integration                        │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  CLAUDE DESKTOP APP                                     │
├─────────────────────────────────────────────────────────┤
│  ✓ All web features PLUS:                              │
│  ✓ Direct file editing                                 │
│  ✓ Computer use (bash commands, file operations)       │
│  ✓ Project memory (persistent context)                 │
│  ✓ GitHub integration via file system                  │
│  ✓ Plan → Ask → Code workflow                          │
│  ✓ Skills and patterns library                         │
└─────────────────────────────────────────────────────────┘
```

---

### The Three Modes: Plan, Ask, Code

**1. PLAN Mode** 🗺️
- **Use for**: Strategic thinking, architecture decisions
- **Example**: "Plan the migration from monolith to modular architecture"
- **Output**: Detailed plan with phases, risks, milestones
- **No code execution**: Just thinking and planning

**2. ASK Mode** 💬
- **Use for**: Questions, clarifications, debugging help
- **Example**: "Why is my search field requiring multiple clicks?"
- **Output**: Explanation, analysis, recommendations
- **No code changes**: Just conversation

**3. CODE Mode** 💻
- **Use for**: Implementing features, fixing bugs, refactoring
- **Example**: "Fix the search field continuous typing bug"
- **Output**: Actual file changes in your repository
- **Direct file editing**: Claude modifies your code

**Visual Workflow:**
```
┌─────────────────────────────────────────────┐
│  YOUR DEVELOPMENT FLOW                      │
├─────────────────────────────────────────────┤
│                                             │
│  "I want analytics dashboard"              │
│         │                                   │
│         ▼                                   │
│  PLAN: How should we build this?           │
│         │                                   │
│         ▼                                   │
│  [Claude creates detailed plan]            │
│         │                                   │
│         ▼                                   │
│  ASK: Any questions about the plan?        │
│         │                                   │
│         ▼                                   │
│  [You ask clarifications]                  │
│         │                                   │
│         ▼                                   │
│  CODE: Implement the analytics dashboard   │
│         │                                   │
│         ▼                                   │
│  [Claude edits your files]                 │
│         │                                   │
│         ▼                                   │
│  Review in GitHub Desktop → Commit         │
│                                             │
└─────────────────────────────────────────────┘
```

---

### Project Memory: The Game Changer

**What is Project Memory?**

In web-based Claude, each new chat starts fresh. In Claude Desktop App with Projects:

```
Traditional Way (Web):
┌──────────────┐ ┌──────────────┐ ┌──────────────┐
│ Chat 1:      │ │ Chat 2:      │ │ Chat 3:      │
│ "Fix bug A"  │ │ "Fix bug B"  │ │ "Fix bug C"  │
│              │ │              │ │              │
│ ❌ Forgets   │ │ ❌ Forgets   │ │ ❌ Forgets   │
│ everything   │ │ Chat 1       │ │ Chats 1 & 2  │
└──────────────┘ └──────────────┘ └──────────────┘

Desktop App Way (Projects):
┌────────────────────────────────────────────┐
│ PROJECT: Life Ninja V3                     │
├────────────────────────────────────────────┤
│ ✓ Remembers all features                  │
│ ✓ Remembers your architecture decisions   │
│ ✓ Remembers bug history                   │
│ ✓ Remembers coding patterns you prefer    │
│ ✓ Accumulates knowledge over time         │
│                                            │
│ Every conversation builds on the last!    │
└────────────────────────────────────────────┘
```

---

## 🚀 Part 2: Installing Claude Desktop App (10 minutes)

### Step 1: Download Claude Desktop App

**Action:**
1. Open your web browser
2. Go to: https://claude.ai/download
   - Or google "Claude Desktop App download"

**What You'll See:**
```
┌─────────────────────────────────────────┐
│   Claude Desktop                        │
│                                         │
│   Bring Claude to your desktop         │
│                                         │
│   [Download for Windows]               │  ← Click
│                                         │
│   Also available for macOS and Linux   │
└─────────────────────────────────────────┘
```

3. **Click**: Download for your operating system

**Expected Outcome**: Installer downloads (ClaudeSetup.exe or similar)

---

### Step 2: Install Claude Desktop App

**Windows Installation:**

1. **Locate** the downloaded installer (usually in Downloads)
2. **Double-click** the installer
3. **Windows Security**: "Do you want to allow?"
   - Click **"Yes"**
4. **Installer runs**: Takes 30-60 seconds
5. **Claude Desktop launches** automatically

**Mac Installation:**

1. Open the `.dmg` file
2. Drag Claude to Applications
3. Open Applications folder
4. Launch Claude
5. **macOS Security**: "Claude is from an unidentified developer"
   - Right-click Claude → Open
   - Click "Open" in the dialog

**Expected Outcome**: Claude Desktop App opens

---

### Step 3: Sign In with Your Claude Pro Account

**Action:**

1. Claude Desktop shows sign-in screen
2. **Click**: "Sign in with Google" or "Sign in with Email"
3. **Use the same account** you use for claude.ai (your Pro account)

**What You'll See:**
```
┌─────────────────────────────────────────┐
│  Welcome to Claude Desktop              │
├─────────────────────────────────────────┤
│                                         │
│  Sign in to continue                   │
│                                         │
│  [Sign in with Google]                 │
│                                         │
│  [Sign in with Email]                  │
│                                         │
└─────────────────────────────────────────┘
```

4. **Browser opens** for authentication
5. **Sign in** with your credentials
6. **Return to Claude Desktop** - you're signed in!

**Important**: Your Claude Pro subscription works for both web and desktop!

**Expected Outcome**: Signed in, Claude Desktop ready to use

---

### Step 4: Verify Computer Use is Enabled

**What is Computer Use?**
- Claude can read/write files
- Claude can run bash commands
- Claude can navigate your file system
- Essential for Code mode

**Verify it's Enabled:**

1. Look at the bottom of the chat input
2. You should see icons for available tools

**What You'll See:**
```
┌─────────────────────────────────────────┐
│  [Type a message...]                    │
│                                         │
│  🖥️ 📁 🔍 ⚙️                          │  ← Tool icons
│  Computer File Search Settings         │
└─────────────────────────────────────────┘
```

If you see these icons, computer use is enabled!

**If Not Enabled:**
1. Click Settings (gear icon)
2. Look for "Enable computer use" or "Beta features"
3. Toggle it ON

**Expected Outcome**: Computer use enabled, ready for Code mode

---

## 📁 Part 3: Creating Your Life Ninja Project (15 minutes)

### Step 5: Create a New Project

**What is a Project?**
- A workspace for one codebase
- Maintains persistent memory
- Can upload reference files
- Accumulates knowledge over time

**Action:**

1. In Claude Desktop, look for "Projects" in the sidebar
2. **Click**: "+ New Project"

**What You'll See:**
```
┌─────────────────────────────────────────┐
│  Create New Project                     │
├─────────────────────────────────────────┤
│  Name:                                  │
│  [Life Ninja V3               ]        │
│                                         │
│  Description (optional):               │
│  [Personal task management app with    │
│   modular architecture migration]      │
│                                         │
│  [Create Project]                      │
└─────────────────────────────────────────┘
```

3. **Name**: "Life Ninja V3"
4. **Description**: Brief summary of what this is
5. **Click**: Create Project

**Expected Outcome**: New project created, opens in Claude Desktop

---

### Step 6: Upload Core Reference Files

**What to Upload:**
These files help Claude understand your project persistently.

**Files to Upload:**

1. **Life Ninja HTML** (current version)
   - File: `life-ninja.html` from your GitHub repo
   - Purpose: Claude knows your current codebase

2. **Master Roadmap** (we'll create this in Document #3)
   - File: `LIFE_NINJA_MASTER_ROADMAP.md`
   - Purpose: Claude knows the vision and plan

3. **Current Issues List**
   - File: `CURRENT_BUGS.md` (create this)
   - Purpose: Claude knows what to fix

4. **Architecture Decision Record**
   - File: `ARCHITECTURE.md` (we'll create in Document #4)
   - Purpose: Claude knows the technical decisions

**How to Upload:**

1. In your project, look for "Knowledge" or "Project Files"
2. **Click**: "+ Add Files" or "Upload"
3. **Select** the files from your computer
4. **Upload** - they become part of project memory

**What You'll See:**
```
┌─────────────────────────────────────────┐
│  Life Ninja V3 Project                  │
├─────────────────────────────────────────┤
│  Knowledge Base (4 files)              │
│                                         │
│  📄 life-ninja.html                     │
│  📄 LIFE_NINJA_MASTER_ROADMAP.md        │
│  📄 CURRENT_BUGS.md                     │
│  📄 ARCHITECTURE.md                     │
│                                         │
└─────────────────────────────────────────┘
```

**Expected Outcome**: Files uploaded, Claude has persistent context

---

### Step 7: Set Up Repository Path

**Tell Claude Where Your Code Lives:**

**First Message in the Project:**

```
You:

I'm setting up Life Ninja V3 development. Here's what you need to know:

📁 Repository Location:
C:\Users\Vikas\Documents\GitHub\life-ninja-v3

🎯 Current Version: 2.14.2

🐛 Current Bugs to Fix:
1. Search field requires multiple clicks
2. Sync delays causing data loss
3. Personas not syncing between devices
4. Gantt needs visual refinement
5. Timezone showing wrong date (India)
6. ESC key functionality needs testing

🏗️ Architecture Goal:
Migrate from single HTML file (11,171 lines) to modular components.

💻 My Capabilities:
- I can copy/paste files
- I can test on PC and Android
- I can use GitHub Desktop
- I CANNOT write code myself
- I CANNOT use command line

📋 Workflow Preference:
- You edit files directly in my repo
- I review changes in GitHub Desktop
- I commit when ready
- I test and report results

Ready to start?
```

**Claude's Response:**
```
Claude:

Perfect! I understand your setup. Here's what I'll do:

✅ All file changes will be in:
   C:\Users\Vikas\Documents\GitHub\life-ninja-v3

✅ I'll use the Code mode for implementations

✅ I'll create complete, tested changes

✅ You'll review in GitHub Desktop before committing

✅ I'll remember:
   - Your 6 current bugs
   - Your non-developer workflow
   - Your testing capabilities
   - Project structure and decisions

Let's start with the highest priority bug. 
Which should we tackle first?
```

**Expected Outcome**: Claude understands your project, ready to code

---

## 🔧 Part 4: Using Claude Desktop App Modes (20 minutes)

### Mode 1: PLAN - Strategic Thinking

**When to Use PLAN:**
- Starting a new feature
- Making architectural decisions
- Figuring out approach before coding

**Example Session:**

```
You (in PLAN mode):

Plan the migration of Life Ninja from a single 11k-line HTML file 
to a modular architecture. I want to keep using the app daily 
while we migrate. I can spend ~2 hours per day on this.

Claude (PLAN response):

Here's a comprehensive migration plan:

PHASE 1: PREPARATION (Week 1)
- Set up build tooling (Vite)
- Create component directory structure
- Document current feature dependencies
- Create rollback strategy
Risk: Low | Time: 8-10 hours

PHASE 2: EXTRACT UTILITIES (Week 2)
- Extract date helpers
- Extract calculation functions
- No UI changes (zero user impact)
- Test suite for utilities
Risk: Very Low | Time: 10-12 hours

PHASE 3: EXTRACT COMPONENTS (Weeks 3-5)
Week 3: TaskCard component
Week 4: Calendar component  
Week 5: Timeline component
Each week: Extract → Test → Commit
Risk: Medium | Time: 30-36 hours

[... detailed plan continues ...]

ROLLBACK STRATEGY:
- Keep monolith working in parallel
- Tag each stable milestone in GitHub
- Can revert to any tagged version in 5 minutes

DAILY USABILITY:
- Weeks 1-2: No change to your usage
- Week 3+: Test migrated version alongside monolith
- Switch fully only when you're confident

TOTAL TIME: ~60-70 hours over 5-7 weeks at 2 hrs/day

Questions?
```

**Key Points:**
- PLAN mode doesn't edit files
- Creates comprehensive strategy
- You review and approve before CODE mode
- Can iterate on the plan

---

### Mode 2: ASK - Questions and Clarifications

**When to Use ASK:**
- Understanding errors
- Debugging logic
- Learning concepts
- Clarifying architecture

**Example Session:**

```
You (in ASK mode):

Why does my search field require multiple clicks to work? 
The typing also works one character at a time.

Claude (ASK response):

Based on your code, this is likely caused by a focus-stealing 
issue. Let me explain:

THE PROBLEM:
When you type in the search field, React re-renders the component.
During re-render, something is causing the input to lose focus.

LIKELY CAUSES IN YOUR CODE:
1. State updates during onChange triggering re-renders
2. Parent component re-rendering the search input
3. Event handlers being recreated on each render

SPECIFIC ISSUE I SEE:
In your code around line 2847, the search input is inside a 
component that re-renders on every state change. When you type 
one character:
- onChange fires
- State updates
- Component re-renders  
- Input loses focus
- You must click again

THE FIX:
Use useRef to maintain focus:

```javascript
const searchRef = useRef(null);

useEffect(() => {
  if (isSearching) {
    searchRef.current?.focus();
  }
}, [isSearching, searchTerm]);
```

This keeps focus even during re-renders.

Want me to implement this fix in CODE mode?
```

**Key Points:**
- ASK mode explains without changing code
- Helps you understand the problem
- Suggests solutions
- Asks if you want to proceed to CODE mode

---

### Mode 3: CODE - Actual Implementation

**When to Use CODE:**
- Implementing features
- Fixing bugs
- Refactoring code
- Creating new files

**Example Session:**

```
You (in CODE mode):

Fix the search field continuous typing bug using your suggested 
approach. The file is at:
C:\Users\Vikas\Documents\GitHub\life-ninja-v3\life-ninja.html

Claude (CODE response):

I'll fix the search field focus issue now.

[Claude uses computer tools to edit the file]

✅ CHANGES MADE:

File: life-ninja.html
Lines modified: 2847-2865

What I did:
1. Added useRef for search input
2. Added useEffect to maintain focus
3. Connected ref to input element
4. Restored focus after re-renders

The search field will now:
- Accept continuous typing
- Not require multiple clicks
- Maintain focus during typing
- Work smoothly

TESTING STEPS:
1. Open life-ninja.html in Chrome
2. Click the search field
3. Type rapidly: "important urgent tasks"
4. Expected: All characters appear, no clicking needed
5. Try on Android too

Review the changes in GitHub Desktop and commit when ready!

If it works perfectly, let me know and we'll move to the next bug.
```

**What Actually Happened:**
- Claude edited your actual file
- Changes are in your GitHub repo
- You can see the diff in GitHub Desktop
- Ready to test immediately

**Key Points:**
- CODE mode makes real changes
- Always edits files in your repository
- Provides testing instructions
- You review before committing

---

## 🧠 Part 5: Project Memory and Persistence (15 minutes)

### How Project Memory Works

**Session 1 (Today):**
```
You: "Fix the search field bug"
Claude: [Fixes it, remembers the solution]
```

**Session 2 (Tomorrow):**
```
You: "The sync is slow, similar to the search issue"
Claude: "I remember the search field fix - that was a focus 
        issue. Sync slowness is different. Let me investigate..."
```

**Session 3 (Next Week):**
```
You: "Create analytics dashboard"
Claude: "I'll use the same component patterns I learned from 
        fixing search and sync. I'll also avoid the focus-stealing 
        pattern we fixed earlier."
```

**The Power:**
- Claude learns from each interaction
- Remembers your preferences
- Applies lessons to new features
- Accumulates project knowledge

---

### What Gets Remembered

**Automatically Remembered:**

1. **Code Structure**
   - Your component patterns
   - Your naming conventions
   - Your coding style

2. **Decisions Made**
   - "Use Vite for building"
   - "Keep Tailwind for styling"
   - "Test on PC and Android"

3. **Bugs Fixed**
   - What was broken
   - How it was fixed
   - Patterns to avoid

4. **Features Implemented**
   - How they work
   - Dependencies
   - Testing approach

5. **Your Workflow**
   - Review in GitHub Desktop
   - Test before committing
   - Report results

**Example of Memory in Action:**

```
Week 1:
You: "Fix search bug"
Claude: [Fixes using useRef]

Week 3:
You: "Add analytics modal"
Claude: "I'll use a modal pattern, and I'll remember to use 
        useRef for any input fields to avoid the focus issue 
        we fixed in the search field."

Week 5:
You: "Add voice input feature"
Claude: "For the voice input field, I'll apply the same focus 
        management pattern we used for search and analytics 
        modals."
```

**Result**: Claude gets better at Life Ninja over time!

---

### Updating Project Knowledge

**When to Update Project Files:**

1. **After Major Milestones**
   - Completed modular migration → Update ARCHITECTURE.md
   - Fixed all 6 bugs → Update CURRENT_BUGS.md
   - Released V3.0.0 → Update ROADMAP.md

2. **When Decisions Change**
   - Switched from Redux to Zustand → Update ARCHITECTURE.md
   - Changed testing framework → Update docs

3. **New Patterns Emerge**
   - Discovered better component pattern → Document it
   - Found optimization technique → Add to knowledge base

**How to Update:**

```
You:

Update the project knowledge. We've completed:
✅ All 6 bugs fixed
✅ Extracted 5 components
✅ Test coverage at 40%

New decisions:
- Using Vitest (not Jest)
- Component pattern: FC with named exports
- State: Zustand (decided against Redux)

Please update the architecture document.

Claude:

I'll update ARCHITECTURE.md with these learnings.

[Updates the file in your repo]

✅ Updated: ARCHITECTURE.md

Added sections:
- Testing: Vitest setup and patterns
- Components: Our FC naming pattern
- State: Why we chose Zustand
- Completed migrations from bug fixes

The knowledge base now reflects our current V3 architecture!
```

**Expected Outcome**: Project knowledge stays current

---

## 🔗 Part 6: GitHub Desktop + Claude Desktop Integration (15 minutes)

### The Complete Workflow

**Step-by-Step Integration:**

```
1. YOU (Planning):
   "I want to add analytics dashboard"
   ↓
2. CLAUDE (PLAN mode):
   Creates detailed implementation plan
   ↓
3. YOU (Review):
   "Looks good, proceed!"
   ↓
4. CLAUDE (CODE mode):
   Edits files in your GitHub repository
   ↓
5. GITHUB DESKTOP (Automatic):
   Detects changes, shows diff
   ↓
6. YOU (Review):
   Check changes in GitHub Desktop
   ↓
7. YOU (Decide):
   Option A: Looks good → Commit
   Option B: Issues → Tell Claude
   ↓
8. YOU (If Option A):
   Commit: "Add: Analytics dashboard"
   Push to GitHub cloud
   ↓
9. YOU (Test):
   Open app, test on PC and Android
   ↓
10. YOU (Report):
    "Works perfectly!" or "Found bug X"
    ↓
11. CLAUDE (If bug):
    Fixes in CODE mode → Back to step 5
```

**Visual Diagram:**
```
┌──────────────────────────────────────────────────┐
│                                                  │
│  YOU ──────> CLAUDE DESKTOP ──────> YOUR FILES  │
│   ▲            (CODE mode)              │        │
│   │                                     ▼        │
│   │                              GITHUB DESKTOP  │
│   │                                     │        │
│   └──────────── REVIEW ────────────────┘        │
│                                                  │
│  If good: Commit & Push                         │
│  If bad: Ask Claude to fix                      │
│                                                  │
└──────────────────────────────────────────────────┘
```

---

### Real Example: Fixing Search Bug

**Complete Flow:**

**1. Initial Request (ASK mode):**
```
You:
Why does the search field need multiple clicks?
File: C:\Users\Vikas\Documents\GitHub\life-ninja-v3\life-ninja.html
```

**2. Claude Analyzes (ASK response):**
```
Claude:
It's a focus-stealing issue from re-renders. Here's why...
[Explains the problem]
Want me to fix it in CODE mode?
```

**3. You Approve (Switch to CODE):**
```
You:
Yes, fix it please.
```

**4. Claude Implements (CODE mode):**
```
Claude:
[Uses computer tools]
✅ Modified: life-ninja.html (lines 2847-2865)
✅ Added useRef for search persistence
✅ Testing steps: [lists them]

Check GitHub Desktop for the changes!
```

**5. You Review in GitHub Desktop:**

Open GitHub Desktop, you see:
```
Changes (1)
✓ life-ninja.html

Diff:
+ const searchRef = useRef(null);
+ 
+ useEffect(() => {
+   if (isSearching) {
+     searchRef.current?.focus();
+   }
+ }, [isSearching, searchTerm]);
+
+ <input
+   ref={searchRef}
```

**6. You Commit:**
```
Summary: "Fix: Search field continuous typing"
Description: "Added useRef to maintain focus during re-renders.
             No more multiple clicks needed.
             Fixes bug #1."
[Commit to main]
```

**7. You Test:**
- Open life-ninja.html
- Click search field
- Type rapidly
- ✅ Works! No clicking needed!

**8. You Report:**
```
You:
Perfect! Search field works great now. Let's move to bug #2.
```

**Claude Remembers This Success:**
- Focus issues → Use useRef
- This pattern works for Life Ninja
- Apply to future input fields

---

### What if Claude's Code Breaks Something?

**Recovery Process:**

**1. You Notice:**
```
You:
The search fix broke the task list! Tasks aren't showing now.
```

**2. Rollback in GitHub Desktop:**
```
History tab → Right-click last commit → Revert this commit
```

**3. Tell Claude:**
```
You:
I rolled back the search fix. It broke the task list.
Here's the error: [paste console error]
```

**4. Claude Analyzes:**
```
Claude:
I see the issue - I accidentally removed the task list 
rendering logic. Let me fix this more carefully.

This time I'll:
1. Only touch the search input
2. Keep task list logic intact
3. Test the changes before delivery
```

**5. Claude Tries Again (CODE mode):**
```
Claude:
✅ Fixed search field (more carefully)
✅ Verified task list still renders
✅ Tested in isolation

Try it now!
```

**6. You Test:**
- Search works ✅
- Task list works ✅
- Both fixed!

**7. Commit the Good Version:**
```
Summary: "Fix: Search field typing (v2, safe)"
[Commit]
```

**Claude Learned:**
- Be more careful with adjacent code
- Test before delivery
- Isolate changes

**This learning carries forward!**

---

## 🎓 Part 7: Advanced Features (10 minutes)

### Feature 1: Skills

**What Are Skills?**
Reusable patterns Claude can apply to your project.

**Example Skill: "Life Ninja Component Pattern"**

Create a file: `SKILLS/life-ninja-component-pattern.md`

```markdown
# Life Ninja Component Pattern

When creating new components for Life Ninja:

## File Structure
```javascript
// TaskCard.jsx
import React from 'react';

const TaskCard = ({ task, onUpdate }) => {
  // Component logic
  return (
    // JSX
  );
};

export default TaskCard;
```

## Naming Convention
- PascalCase for component files
- Descriptive names (TaskCard, not Card)
- One component per file

## Props Pattern
- Destructure props in parameters
- Use PropTypes or TypeScript
- Include onUpdate handlers

## State Management
- Use Zustand for global state
- useState for local state
- useRef for DOM references (learned from search fix!)

## Styling
- Tailwind utility classes
- No inline styles
- Responsive by default (mobile-first)

## Testing
- Vitest for unit tests
- Test user interactions
- Mock Supabase calls
```

**Upload to Project:**
- Claude now knows this pattern
- Applies it automatically
- Consistent components every time

---

### Feature 2: Custom Instructions

**Set Project-Wide Instructions:**

In project settings, add:

```
CRITICAL RULES FOR LIFE NINJA:
1. ALWAYS test on both PC and Android
2. NEVER break existing features
3. ALWAYS use GitHub Desktop workflow
4. ALWAYS provide testing steps
5. ALWAYS preserve Supabase sync logic
6. NEVER use command line (user can't)
7. ALWAYS create complete files (no snippets)

USER CONSTRAINTS:
- Non-developer, needs simple explanations
- Can only copy/paste complete files
- Uses GitHub Desktop for version control
- Tests manually (no automated testing yet)

CODE PREFERENCES:
- React functional components
- Zustand for state
- Tailwind for styling
- Vitest for tests
- Clear comments in complex logic
```

**Claude follows these rules automatically in all conversations!**

---

### Feature 3: Templates

**Create Reusable Templates:**

**Bug Fix Template:**
```markdown
# Bug Fix Template

## Bug Description
[What's broken]

## Root Cause
[Why it's broken]

## Solution
[How we'll fix it]

## Files Changed
- file1.js (lines X-Y)
- file2.js (lines A-B)

## Testing Steps
1. [Step 1]
2. [Step 2]
3. Expected outcome

## Rollback Plan
[If this breaks something]
```

**New Feature Template:**
```markdown
# Feature Implementation Template

## Feature Name
[Name]

## User Story
As a [user], I want [feature] so that [benefit].

## Acceptance Criteria
- [ ] Criterion 1
- [ ] Criterion 2

## Implementation Plan
1. [Step 1]
2. [Step 2]

## Files to Create/Modify
[List]

## Dependencies
[What this relies on]

## Testing Checklist
- [ ] Works on PC
- [ ] Works on Android
- [ ] Syncs across devices
- [ ] No console errors

## Rollback Plan
[Safety net]
```

**Use Templates:**
```
You:
Use the bug fix template for the sync delay issue.

Claude:
# Bug Fix: Sync Delay Causing Data Loss

## Bug Description
Sync takes too long between devices, causing users to lose 
data when switching devices quickly.

[... fills out entire template ...]
```

---

## 💰 Part 8: Cost Optimization (10 minutes)

### Staying Within Your Budget

**Your Current Budget:**
- ✅ Claude Pro: $20/month (INR 2,200)
- ✅ Other subscriptions: Google One, OneDrive

**Claude Desktop App Usage:**
- Included in Claude Pro ✅
- No additional cost for computer use ✅
- Same message limits as web ✅

**Cost-Free Tools We'll Use:**

1. **GitHub**: Free tier
   - Unlimited public/private repos
   - GitHub Desktop (free)
   - Version control (free)

2. **Vite**: Free, open-source
   - Build tool
   - Development server
   - No cost

3. **Vitest**: Free, open-source
   - Testing framework
   - No cost

4. **Supabase**: Free tier
   - You're already using this ✅
   - 500MB database
   - 50,000 monthly active users
   - Real-time subscriptions

**Services to AVOID (they cost money):**

| Service | Why Avoid | Free Alternative |
|---------|-----------|------------------|
| ❌ Anthropic API | $$ per request | Use Claude Pro (included) |
| ❌ OpenAI API | $$ per request | Use ChatGPT Go (free till Nov) |
| ❌ Vercel/Netlify Pro | $$ for hosting | Use GitHub Pages (free) |
| ❌ Supabase Pro | $25/month | Stay on free tier |

**Optimization Strategies:**

1. **Use Claude Desktop Efficiently**
   - Plan before coding (saves messages)
   - Batch related changes
   - Review before asking for edits

2. **Development Workflow**
   - Test locally (free)
   - Use GitHub Pages for deployment (free)
   - Supabase free tier is plenty for personal use

3. **AI Usage**
   - Claude Pro for development (included)
   - ChatGPT Go for research (free till Nov)
   - Perplexity Pro for search (free till July)

**Your Cost Breakdown:**
```
Development Tools: $0
Claude Pro: $20/month (already paying)
GitHub: $0
Hosting: $0 (GitHub Pages)
Database: $0 (Supabase free tier)
──────────────────────────
Total: $20/month ✅
```

**When You Might Need to Pay (Optional, Future):**

- Voice features: ElevenLabs ($5/mo)
- AI features: Anthropic API (~$10-20/mo)
- Advanced analytics: Mixpanel ($0 for < 100K events)

**But for V3.0 foundation: $0 additional! ✅**

---

## 📚 Part 9: Best Practices (15 minutes)

### Practice 1: Start Each Session with Context

**Bad Start:**
```
You: "Fix the bug"
```

**Good Start:**
```
You:

Starting development session.

📍 Current Status:
- Working on V3 modular migration
- Completed: Search fix, sync optimization
- Next: Personas sync bug

🎯 Today's Goal:
Fix personas not syncing between devices

📁 Working Directory:
C:\Users\Vikas\Documents\GitHub\life-ninja-v3

💭 Context:
Personas are stored in Supabase 'user_preferences' table.
PC updates work, but Android doesn't receive real-time updates.
Probably a real-time subscription issue.

Ready?
```

**Why Better:**
- Claude knows where you are
- Understands the goal
- Has necessary context
- Can start immediately

---

### Practice 2: Use Descriptive Mode Names

**In Claude Desktop, name your conversations:**

Instead of:
```
❌ "New Chat"
❌ "Development"
❌ "Bug Fix"
```

Use:
```
✅ "Life Ninja: Personas Sync Fix"
✅ "Life Ninja: Analytics Dashboard Implementation"
✅ "Life Ninja: Modular Migration - Week 3"
```

**Benefits:**
- Easy to find old conversations
- Know what each conversation covered
- Better organization

---

### Practice 3: Document Decisions

**After Major Decisions:**

```
You:

Document this decision in the project knowledge:

DECISION: State Management
Date: Feb 2, 2026
Choice: Zustand
Alternatives Considered: Redux, Context API

Reasoning:
- Simpler than Redux
- Better than Context for our use case
- Smaller bundle size
- Easier to test

Implementation:
- Install zustand
- Create stores/taskStore.js
- Migrate from useState gradually

Claude:

✅ Documented in ARCHITECTURE.md
✅ Added to decision log

Future me will know why we chose Zustand!
```

---

### Practice 4: Create Session Summaries

**End of Each Session:**

```
You:

Create a session summary for project memory.

Claude:

# Session Summary: Feb 2, 2026

## Completed
✅ Fixed search field continuous typing
✅ Fixed timezone display (India)
✅ Tested both fixes on PC and Android

## Code Changes
- life-ninja.html (3 commits)
  - Search: Added useRef for focus
  - Timezone: Use local time not UTC
  - Version: Updated to V2.14.3

## Bugs Remaining
4. Sync delays (next priority)
5. Personas not syncing
6. Gantt visual refinement
7. ESC key verification

## Next Session
- Start with sync delay bug
- Investigate Supabase real-time subscription
- Estimated time: 1-2 hours

## Notes
- Search fix pattern can be reused for other inputs
- Timezone fix was simple (one line change)
- User prefers testing on Android after PC
```

**Save this summary in project files!**

---

## 🎯 Part 10: Your First Session Checklist

### Complete First-Time Setup

**Before Starting Development:**

- [ ] Claude Desktop App installed
- [ ] Signed in with Claude Pro account
- [ ] Computer use enabled (tool icons visible)
- [ ] Created "Life Ninja V3" project
- [ ] Uploaded current HTML file to project
- [ ] Uploaded roadmap/docs to project
- [ ] Set repository path in first message
- [ ] Understand PLAN / ASK / CODE modes
- [ ] GitHub Desktop is set up (from Doc #1)
- [ ] Repository folder located and accessible

**First Development Session:**

- [ ] Open Claude Desktop App
- [ ] Select "Life Ninja V3" project
- [ ] Start with ASK mode for bug analysis
- [ ] Switch to CODE mode for fix
- [ ] Review changes in GitHub Desktop
- [ ] Test the changes locally
- [ ] Commit if working
- [ ] Push to GitHub cloud
- [ ] Document the fix

**After First Session:**

- [ ] Create session summary
- [ ] Update CURRENT_BUGS.md
- [ ] Tag working version in GitHub
- [ ] Plan next session

---

## 🆘 Part 11: Troubleshooting

### Issue 1: Claude Can't Access My Files

**Symptoms:**
- "I don't have access to that file"
- "File not found"

**Solution:**
1. Verify computer use is enabled
2. Check file path is correct
   - Use full path: `C:\Users\...\life-ninja-v3\life-ninja.html`
   - Not relative path: `.\life-ninja.html`
3. Make sure file exists in that location

---

### Issue 2: Changes Not Showing in GitHub Desktop

**Symptoms:**
- Claude says it edited file
- GitHub Desktop shows no changes

**Solution:**
1. Click "Refresh" in GitHub Desktop (Ctrl+R)
2. Check Claude edited the right file
   - Correct: `\GitHub\life-ninja-v3\life-ninja.html`
   - Wrong: `\Downloads\life-ninja.html`
3. Verify file was saved (Claude should confirm)

---

### Issue 3: Claude Forgot Project Context

**Symptoms:**
- Asks questions it should know
- Doesn't remember previous fixes
- Seems to start fresh

**Solution:**
1. Make sure you're in the right PROJECT
   - Not just any chat - the specific Life Ninja V3 project
2. Check project files are uploaded
3. Reference previous conversations:
   ```
   You: "Remember when we fixed the search field with useRef?
        Apply that same pattern here."
   ```

---

### Issue 4: Code Mode Not Available

**Symptoms:**
- No CODE option
- Only ASK available

**Solution:**
1. Enable computer use in settings
2. Restart Claude Desktop App
3. Update Claude Desktop to latest version
4. Check your Pro subscription is active

---

## 📖 Glossary

| Term | Simple Explanation |
|------|-------------------|
| **PLAN Mode** | Strategic thinking, no code changes |
| **ASK Mode** | Questions and explanations |
| **CODE Mode** | Actual file editing and changes |
| **Project** | Workspace with persistent memory |
| **Computer Use** | Claude can read/write files |
| **Project Memory** | Claude remembers across sessions |
| **Skill** | Reusable pattern Claude knows |
| **Session Summary** | Notes from a development session |

---

## ✅ Setup Complete Checklist

Before moving to Document #3:

- [ ] Claude Desktop App installed and working
- [ ] Signed in with Claude Pro
- [ ] Created Life Ninja V3 project
- [ ] Uploaded reference files
- [ ] Tested PLAN mode
- [ ] Tested ASK mode
- [ ] Tested CODE mode (made a small edit)
- [ ] Changes appeared in GitHub Desktop
- [ ] Successfully committed a Claude-made change
- [ ] Understand how to rollback if needed
- [ ] Know how to update project knowledge
- [ ] Created first session summary

**All checked?** → You're ready for Document #3: Master Roadmap! 🚀

---

**Document Version**: 1.0  
**Last Updated**: February 2, 2026  
**Previous**: 01_GITHUB_DESKTOP_SETUP_GUIDE.md  
**Next**: 03_CONSOLIDATED_MASTER_ROADMAP.md  
**Estimated Setup Time**: 30-45 minutes  
**Support**: Reference this anytime you need Claude Desktop help!
