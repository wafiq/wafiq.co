# wafiq.co

### To develop

1. `git clone` in your working folder.
2. `bundle install` to download all dependencies.
3. `middleman s` to run development server, and open in `http://localhost:4567`

### To deploy

1. `middleman b` to build the static HTML output.
2. Add a file named `.s3_sync` and add AWS credential as following:

```
aws_access_key_id: AKIAXXX
aws_secret_access_key: pmkBwxxxxxxxx
```
3. Open `config.rb` file, around `activate :s3_sync` line, customize your AWS bucket and region.
