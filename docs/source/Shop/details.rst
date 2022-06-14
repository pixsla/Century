Product details page - details.tpl
-----

located in /child/productdetails/

hides short descritpion from original position
Hides lines 168-180

.. code-block::

  {* disbale short desc pixsla
                          {block name='productdetails-details-info-description-wrapper'}
                          {if $Einstellungen.artikeldetails.artikeldetails_kurzbeschreibung_anzeigen === 'Y' && $Artikel->cKurzBeschreibung}
                              {block name='productdetails-details-info-description'}
                                  {opcMountPoint id='opc_before_short_desc'}
                                  <div class="shortdesc" itemprop="description">
                                      {$Artikel->cKurzBeschreibung}
                                  </div>
                              {/block}
                          {/if}
                          {opcMountPoint id='opc_after_short_desc'}
                          {/block}
  *}
  
Adds short description after SKU
added on line 226

.. code-block::

   {* Pixsla Short Descritpion *}
                    {block name='productdetails-details-info-description-wrapper'}
                              {if $Einstellungen.artikeldetails.artikeldetails_kurzbeschreibung_anzeigen === 'Y' && $Artikel->cKurzBeschreibung}
                                  {block name='productdetails-details-info-description'}
                                      {opcMountPoint id='opc_before_short_desc'}
                                      <div class="shortdesc" itemprop="description">
                                          {$Artikel->cKurzBeschreibung}
                                      </div>
                                  {/block}
                              {/if}
                              {opcMountPoint id='opc_after_short_desc'}
                              {/block}
  {* Pixsla end *}
  
Insert Klarna Banner in german and englisch on line 317

.. code-block::

  {* insert Klarna banner *}
  {if $meta_language == "de"}								
  {literal}
  <script
    async
    src="https://eu-library.playground.klarnaservices.com/lib.js"
    data-client-id="29b0834e-6f5e-5b6f-90ce-6cda38c383ea"
  ></script>
  <!-- Placement v2 -->
  <klarna-placement
    data-key="top-strip-promotion-auto-size"
    data-locale="de-DE"
  ></klarna-placement>
  <!-- end Placement -->
  {/literal}
  {/if}
  {if $meta_language == "en"}
  {literal}
  <script
    async
    src="https://eu-library.playground.klarnaservices.com/lib.js"
    data-client-id="29b0834e-6f5e-5b6f-90ce-6cda38c383ea"
  ></script>
  <!-- Placement v2 -->
  <klarna-placement
    data-key="top-strip-promotion-auto-size"
    data-locale="en-DE"
  ></klarna-placement>
  <!-- end Placement -->
  {/literal}
  {/if}
