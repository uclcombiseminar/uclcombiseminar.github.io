# Built-in Features

* To access custom definition styling, use the format `<span class="defn">content</span>`
* Call box styling with `<div class="boxed">content</div>`
* All hard returns in markdown files automatically generate paragraph breaks with space between them.
* By default, horizontal lines for section breaks are light grey with built in margin.
* To create a separate footnotes section, insert a horizontal line at the bottom of your blog post.
* To designate a page-specific social image, use `image: url-path-to-image` in your liquid. NOTE: only insert the portion of the path after the images directory. * Mobile compatible

# Editing How-To

I made style customization easy with variables. Go to sass -> variables to adjust the color palette, font choices, content width, and mobile breakpoints.

If you'd like to make your own variable, the syntax is `$variable-name: variable-value;`. Whenever you want to call that value, the syntax is `css-selector: $variable-name;`

All sizing, aside from base font size and fixed widths, is sized in rems. These are relative units that scale using the base font size as their constant (1rem = base font size). Sticking to rems when adjusting your sizing ensures your site is more responsive and proportionally constant across various screen and window sizes.

The logo svg file (icon.svg) affects both the navigation logo and the browser icon. To change the color, open the svg file and change `fill:#00b595` to your new accent color. To change the color of the alef itself, change `stroke:#fff`, and to make it thicker or thinner, change `stroke-width:8px`.

# Individualized Layout Styling

The "base" stylesheet applies to the entire site. The "nav" stylesheet applies to the nav bar across the site.

All {{content}} is wrapped in `<main>` tags so it accesses base main content styling. Layouts with special formatting have a class added to their main tag (note: the post layout is wrapped in a highest level div instead, because it's derived from the default layout). Those class names correspond to a stylesheet of the same name in the sass directory.

The formatting in these layout stylesheets is layout-specific.

# Current Pages
* math blog
* about
