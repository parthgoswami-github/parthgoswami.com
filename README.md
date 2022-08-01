# Website

This website is built using Hugo (a static site generator) + github (to store your content) + netlify (to deploy your website). All tools are based on open source. 

### Installation

```
$ brew install hugo
# or
$ port install hugo
# To verify your new install:
$ hugo version
```

### Create a New Site

```
$ hugo new site quickstart
```

This command will create a new Hugo site in a folder named quickstart.

### Add a Theme

First, download the theme from GitHub and add it to your site’s themes directory:

```
$ cd themes
$ git clone https://github.com/dillonzq/LoveIt.git themes/LoveIt
```

Then, add the theme to the site configuration:
echo theme = \"LoveIt\" >> config.toml

### Local Development 

You can manually create content files (for example as content/<CATEGORY>/<FILE>.<FORMAT>) and provide metadata in them, however you can use the new command to do a few things for you (like add title and date):

```
hugo new posts/my-first-post.md
```

### Start the Hugo server

```
hugo server -D
```

Navigate to your new site at http://localhost:1313/

### Customize the Theme

Your new site already looks great, but you will want to tweak `config.toml` a little before you release it to the public.

### Build

It is simple. Just call:

```
$ hugo -D
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

You may use github to store the content and Netlify to host the website. 
