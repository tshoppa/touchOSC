
# touchOSC script minifier

A lua minifier for touchOSC templates based on [lua-minify by stravant](https://github.com/stravant/lua-minify)

# usage

1. Copy the Minifier Control to your template
2. Run the minifier's script **from the script box** (use the little play button on the bottom right of the script box.) **Do not run the template**, vastly replacing script code during runtime might crash touchOSC
3. remove the minifier control and save the template

# options

You can customize the minifier in the minifier's script:

## minifying targets
If you just want to minify scripts of specific controls, add them to the *toMinify* table with their full path. Example:

    local toMinify = {
      root,
      root.children.container.children.button
    }

will minify the root script and the button's script.
To minify scripts of all controls in the template leave the table empty.

    local toMinify = {
    }

## exclude function names
By default, the minifier substitutes function names with shorter names. If you want function names to be excluded from that, add them to the *exclude* table.
**Do not remove the callback function names** included by default. TouchOSC won't work properly if these are minified. 

## dry run
If you just want to see the result without actually replacing scripts in your template, set *printOnly* to true. The minimized code will be printed out in the log console.
