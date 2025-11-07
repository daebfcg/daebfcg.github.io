# DAEBFCG

Luthiery and Musical Projects blog

## Overview

A blog site done using the following tech:

* hugo
* github actions
* hosted on github pages


## Creating a new post
Run this command
```sh
hugo new --kind post-bundle posts/<DATE>
```
This will create new folder for the page bundle with an index.md.  Edit the index.md. Change the title and date as needed.  Don't forget to set draft to false.  

### Pictures
Put any pictures for the post directly into this new post folder.

If they are straight off the phone run this to scale them down to reasonable file size:

```sh
find . -maxdepth 1 -iname "PXL_*.jpg" -exec convert -set filename:f '%t' -resize 50% {} ./web_%[filename:f].jpg \;
```

Then rename the `web_` photos as desired and place thm on the page using this shortcode:

```
{{<imgresize filename.png "800x800" "alt text here">}}
```

In general, use 800 for horizontals and 600 for verticals.

## Other static images

* put the image under the `static/resources/` directory in the repo
* use the `image` shortcode found [here](https://github.com/panr/hugo-theme-terminal#built-in-shortcodes)
* set src to `/resources/<image-name.png>`
* when the site builds, you should now see your image.

## Development

First time cloning, run `git submodule update --init`.

You can use the custom dev container that exists in order to run this site locally.
From within the devcontainer terminal just run the following:

```sh
hugo server
```

And it will start a development server of the site with hot reload functionality
