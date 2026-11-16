# Dad's 50th Present

A small static gift site: four questions, a present to unwrap, then a reveal page with falling flowers and the birthday video.

## Files
- `index.html` : the whole site (styles and script are inside it)
- `video.mp4` : the birthday video (720p)
- `poster.jpg`, `p03.jpg`, `p12.jpg`, `p20.jpg` : images used on the pages
- `netlify.toml` : tells Netlify there is no build step

## Put it on GitHub
1. On github.com choose New repository, name it (for example `dad-50th`), set it to **Private**, and create it.
2. On the new repo page click "uploading an existing file", drag in every file from this folder (the files, not the folder itself), and commit.

## Host it on Netlify
1. On app.netlify.com choose Add new site > Import an existing project > GitHub and pick the repo.
2. Leave the build command empty and the publish directory as `.` (already set by `netlify.toml`), then deploy.
3. Netlify gives you a link such as `https://something.netlify.app`. Rename it under Site configuration > Change site name.

## Changing the questions
Open `index.html` and search for `data-step="1"`. Each question is a `<section>`; the correct answer is the button with `data-ok="1"`, and `data-msg` is the line shown for a wrong answer.
