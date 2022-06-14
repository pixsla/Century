header-top-bar.top
------

Adds the logosand the redirection based on the site language
General styles for new custom div containers

.. code-block::

  <style>
  div#header-top-bar {
      padding-bottom: unset !important;
      padding-top: unset !important;
      padding-right: 8px;
      padding-left: 8px;
      height: 41px;
  }

      .justify-content-center.header_images {
          order: 1;
          max-width: 75%;
          flex: 0 0 75%;
          display: inline-flex;
          flex-wrap: wrap;
          align-items: center;
          justify-content: space-between !important;
      }
      .header_images-cst-1 img.topbar-icons {
              padding-right: 7px;
              width: 75px;
          }
  .header_images-cst-2 img.topbar-icons {
      padding-right: 4px;
      padding-left: 8px;
  }
  ul.nav.topbar-main.nav-dividers {
      display: flex;
      flex-wrap: wrap;
      padding-left: 0;
      margin-bottom: 0;
      list-style: none;
      align-items: center;
      max-width: 25%;
      flex: 0 0 25%;
  }
  body[data-page="11"] div#header-top-bar {
      display: block !important;
  }

  body[data-page="11"] div#header-top-bar .container-fluid.container-fluid-xl {
      display: none;
  }
      </style>

Adds the content to new "justify-content-center header_images" container
For german

.. code-bloc::

      {strip}
      <div class="justify-content-center header_images">
          <div class="header_images-cst-1">
                 {if $meta_language == "de"}
          <a href="https://www.century-europe.eu/Punok_1" title="Punok">
          <img class="topbar-icons" src="/media/image/storage/opc/top-bar/punoklogo.svg">
          </a><a href="https://www.century-europe.eu/Gameness" title="gameness">
          <img class="topbar-icons" src="/media/image/storage/opc/top-bar/gameness-logo-v3.png"> </a>
          <a href="https://www.century-europe.eu/Black-Belt-Magazin" title="blackbeltmag">
          <img class="topbar-icons" src="/media/image/storage/opc/top-bar/black-belt-logo.png"> </a> 
      {/if}
      
Adds the content to new "justify-content-center header_images" container
For englisch

.. code-block::

      {if $meta_language == "en"}
          <a href="https://www.century-europe.eu/Punok_2" title="Punok">
          <img class="topbar-icons" src="/media/image/storage/opc/top-bar/punoklogo.svg">
          </a><a href="https://www.century-europe.eu/Gameness_1" title="gameness">
          <img class="topbar-icons" src="/media/image/storage/opc/top-bar/gameness-logo-v3.png"> </a>
          <a href="https://www.century-europe.eu/Black-Belt-Magazin_1" title="blackbeltmag">
          <img class="topbar-icons" src="/media/image/storage/opc/top-bar/black-belt-logo.png"> </a>
      {/if}
          </div>
           <div class="header_images-cst-2">
              <img class="topbar-icons"src="/media/image/storage/opc/top-bar/united-states.png"><a href="https://www.centurymartialarts.com/">USA</a>
              <img class="topbar-icons"src="/media/image/storage/opc/top-bar/canada.png"><a href="https://www.centurymartialarts.ca/">CA</a>
          </div>
       </div>
