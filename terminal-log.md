# Terminal Navigation & Setup Log
## Exercise 1 : Basic Navigation
`pwd`- Showed the current working directory path.
`ls` - Listed files and directories in the current folder.
`cd ~/Documents` - Navigated to the Documents directory.
`cd ..` - Moved up one directory level.
`cd ~` - Returned to the home directory.
`cd ~/terminal-practice` - Navigated into the terminal practice directory.

## Exercise 2 : Create Project Structure
`mkdir my-project` - Created the main project folder.
`cd my-project`- Navigated into the my-project directory.
`mkdir -p src/css src/js src/images docs tests` - Created nested subdirectories for source assets,docs, and tests.
`touch README.md`- Created an empty README.md file inside my-project.
`ls -R`- Listed all files and subdirectories to verify the structure.

# File Operations

## Exercise 1 : Create and Edit Files
`touch index.html` -Created a new empty index.html file.
`cat index.html` - Viewed file contents.
`cp index.html backup.html` - Copied index.html to create backup.html.
`mv backup .html docs/` - Moved the file into the docs directory.
`mv index.html home.html` - Renamed index.html to home.html.
`rm home.html` - Deleted the home.html file.

## Working with Directories
`cp -r src/ src-backup/` - Copied the src directory to src-backup.
`mv src-backup/ archive/` - Renamed the src-backup directory to archive.
`rmdir archive/` - Attempted to remove archive failed because the directory was not empty.
`rm -r archive/` - Removed the non-empty archive directory and its contents.
## Challenge: Portfolio Reorganization
`mkdir portfolio-v2` - Created anew folder for the re-organized project version 2 structure.
`mv src/ portfolio-v2/` - Moved the src folder into portfolio-v2.
`mv README.md portfolio-v2` - Moved the README file into portfolio-v2.
`ls -R portfolio-v2` - Listed the contents of portfolio-v2 to verify the final reorganized structure.

# Useful Terminal Commands

## Search and Find
`find portfolio-v2 -name "*.html"`
`grep -rn "contact" portfolio-v2/`
`grep -r "button" ./src/`
`wc -1 portfolio-v2/src/css/*.css`
`history `

### View and Edit
`head-10 style.css`
`tail-10 style.css`
`wc index.html`
`wc -1 index.html`

## Questions and Answers
1. How many HTML files are in your portfolio project?
`portfolio-v2/docs/backup.html`
2. Which files contain the word "contact"? 
` grep -rn "contact" portfolio-v2/` - None 
3. How many lines is your CSS file?
- `wc -l portfolio-v2/src/css/*.css` - Attempted line count for CSS files; confirmed `src/css/` directory is currently empty (0 lines / no CSS file).
4. What were your last 10 terminal commands?
- `history` 
 `ls -R portfolio-v2`
 `tail -10 portfolio-v2/src/css/*.css`
 `wc index.html`
 `wc portfolio-vs/index.html/`
  `wc -l portfolio-v2/docs/backup.html`
  `wc -l portfolio-v2/src/css/*.css`
  `find portfolio-v2 -name "*.html"`
   `grep -rn "contact" portfolio-v2/`
   `wc -l portfolio-v2/src/css/*.css/`
    `history`

 ### Shell Script Basics
 - Created `new-project.sh` to automate project folder and file creation.
- Made the script executable using`chmod +x new-project.sh`.
- Tested the script successfully with`./new-project.sh my-awesome-app`




