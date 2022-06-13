Variables.scss
--------

Changes:

Defines the overall colors

.. code-block::

    //colors
    $gray-lighter:                      #f5f7fa !default;
    $gray-light:                        #9b9b9b !default;
    
    $gray:                              #707070 !default;
    $gray-dark:                         #525252 !default;
    $gray-medium:                       #ebebeb !default;
    $gray-darker:                       #525252 !default;
    $sand:                              #ebebeb !default;
    $cool-white:                        #f8f8f8 !default;
    $primary:                           #cf202f !default;
    $secondary:                         $gray-darker !default;
    $success:                           #1C871E !default;
    $bg-success:                        #cee8d1 !default;
    $info:                              #525252 !default;
    $bg-info:                           #F5F7FA !default;
    $warning:                           #f39932 !default;
    $bg-warning:                        #F9F2DC !default;
    $danger:                            #FFFFFF !default;
    $bg-danger:                         #cf202f !default;
    $bg-main:                           $gray-lighter !default;
    $bg-main-ligther:                   $bg-main !default;
    $white:                             #ffffff !default;
    $black:                             #000000 !default;

    $dark:                              $gray-dark !default;
    $gray-100:                          $gray-lighter !default;
    $gray-500:                          $gray-light !default;
    $gray-600:                          $gray !default;
    $gray-700:                          $gray-dark !default;

    $yiq-text-dark:                     $gray-darker !default;
    $yiq-text-light:                    $gray-lighter !default;

    $bg-typeahead-fix:                  $white !important  !default;

    $theme-colors				: () !default;
    $theme-colors: map-merge((
            'gray'			: $gray,
            'gray-light'	: $gray-lighter,
            'gray-medium'	: $gray-medium,
            'gray-dark'		: $gray-light,
            'gray-darker'	: $gray-darker
    ), $theme-colors);

    // styles

    $highlight-border-size:             .375rem !default;

    $body-bg:                           $gray-100 !default;
    $body-color:                        $gray-700 !default;
    $table-color:                       $body-color !default;

    $copyright-bg-color:               $gray-dark !default;
    $footer-bg-color:                  $bg-main !default;
    $footer-color:                     $body-color !default;
    $header-bg-color:                  $white !default;
    $header-color:                     $body-color !default;

    $headings-color:                    $gray-700 !default;
    $navbar-light-hover-color:          $primary !default;

    $text-muted:                        $gray !default;
    $text-muted-header:                 $text-muted !default;
    $input-color-placeholder:           $gray !default;

Defnies the colors and decor of the links 
.. code-block::

    /* links */

    $link-color:                        $gray-darker !default;
    $link-decoration:                   underline !default;
    $link-hover-color:                  #24282a !important;
    $link-hover-decoration:             none !default;

    $border-radius:                     .125rem !default;
    $border-radius-lg:                  $border-radius !default;
    $border-radius-sm:                  $border-radius !default;

    $border-width:                      1px !default;
    $border-color:                      $gray-medium !default;


Defines the new font "Industry" located in /themes/base/fonts/
.. code-block::

    // font

    $line-height-base:                  1.5 !default;
    $nova-theme-path:                   ".." !default;
    $fa-font-path:                      "../base/fontawesome/webfonts" !default;
    $font-family-sans-serif:            'Industry', sans-serif !default;
    $font-accent:                       Industry, sans-serif !default;

    $font-size-base:                    rem(14px) !default;
    $font-size-lg:                      rem(16px) !default;
    $font-size-sm:                      rem(12px) !default;
    $font-size-xs:                      rem(11px) !default;

    $font-weight-lighter		: lighter !default;
    $font-weight-light			: 300 !default;
    $font-weight-normal			: 300 !default;
    $font-weight-semibold		: 600 !default;
    $font-weight-bold			: 900 !default;
    $font-weight-bolder			: bolder !default;

New color of info-button
.. code-block::

    .btn-info {
        color: #ffffff;
        background-color: #cf202f !important;
        border-color: #ffffff;
        box-shadow: none;
    }

Imports the above font into frontend
.. code-block::

    @import url("https://use.typekit.net/kue3yyf.css");
    body, .tooltip, .popover, .fa-sup, #footer .productlist-filter-headline {font-family: 'Industry', sans-serif;}

Change of color for warning singn e.g. empty cart or new price in cart or no shipping method in cart
.. code-block::

    .text-muted-util {
        color: #cf202f;
    }
    .alert-danger {
        color: #FFFFFF !important;
    }

Hides small blog image in News area
.. code-block::
    .blog-details .blog-details-image {
        display: none !important;
    }


