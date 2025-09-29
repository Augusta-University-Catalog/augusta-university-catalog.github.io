# Augusta University Catalog

This website complements Augusta University's [catalog page](http://catalog.augusta.edu/) by presenting its content as a navigable table.
It relies heavily on the [Modern-Campus-Catalog-Scraper](https://github.com/Augusta-University-Catalog/Modern-Campus-Catalog-Scraper) python script developed localy. 

> [!WARNING]  
> This website is still under active development, and does not aim at taking precedence over the "official catalog". 

## Local testing

You can deploy [the website locally](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll) to test it.
In short:

- [Install Jekyll](https://jekyllrb.com/docs/installation/),
- Clone this repository, enter it,
- Run

    ```
    gem install bundler jekyll
    bundle install
    bundle exec jekyll serve
    ```
- Navigate to <http://127.0.0.1:4000/>, or whichever URL is given in the terminal output.
