tangrammer.github.com
=====================
this is the public repo accesible from [http://tangrammer.github.io/](http://tangrammer.github.io/)

Blog powered by cryogen is [https://github.com/tangrammer/cryogen-blog](https://github.com/tangrammer/cryogen-blog)

### Instructions to make changes
```
git clone git@github.com:tangrammer/cryogen-blog.git your-blog
git clone git@github.com:tangrammer/tangrammer.github.com.git your-blog/resources/public
cd your-blog
lein ring server
.... edit your site to get new web version ....
... and push changes to both repos ....
git add . && git commit -am "WIP" && git push
cd resources/public &&  git add . && git commit -am "WIP" && git push && cd ../../

```

### .gitignore needs following line extra
```
/resources/public
```


### resources/templates/config.edn change :blog-prefix and add README.md to :resources
``` :blog-prefix      "" ```
``` :resources        ["css" "js" "404.html" "README.md"] ```
