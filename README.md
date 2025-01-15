# Alice

[![MIT Licensed][icon-mit]][license]

Link to Alice's Adventures In Wonderland book: [book][1]  
All needed illustrations could be found at: [images][2]

## Getting started

- Create [GitLab account][3]. Strictly recommended pattern
  for the __username__: `name.lastname`, use your personal
  email (ex: `@gmail.com`)
- Create [Personal Access Token][4] with `write_repository` scope
- Request Access:
  ![requestAccess][5]
- Clone repository to your local machine

```bash
git clone https://YOUR_TOKEN_NAME:YOUR_TOKEN_VALUE@gitlab.com/iryna.v.afanasieva/alice.git
```

If you clone without your Personal Access Token

```bash
git remote set-url origin https://YOUR_TOKEN_NAME:YOUR_TOKEN_VALUE@gitlab.com/iryna.v.afanasieva/alice.git
```

- Create new branch, follow `feature/page-No` pattern,
  lets assume that your page number is 42:

```bash
git checkout -b feature/page-42
```

- Add necessary page content into [AliceInWonderland.md][6]:
  1. Add solid line
  1. Add page number
  1. Add page content
  1. **Attention!** Redundant empty lines are not accepted
- Commit changes: commit message should begin with `Page No:`

```bash
git status
git add .
git status
git commit -m "Page 42: your changes description"
```

- Push your branch into repository:

```bash
git push -u origin feature/page-42
```

- Take a look at your `AliceInWonderland.md` file:
  1. All fragments from the `main` branch should not be changed
  1. Newly added fragment has the same style
- Create MR (Merge Request)
- Rebase your branch if `main` ahead:
  ![Rebase Your Branch][7]
- Resolve merge conflicts if needed
- Make sure your MR pipeline is green (status: `passed`)
- Wait for a review

## Additional Sources

- [Git tips][8] — consolidate your knowledge of Git
- [Learn git branching][9] — improve your understanding of branching
- [Markdown Guide][10]

[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[license]: https://gitlab.com/gitlab-org/gitlab-foss/-/raw/master/LICENSE
[1]: https://www.adobe.com/be_en/active-use/pdf/Alice_in_Wonderland.pdf
[2]: https://www.gutenberg.org/files/19778/19778-h/images/
[3]: https://gitlab.com/users/sign_up
[4]: https://gitlab.com/-/user_settings/personal_access_tokens
[5]: requestAccess.png
[6]: AliceInWonderland.md
[7]: rebaseYourBranch.png
[8]: http://sixrevisions.com/web-development/git-tips/
[9]: http://learngitbranching.js.org
[10]: https://www.markdownguide.org/basic-syntax/
