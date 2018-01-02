# Simple Git With Bin

Fork from [simple-git](https://github.com/steveukx/git-js) project. Support to indicate the Git bin path.

# Installation

```
npm install simple-git-with-bin
```

# Dependencies

no

# Usage

Include into your app using:

```js
const gitWithBin = require('simple-git-with-bin')
const git = gitWithBin(workingDirPath, { git: binPath })
git.status((err, status) => {
  if (!err) {
    console.log(status)
  }
})
```

set `workingDirPath` to empty string, defaulting to the current directory.

```js
const gitWithBin = require('simple-git-with-bin')
const git = gitWithBin('', { git: binPath })
git.status((err, status) => {
  if (!err) {
    console.log(status)
  }
})
```

For more info, refer to the [simple-git documentation](https://github.com/steveukx/git-js)
