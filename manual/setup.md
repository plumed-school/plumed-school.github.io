# [Module](../manual.md): setup

| Description    | Usage |
|:--------|:--------:|
| Description of module | [![used in 8 tutorials](https://img.shields.io/badge/tutorials-8-green.svg)](https://www.plumed-tutorials.org/browse.html?search=setup)[![used in 149 eggs](https://img.shields.io/badge/nest-149-green.svg)](https://www.plumed-nest.org/browse.html?search=setup)|

## Actions 

The following actions are part of this module

{% assign moduleacts = site.data.actionlist | where: "module", "setup" %}
{:#browse-table .display}
| Name | Description |
|:--------:|:--------|
{% for item in moduleacts %}| [{{ item.name }}]({{ item.path }}) | {{ item.description }} |
{% endfor %}
<script>
$(document).ready(function() {
var table = $('#browse-table').DataTable({
  "dom": '<"search"f><"top"il>rt<"bottom"Bp><"clear">',
  language: { search: '', searchPlaceholder: "Search project..." },
  buttons: [
        'copy', 'excel', 'pdf'
  ],
  "order": [[ 0, "desc" ]]
  });
$('#browse-table-searchbar').keyup(function () {
  table.search( this.value ).draw();
  });
  hu = window.location.search.substring(1);
  searchfor = hu.split("=");
  if( searchfor[0]=="search" ) {
      table.search( searchfor[1] ).draw();
  }
});
</script>
