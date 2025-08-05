# [BaRatin-tools.github.io](https://baratin-tools.github.io/)

Files used to build the website <https://baratin-tools.github.io/> with [Hugo](https://gohugo.io/) and the [blogdown](https://bookdown.org/yihui/blogdown/) R package.

The served static files are in folder /docs/

## Site rebuild instruction
To rebuild the site from scratch (removing pages not present anymore), remove docs folder
```bash
rm -r docs
```
Then in R, rebuild the site using rmarkdown (alternatively Build Website in the build tab of Rstudio can be used):
```R
rmarkdown::render_site(encoding = 'UTF-8')
```
To serve the site and check the pages locally do (prior to commit):
```R
blogdown::serve_site()
```