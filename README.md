# imouto.is-cute.moe

A (cute) static link shortener, powered by [Suri](https://github.com/jstayton/suri).

## 📃 About
[imouto.is-cute.moe](https://imouto.is-cute.moe) is a fork of [Suri](https://github.com/jstayton/suri) to host URLs from [is-cute](https://github.com/is-cute).

This repository is deployed to GitHub pages. Changes made to the [`master`](https://github.com/is-cute/suri/tree/master) branch are automatically compiled with a custom workflow and written to the [`gh-pages`](https://github.com/is-cute/suri/tree/gh-pages) branch.

## 🔗 List of Public URLS
| Path         | Host URL                              | Description      |
| :----------- | :------------------------------------ | :--------------- |
| /            | https://derpie.is-cute.moe            | Root domain      |
| /tablet-area | https://hitori.is-cute.moe/ATy3xI.png | osu! Tablet Area |

## 🌠 Deployment
> **Note**  
> You can find full deployment instructions in the [official repository](https://github.com/jstayton/suri).
>
> *This section will cover additional details not found there.*

### Static Hosting with GitHub Pages
> **Note**  
> You can find the workflow to use for your own project [here](https://raw.githubusercontent.com/is-cute/suri/master/.github/workflows/main.yml). 

Copy the [source repository](https://github.com/jstayton/suri) and create a workflow file under `.github/workflows/build.yml`. This will be the file used by GitHub Actions to compile your new build whenever changes are made.

Your website should be deployed from the `gh-pages` branch.

### Managing Links
Links are managed through `src/links.json`. An example config can be found below or in the [source repo](https://github.com/jstayton/suri/blob/master/src/links.json).

```json
{
  "/": "https://derpie.is-cute.moe",
  "/bocchi": "https://bocchi.is-cute.moe",
  "/localhost": "http://127.0.0.1"
}
```
> **Note**  
> In this example, `yourdomain.com/` would take you to https://derpie.is-cute.moe, while `yourdomain.com/localhost` would take you to http://127.0.0.1.
