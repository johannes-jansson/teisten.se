# teisten.se

Stand inside the site folder.

Install dependencies with `bundle install`. 
run with `jekyll serve --livereload`
or rather with `bundle exec jekyll serve --livereload`

To deploy run `jenv local 1.8` and then `s3_website push`.
https://www.andrewhoog.com/post/howto-install-s3_website-on-macos/

## Disabling Minification during Development
Minification takes time and significantly slows down development. To disable it, create a ` _config.dev.yml` file, and add the following contents:
```
jekyll-minifier:
  exclude: "*"
  ```

Then, start your development server using the following command:
```
jekyll serve --config _config.yml,_config.dev.yml  --incremenlal
```

