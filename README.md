# sven-cruises

## Building the site 
`hugo`

## Serving Locally
`hugo server`
`hugo server -D` to also include posts marked as draft.

## Creating new album
From the [autophugo readme](https://github.com/kc0bfv/autophugo/): 
Inside your project create the directory assets/NAME-OF-YOUR-ALBUM. Place all of one album's photos inside that directory.

`hugo new NAME-OF-YOUR-ALBUM/_index.md`

It will create an index file for your first album. Open content/NAME-OF-YOUR-ALBUM/_index.md with your text editor.

Change the title of your album if you wish, and set the filename of album's cover thumbnail. The filename is relative to the assets folder, so if your album is named dogs and one of your images there is named dog_01.jpg you can put dogs/dog_01.jpg in albumthumb to select it.

In addition to those frontmatter options, you can also specify metadata for some or all of your images. Do that by modifying the resources array with map elements. The maps specify the image they apply to with the src key, as src: "album/image.jpg". You can then specify some or all of the following items: alt, phototitle, and description. Demonstration of this is in the exampleSite directory albums.