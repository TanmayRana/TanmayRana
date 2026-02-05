# 🚀 GitHub Profile Setup Guide

This guide will help you set up your awesome GitHub profile with all the dynamic features and GitHub Actions.

## 📋 Prerequisites

- A GitHub account
- Basic knowledge of Git and GitHub

## 🎯 Step-by-Step Setup

### 1. Create Special Repository

1. Go to [GitHub](https://github.com)
2. Click on **"+"** in the top-right corner → **"New repository"**
3. **IMPORTANT**: Name the repository **exactly** as your GitHub username (e.g., `TanmayRana`)
4. Make sure the repository is **Public**
5. Check **"Add a README file"**
6. Click **"Create repository"**

### 2. Upload Files to Your Repository

1. Clone your newly created repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_USERNAME.git
   cd YOUR_USERNAME
   ```

2. Copy the `README.md` file to your repository root

3. Create the `.github/workflows` directory and add all workflow files:
   ```bash
   mkdir -p .github/workflows
   ```

4. Add the following workflow files to `.github/workflows/`:
   - `snake.yml` - For contribution snake animation
   - `blog-post-workflow.yml` - For blog post updates
   - `dev-metrics.yml` - For development metrics (optional)

5. Commit and push:
   ```bash
   git add .
   git commit -m "✨ Add awesome GitHub profile"
   git push origin main
   ```

### 3. Configure GitHub Actions

#### Enable GitHub Actions

1. Go to your repository on GitHub
2. Click on **"Settings"** → **"Actions"** → **"General"**
3. Under **"Workflow permissions"**, select:
   - ✅ **"Read and write permissions"**
   - ✅ **"Allow GitHub Actions to create and approve pull requests"**
4. Click **"Save"**

#### Run Snake Animation Workflow

1. Go to **"Actions"** tab in your repository
2. Click on **"Generate Snake Animation"** workflow
3. Click **"Run workflow"** → **"Run workflow"**
4. Wait for it to complete (should take ~1 minute)

This will create an `output` branch with the snake animation SVGs.

### 4. Customize Your Profile

#### Update Personal Information

Replace the following in `README.md`:

1. **Username**: Replace all instances of `TanmayRana` with your GitHub username
2. **Email**: Replace `tanmayrana2001@gmail.com` with your email
3. **LinkedIn**: Update the LinkedIn URL
4. **LeetCode**: Update your LeetCode profile URL
5. **Location**: Update your location information
6. **Projects**: Add your own project details with correct repository links

#### Update Project Links

In the "Featured Projects" section, update:
- Repository URLs
- Live demo URLs (if available)
- Project descriptions
- Technologies used

### 5. Optional Enhancements

#### Add WakaTime Stats (Optional)

If you want to display coding activity metrics:

1. Sign up at [WakaTime](https://wakatime.com/)
2. Install WakaTime extension in your code editor
3. Get your WakaTime API key from [Account Settings](https://wakatime.com/settings/account)
4. In your GitHub repository:
   - Go to **Settings** → **Secrets and variables** → **Actions**
   - Click **"New repository secret"**
   - Name: `WAKATIME_API_KEY`
   - Value: Your WakaTime API key
5. Create another secret:
   - Name: `GH_TOKEN`
   - Value: Your GitHub Personal Access Token ([Create one here](https://github.com/settings/tokens))

#### Add Blog Post Updates

If you have a blog (Dev.to, Medium, etc.):

1. Update the RSS feed URL in `blog-post-workflow.yml`:
   ```yaml
   feed_list: "https://dev.to/feed/YOUR_USERNAME"
   ```

2. The workflow will automatically fetch your latest blog posts and update the README

#### Customize Themes

You can change the color themes for stats cards:

Available themes: `dark`, `radical`, `merko`, `gruvbox`, `tokyonight`, `onedark`, `cobalt`, `synthwave`, `highcontrast`, `dracula`

Update in README.md:
```markdown
?theme=tokyonight
```

### 6. Verify Everything Works

1. Check your GitHub profile: `https://github.com/YOUR_USERNAME`
2. Verify that the README is displayed
3. Check that the snake animation appears (may take a few minutes)
4. Ensure all badges and stats are loading correctly

## 🎨 Customization Tips

### Header Image

You can customize the header wave animation:
```markdown
https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200...
```

Parameters:
- `type`: waving, wave, cylinder, egg, etc.
- `color`: gradient, timeGradient, or hex color
- `height`: Height in pixels
- `text`: Your text
- `fontSize`: Font size

### Typing Animation

Customize the typing animation messages:
```markdown
&lines=Full-Stack+Developer;AI+Enthusiast;Your+Custom+Message
```

### Badges

Add more badges from [shields.io](https://shields.io/) or [simpleicons.org](https://simpleicons.org/)

Format:
```markdown
![Badge Name](https://img.shields.io/badge/-Badge_Text-COLOR?style=for-the-badge&logo=LOGO_NAME&logoColor=white)
```

## 🔧 Troubleshooting

### Snake Animation Not Showing

1. Make sure the workflow ran successfully in Actions tab
2. Check that the `output` branch was created
3. Verify workflow permissions are set correctly
4. Wait a few minutes and refresh the page

### Stats Not Loading

1. Check that your username is correct in all URLs
2. Try clearing browser cache
3. Wait a few minutes as external APIs may be slow

### Workflow Failing

1. Check the Actions tab for error messages
2. Ensure GitHub Actions is enabled
3. Verify all permissions are set correctly
4. Check that branch name is `main` (not `master`)

## 📚 Additional Resources

- [GitHub Profile README Guide](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Snake Animation](https://github.com/Platane/snk)
- [Shields.io - Badges](https://shields.io/)
- [Simple Icons](https://simpleicons.org/)

## 🎯 Next Steps

1. ✅ Set up your profile repository
2. ✅ Add README.md
3. ✅ Configure GitHub Actions
4. ✅ Customize with your information
5. ✅ Add your projects
6. 🌟 Keep updating with new projects and achievements!
7. 🚀 Share your awesome profile!

## 💡 Pro Tips

1. **Keep it updated**: Regularly update your projects and achievements
2. **Pin your best repositories**: Pin your top 6 repositories on your profile
3. **Add project screenshots**: Include GIFs or images in project READMEs
4. **Write good commit messages**: They show up in your activity
5. **Contribute to open source**: Builds your contribution graph
6. **Maintain consistency**: Use similar styling across all your READMEs

---

**Happy Coding! 🚀**

If you need help or have questions, feel free to open an issue in your repository or reach out!
