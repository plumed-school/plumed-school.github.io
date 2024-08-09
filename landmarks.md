# Module: landmarks

| Description    | Usage |
|:--------|:--------:|
| Description of module | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=landmarks)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=landmarks)|

## Actions 

The following actions are part of this module

{% assign moduleacts = site.data.actionlist | where: "module", "landmarks" %}
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
