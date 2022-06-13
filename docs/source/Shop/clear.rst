clear.scss
--------
(my-nova) 
Changes:


Imports custom font in diverent areas of frontend
.. code-block::
    @import url("https://use.typekit.net/kue3yyf.css");
    body, .tooltip, .popover, .fa-sup, #footer .productlist-filter-headline {font-family: 'Industry', sans-serif;}


    .text-muted-util {
        color: #cf202f;
    }

    .btn-info {
        color: #FFFFFF;
        background-color: #cf202f;
        border-color: #FFFFFF;
        box-shadow: none;
    }
    
Primary Button of the shop e.g. add-to-cart or call-to-action
.. code-block::
    .btn-primary {
        color: #FFFFFF;
        background-color: #cf202f;
        border-color: #FFFFFF;
    }
    .yousave {
        font-weight: bold;
    }
    .btn-primary:hover {
        color: #ffffff;
        background-color: #cf202f;
        border-color: #ffffff;
        box-shadow: none;
    }
    
Warning button
.. code-block::

    .alert-danger {
        color: #FFFFFF !important;
    }
