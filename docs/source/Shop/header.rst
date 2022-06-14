header.tpl
-------------

located in /child/layout/
Changes onscroll head and footer color to carcoal

.. code-block::

  {extends file="{$parent_template_path}/layout/header.tpl"}

  {block name='layout-header-head-theme-color'}
  <meta name="theme-color" content="{if $Einstellungen.template.theme.theme_default === 'clear'}#cf202f{else}#1C1D2C{/if}">
  {/block}
