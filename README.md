
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

- The href, src path `title`, `project category`, and `project-name` would need updating — if changing out any of the images. The file name under assets needs to match the file path for href and src in the html.

## After updating in Visual Studio Code, commit and deploy changes to Github, via terminal:

Type in the terminal, cd ~ and click return
Type, ls and click return 
Type cd Desktop and click return
Type ls and click return
You will now see all of your files listed that you have on your Desktop.
Type cd peterperspective.github.io-main (or whatever the site file name is that you previously downloaded on your Desktop)

git status and click return
git add [add files] and click return
git status and click return
git commit and click return
(Opens commit window in new tab. type commit message, save and close tab)
Type `git push peterperspective main`, return

The changes will be live on website (may take a few minutes, and a hard-refresh of browser)
https://peterperspective.github.io