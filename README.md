```diff
- Repo updated to 2.X.X multi-language version.
# If your resume is broked, and you want use old version,
# in YOUR_REPO/_config.yml change this line
- remote_theme: annndruha/minimal-resume
# to this:
- remote_theme: annndruha/minimal-resume@v1.0.0
```

# Fork this repo for create your own web CV. ([Example](https://cv.annndruha.space/))
Launch your resume site without server on github pages! Optional need a domain name.

# Configuration

* Fork this repo as `<you_github_nickname>.github.io`
* Setup your domain (may skip this step and site be on `<you_github_nickname>.github.io`)
  * Create CNAME subdomain record on your DNS provider:
    * `cv` -> `<you_nickname>.github.io`
  * Open fork repository settings
  * Go to `Pages/Custom domain` enter you `cv.<example.com>` (And enforce HTTPS)
  * Change [CNAME-file](https://github.com/annndruha/annndruha.github.io/blob/main/CNAME) in fork with your subdomain: `cv.<example.com>`
* Change left side with your information via [_config.yml](./_config.yml) like this:
  ```yaml
  fullname: Andrey Marakulin
  favicon: /assets/images/favicon.svg
  logo: /assets/images/photo.png
  
  show_info: true # Show block with information
  age: 24 y.o.
  location: Moscow, Russia
  language: Russian, English
  
  show_contacts: true # Show block with buttons
  mailto: mailto:annndruha.github@gmail.com
  cv_pdf_link: https://raw.githubusercontent.com/Annndruha/annndruha.github.io/main/pdf/cv_pdf.pdf
  
  # Don't change this
  remote_theme: annndruha/minimal-resume
  plugins:
  - jekyll-remote-theme
  ```
* Change [index.md](./index.md) with you information
* Change `/assets/images/photo.png` and pdf link
* Wait a minute for GitHub-actions auto build and enjoy your site 😋!


# Extra

This site required page theme [minimal-resume](https://github.com/Annndruha/minimal-resume) which is in the [_config.yml](./_config.yml) as remote_theme.

Site hasn't got a pdf converter, manually update the pdf file: [cv_pdf.pdf](./pdf/cv_pdf.pdf)
