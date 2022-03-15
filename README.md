# Github Action: rio-clean-dev-releases

## Release new version

1) Make sure you have `@vercel/ncc` installed globally.
    - `npm i -g @vercel/ncc` if not the case.
1) Compile the `index.js` file.
    - `ncc build index.js --license licenses.txt`
1) Bump version in `package.json` file.
1) Stage the new/edited files.
    - `git add .` or else
1) Commit
    - `git commit -m YOUR_MESSAGE`
1) Tag
    - `git tag -a -m RELEASE_NAME RELEASE_CODE`
1) Push
    - `git push --follow-tags`