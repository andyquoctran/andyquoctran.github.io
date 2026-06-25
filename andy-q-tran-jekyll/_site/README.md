# andy q tran — Jekyll website

A minimal two-page personal website for GitHub Pages. The background is `#121212`, matching the attached color.

## Put it on GitHub Pages

1. Create a new GitHub repository. For your main personal site, name it `YOUR-USERNAME.github.io`.
2. Upload **the contents of this folder** to the repository root. Do not upload the enclosing folder itself.
3. On GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose the `main` branch and the `/ (root)` folder, then save.
6. GitHub will publish the site after a minute or two.

For a repository named `YOUR-USERNAME.github.io`, your site will be at:

```text
https://YOUR-USERNAME.github.io
```

For a normally named project repository, it will be at:

```text
https://YOUR-USERNAME.github.io/REPOSITORY-NAME/
```

The site already supports either setup.

## Edit the text

- Edit `index.md` for the **me** page.
- Edit `research.md` for the **research** page.
- Everything below the `---` lines at the top of each file is the visible page text.

You can write in Markdown:

```md
# Big heading
## Smaller heading
**bold**
[a link](https://example.com)
- a list item
```

## Add a picture on the right

1. Put an image in `assets/images/`, such as `me.jpg`.
2. At the top of `index.md`, replace the commented lines with:

```yaml
image: /assets/images/me.jpg
image_alt: A photo of Andy Q. Tran
```

Do the same in `research.md` for a separate research image.

## Write LaTeX

MathJax is already included. Use `$...$` for inline math and `\[ ... \]` or `$$ ... $$` for displayed math:

```md
Inline: $W^r_d$

Display:
\[
r(D) - r(K-D) = \deg(D) + 1 - g.
\]
```

## Preview the site locally (optional)

This is only for when you want to test changes on your own computer.

1. Install Ruby, then run:

```bash
bundle install
bundle exec jekyll serve
```

2. Open `http://localhost:4000` in your browser.

You do not need to do this for GitHub Pages; GitHub builds the site for you.
