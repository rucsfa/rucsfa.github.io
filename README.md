# Rutgers University–Camden Student Finance Association

A static website with Home, About, and History pages. There are no build steps or package dependencies.

## Test locally

From the repository root, start a local server with Python 3.

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open [http://127.0.0.1:8000](http://127.0.0.1:8000). Use the navigation to visit all three pages. At a narrow viewport, check that the navigation and cards fit without horizontal scrolling. Tab through the links, check the Events link on Home, and verify the membership, Instagram, advisor, and past leadership links. Stop the server with Ctrl+C.

## Deploy with GitHub Pages

1. Commit the site files and push or merge them into `main`.
2. In the GitHub repository, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/ (root)**, then click **Save**. The root `.nojekyll` file lets GitHub Pages publish the static files directly.
4. Check the Pages deployment in **Actions**, then verify the site at [rucsfa.github.io](https://rucsfa.github.io/). Subsequent pushes to `main` trigger another deployment.

See [GitHub Pages publishing source documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) for setup details.

## Update content

Edit `index.html` for the home and events sections, `about.html` for the mission and advisor, and `history.html` for past leadership. Shared styling lives in `assets/site.css`. Update the header and footer in all three pages if a shared link changes.
