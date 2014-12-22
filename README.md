UnderStrap Wordpress Theme Framework
===

Live Demo: http://holgerkoenemann.de/understrap/

Changelog
=
                - 0.2 Dec. 22th 2014
                   - Adding Jasny Off-Canvas nav and Owl.Carousel Slider script
                   - Enqueue scipts and styled dynamically
                                   
                - 0.1 Dec. 10th 2014 - First commit

Basically I like the _s Wordpress Starter Theme from Automattic and the grid Framework Bootstrap. Additionally I´am a huge SASS/COMPASS fan. Why don´t combine all these three things into a solid Wordpress Theme Framework?
That´s what UnderStrap is (or will be...)

At the moment UnderStrap is in a very early stage. But if you wan´t feel free to use it for your own Wordpress theme!

Basic Features
=
- Combines the _s Wordpress Starter Theme and Bootstrap
- Comes with Bootstrap SASS source files and additonal scss files. Nicely sorted and ready to add your own variables/customize the Bootstrap variables.
- Uses a single and minified CSS file 
- Font Awesome Icon Font integrated (V 4.2.0): http://fortawesome.github.io/Font-Awesome/
- Off-Canvas navigation - By Jasny Bootstrap Plugin (V 3.1.3): http://jasny.github.io/bootstrap/
(activate it by adding a widget to widget position "Off Canvas" - It works but did not looks good at the moment... )
- Comes with extra slider script - By owl.carousel (V 2.0.0-beta.2.4): http://www.owlcarousel.owlgraphic.com/
- Simple RTL file
- Jetpack ready
- Child Theme ready (A basic starter Child Theme will be released in the future as a separate Repository)
- Translation ready

Starter Theme + HTML Framework = Wordpress Theme Framework
=
The _s theme is a good starting point to develope a Wordpress theme. But it is "just" a raw starter theme. Means it outputs all the Wordpress stuff correctly but without any layout or design.
Why don´t add a well known and supported layout framework to have a solid, clean and responsive foundation? Thats where Bootstrap comes in.

Confused by all the CSS and SCSS files?
=
Some basics about the SCSS and CSS files comes with UnderStrap:
- The theme itself uses the style.css in the root directory just to identify the theme inside of Wordpress. The file is not loaded by the theme and did not include any styles
- The theme.css file in /css/ subdirectory provides all styles. It is composed by six different SCSS sets and one variables file from /sass/ directory:

                  1./sass/underscores/understrap_underscores.scss (<- Basics for the _s theme)
                  2./sass/bootstrap/understrap_bootstrap.scss (<- which imports all Bootstrap SCSS files and mixins from /sass/bootstrap/ directory)
                  3./sass/understrap/understrap.scss (<- Just used minimal styles to combine _s and Bootstrap aand the other assets nicely)
                  4./sass/font-awesome/understrap_font-awesome.scss (<-imports all Font Awesome icons and the font itself)
                  --------------- Don´t edit the files above --------------- 
                  
                  5./sass/theme/theme.scss (<- Thats your part! Here you can add your own style) 
                  and
                  6.sass/theme/_theme_variables.scss (<- here you can define own variables or you could overwrite existing Bootstrap variables easily without touching the original BS code)

- Don´t edit the first four files/filesets or you aren´t able to update it without overwriting your own work!
- Your design goes into: /sass/theme directory. Add your styles to the theme.scss file and your variables to the _theme_variables.scss. Or add other scss files into it and @import it into theme.scss


