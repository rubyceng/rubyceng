# WakaTime Integration Setup Guide

This repository has been integrated with WakaTime statistics to automatically display beautiful coding metrics in the README.

## Setup Instructions

### 1. WakaTime Setup
1. Create a [WakaTime account](https://wakatime.com) if you don't have one
2. Get your WakaTime API Key from [Account Settings](https://wakatime.com/settings/account)
3. Install WakaTime plugins in your favorite IDE/editors:
   - [VS Code](https://wakatime.com/vs-code)
   - [IntelliJ IDEA](https://wakatime.com/intellij-idea)
   - [WebStorm](https://wakatime.com/webstorm)
   - [Other IDEs](https://wakatime.com/plugins)

### 2. Repository Secrets Setup
1. Go to your repository Settings → Secrets and variables → Actions
2. Add a new repository secret:
   - Name: `WAKATIME_API_KEY`
   - Value: Your WakaTime API key from step 1.2

### 3. Workflow Features
The GitHub Action will automatically update your README with:
- 📊 **Coding Time Statistics** - Total time spent coding
- 💻 **IDE/Editor Usage** - Which development tools you use most
- 🔧 **Programming Languages** - Time spent in each language
- 📅 **Most Productive Days** - When you're most active
- ⏰ **Daily Patterns** - Morning vs evening productivity
- 🌍 **Operating System** - Development environment details
- 📁 **Project Statistics** - Time spent on different projects
- 📈 **Repository Language Distribution** - Languages across your repos

### 4. Schedule
- The workflow runs automatically every day at 10:00 AM Beijing time (2:00 AM UTC)
- You can also manually trigger it from the Actions tab → Waka Readme → Run workflow

### 5. Customization
You can modify `.github/workflows/waka-readme.yml` to:
- Change the update schedule (modify the cron expression)
- Enable/disable specific statistics (set flags to "True" or "False")
- Change the locale for different languages
- Customize commit messages and date formats

## Statistics Preview
Once set up, you'll see beautiful statistics like:
- Language usage charts
- IDE preferences
- Daily/weekly coding patterns  
- Project time breakdown
- And much more!

The statistics will appear in the `📊 Development Statistics` section of the README.