
# How to make updates to this repo

## Download site files to your local computer

- Click on the 'peterperspective.github.io' repo
- Click on the green 'Code' button and a dropdown menu appears, click on 'Download ZIP,' save somewhere on your computer. I recommend the Desktop. Open ZIP file (these are all of the files that make up the website).
- under /dist/assets/img/portfolio/fullsize are all of the images for the portfolio section in order.
- open the index.html file in Visual Studio code, the portfolio section is under the <!-- Portfolio --> comment section
the HTML for each card looks like this:

```
<div class="col-lg-4 col-sm-6">
    <a class="portfolio-box" href="dist/assets/img/portfolio/fullsize/1.jpg" title="Health Awareness - SVA, NYC">
        <img class="img-thumbnail" src="dist/assets/img/portfolio/fullsize/1.jpg" alt="" />
        <div class="portfolio-box-caption">
            <div class="project-category text-wclicke-50">Illustration</div>
            <div class="project-name">Health Awareness - SVA, NYC</div>
        </div>
    </a>
</div>
```

- The image files names and copy under `href`, `src` path, `title`, `project category`, and `project-name` would need updating — if changing out any of the images. The file name under assets needs to match the file path for href and src in the html.

## Before updating the content (html, images, etc.)

- Type in the terminal, cd ~ and click return
- Type, `ls` and click return 
- Type `cd Desktop` and click return
- Type `ls` and click return
- You will now see all of your files listed that you have on your Desktop.
- If you saved the website file in another location on your computer, repeat the steps to type `ls` return, and type `cd [file-name]` return, type `ls` return, until you see the new website folder downloaded from Github
- Type `cd peterperspective.github.io-main` (or whatever the site file name is that you previously downloaded on your Desktop)
- Type `git pull`and click return. If anyone else made any edits to your repo, this command will pull them down to your local computer folder

## After updating files in Visual Studio Code

### Login into Github via the terminal:
(Should only need to do the first time, per computer)

- Type `git config --global user.email peterperspective@gmail.com`

### Commit and deploy changes to Github, via terminal:
(Repeat everytime updating website)

- `git status` and click return
- `git add` [add files] and click return
- `git status` and click return
- `git commit` and click return
(Opens commit window in new tab. type commit message, save and close tab)

- For the first time, per computer, type `git push https://github.com/peterperspective/peterperspective.github.io.git`
- Now type username and password and it should be saved by git.

For continuous updates, type `git push peterperspective.github.io main`, return

The changes will be live on website (may take a few minutes, and a hard-refresh of browser)
https://peterperspective.github.io

## Additional readings 

### Getting started with Git
https://docs.github.com/en/get-started/getting-started-with-git 

#### Git cheatsheat
https://training.github.com/downloads/github-git-cheat-sheet/

#### Set up Git for new repos
https://docs.github.com/en/get-started/getting-started-with-git/set-up-git

