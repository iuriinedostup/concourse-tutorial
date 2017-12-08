git checkout --orphan version
git rm --cached -r .
rm -rf *
rm .gitignore .gitmodules
touch README.md
# Copy all this MD content into readme.md
echo "0.0.1" > version
git add .
git commit -m "new branch"
git push origin version