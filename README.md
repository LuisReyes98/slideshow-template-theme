# Slide Show Theme

JS less Slide Show component using [Fadeshow](https://github.com/alexerlandsson/css-fadeshow)

The Slide show default height is
100vh , to cover the full view port as a Hero Slider

the class for the height is:
``` .slideshow_height_ ```
overwrite it in your theme if you need a custom height


## Usage 
this theme is set up to work with [machu pichu](https://github.com/foundpatterns/machu-picchu)

### [Machu Pichu](https://github.com/foundpatterns/machu-picchu) set up
Open the terminal or command line in the same folder where you have donwload this theme once  there run:
``` 
mp unpack
```
That's it! you are ready to go

## Other info 

### css 
The css minified file for fadeshow should be  in 
```stylesheets/fadeshow/css```

### scss/sass
To use the fadeshow sass custom desing read the instruccions at [Fadeshow](https://github.com/alexerlandsson/css-fadeshow#customized-installation)
and then compile ```css-fadeshow.scss``` into ```stylesheets/fadeshow/css/css-fadeshow.min.css ```

#### How to compile the scss/sass
if you dont have sass you'll have to install it, [Install Sass](https://sass-lang.com/install)
open the terminal in the same folder as ```css-fadeshow.scss``` and then run the command 
```  
sass css-fadeshow.scss:../css/css-fadeshow.min.css --style compressed
```
to get a minified css file 

#### Known Scss Issues
In the last version of the scss of fadeshow the file ```theme-quicknav.scss```
that would be located at ```stylesheets/fadeshow/scss/theme/themes/classic/theme-quicknav.scss```
its broken in the line 8 here: 
```
  &:hover {
    opacity: 1;
  }
```
you can comment or erase these lines without any issues.

####Customize your own fadeshow 
if you wish to use your own forked version of fadeshow, just change the url at ```manifest.scl```
and add your own here
```
fadeshow = {
  url = "https://github.com/alexerlandsson/css-fadeshow", #your own forked url goes here
}
```