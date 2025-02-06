# koha_staff_branding

Custom CSS to modify colors in the Koha staff client to match your brand colors

This css can be added to the IntranetUserCSS system preference in Koha to modify the colors in your Koha staff client.

Updated on 2025-02-06 to account for changes in Koha 24.11

The color variables in this file are based on the colors we use at Next Search Catalog and are as follow:

| Color | variable name | Color ID |
|-----|-----|-----|
| dark color |  `--c_dark` | #0157b9 |
| dark text |  `--t_dark` | #FFFFFF |
| dark hover color |  `--c_dark_hov` | #04368e |
| dark hover text |  `--t_dark_hov` | #FFFFFF |
| medium color | `--c_medium` | #1f9bde |
| medium text | `--t_medium` | #FFFFFF |
| medium hover color | `--c_medium_hov` | #0157b9 |
| medium hover text | `--t_medium_hov` | #FFFFFF |
| light color | `--c_light` | #d7ebff |
| light text | `--t_light` | #000000 |
| light hover color | `--c_light_hov` | #1f9bde |
| light hover text | `--t_light_hov` | #FFFFFF |
|-----|-----|-----|
| general text color | `--general_text` | #000000 |
| general link color | `--general_link` | #04368e |
|-----|-----|-----|
| header color | `--c_head` | #FFFFFF |
| header text | `--t_head` | #000000 |
| header hover color | `--c_head_hov` | #e0e0e0 |
| header hover text | `--t_head_hov` | #000000 |

I used [A11Y - Color blindness empathy test](https://addons.mozilla.org/en-US/firefox/addon/a11y-color-blindness-test/) and [Venngage's Accessible Color Palette Generator](https://venngage.com/tools/accessible-color-palette-generator) to take the colors from our logo and create a palatte that would look good with our logo and be accessible for people that might have vision issues.

To set different colors for your library, find the section labeled "root" in the css file, then replace my hexidecimal color codes with your own.

```css

  /* root section sets Brand colors */

  :root {

    /* Dark */
    --c_dark: #0157b9;
    --t_dark: #FFFFFF;

    --c_dark_hov: #04368e;
    --t_dark_hov: #FFFFFF;

    /* Medium */
    --c_medium: #1f9bde;
    --t_medium: #FFFFFF;

    --c_medium_hov: #0157b9;
    --t_medium_hov: #FFFFFF;

    /* Light */
    --c_light_hov: #1f9bde;
    --t_light_hov: #FFFFFF;

    --c_light: #d7ebff;
    --t_light: #000000;


    /* Colors for header */
    --c_head: #FFFFFF;
    --t_head: #000000;

    --c_head_hov: #e0e0e0;
    --t_head_hov: #000000;

    /* Text colors */
    --general_text: #000000;
    --general_link: #04368e;

  }


```