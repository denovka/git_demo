[![MIT Licensed][icon-mit]][license]

# Alice

Link to Alice's Adventures In Wonderland book: [https://www.adobe.com/be_en/active-use/pdf/Alice_in_Wonderland.pdf](https://www.adobe.com/be_en/active-use/pdf/Alice_in_Wonderland.pdf)  
All needed illustrations could be found at: [https://www.gutenberg.org/files/19778/19778-h/images/](https://www.gutenberg.org/files/19778/19778-h/images/)

## Getting started

1. Create [GitLab account](https://gitlab.com/users/sign_up). Strictly recommended pattern for the __username__: `name.lastname`, use your personal email (ex: `@gmail.com`) 
2. Create [Personal Access Token](https://gitlab.com/-/profile/personal_access_tokens) with `write_repository` scope
3. Request Access:  
![requestAccess](requestAccess.png)
4. Clone repository to your local machine
```
git clone https://{YOUR_TOKEN_NAME:TOKEN}@gitlab.com/iryna.v.afanasieva/alice.git
```
5. Create new branch, follow `feature/page-No` pattern, lets assume that your page number is 42:
```
git checkout -b feature/page-42
```
6. Add necessary page content into [AliceInWonderland.md](AliceInWonderland.md):
    - add solid line;
    - add page number;
    - add page content;
    - **Attention!** Redundant empty lines are not accepted
7. Commit changes: commit message should begin with `Page No:`
```
git status
git add .
git status
git commit -m "Page 42: {your changes description}"
```
8. Push your branch into repository:
```
git push -u origin feature/page-42
```
9. Create MR (Merge Request)
10. Resolve merge conflicts if needed
11. Wait for a review

## Additional Sources

- [Git tips](http://sixrevisions.com/web-development/git-tips/) — consolidate your knowledge of Git
- [Learn git branching](http://learngitbranching.js.org) — improve your understanding of branching
- [Markdown Guide](https://about.gitlab.com/handbook/markdown-guide/)

[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[license]: https://gitlab.com/gitlab-org/gitlab-foss/-/raw/master/LICENSE
