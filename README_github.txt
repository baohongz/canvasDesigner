# baohongz / w1
git clone https://github.com/baohongz/MyProject.git
cd MyProject
git checkout --orphan gh-pages

git status

# Update files
git add .
git commit -a -m "Data Visualization, RNA-seq 101"
git push origin gh-pages

# Add files
git add jquery.js jquery.tablesorter.min.js
git commit -a -m "Added jQuery"
git push origin gh-pages

# update local copy
git pull origin gh-pages

# rename file
git mv QAmiRSeq.html QuickMIRSeq.html

zip -r Lupus_eQTL.zip *.html *.pl package


# w!2
git clone https://github.com/interactivereport/ZSF1 -b gh-pages
git push https://interactivereport@github.com/interactivereport/ZSF1.git gh-pages:gh-pages

I am using Mac and the issue is solved by deleting github record from keychain access app: Here is what i did:

Open "Keychain Access.app" (You can find it in Spotlight or LaunchPad)
Select "All items" in Category
Search "git"
Delete every old & strange items Try to Push again and it just WORKED
