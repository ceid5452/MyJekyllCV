# MyJekyllCV

How to create a Jekyll theme on macOS in a few steps:
- **[Jekyll documendation](https://jekyllrb.com/docs/installation/macos/)** </br>

### 1. Install xcode
xcode-select –install 

# 2. Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 3. Install Ruby
brew install ruby

# 4. Install the newst version of jekyll
sudo gem install bundler jekyll

# 5. Create a new jekyll page
jekyll new project_name 

# 6. Change  directory and open the project
cd directory/project_name  

# 7. Open the project on localhost
bundle exec jekyll serve 

# 8. Type the server address to your browser to see the project 

# 9. Edit or create your yaml files on _data and call them on index.markdown

# 10. Take GitHub to the command line
- **[cli documendation](https://cli.github.com/)** </br>
brew install gh

# 11. Add your project on github
- **[full documendation](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-an-existing-project-to-github-using-the-command-line)** </br>
git init -b main
git add . && git commit -m "initial commit"
gh repo create --source=. --public --push


