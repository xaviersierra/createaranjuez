## Developer set up

### Tools instalation

- Install the prerequisites listed in this [page](https://jekyllrb.com/docs/installation/)

### Build and run

``` sh
bundle exec jekyll serve
```

### Troubleshooting

- If when running the project, ask for install gitlab don't do it. Instead make sure that ruby is added to the classpath.
  Running:
  ``` sh
  PATH=$PATH:$HOME/.local/share/gem/ruby/3.0.0/bin
  ```
  Would temporary solve the issue in some linux environments
