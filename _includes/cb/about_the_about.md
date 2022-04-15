{% comment %}
    Find some sample images or use defaults for About demos
{% endcomment %}
{% assign imagesample = site.data[site.metadata] | where_exp: 'item','item.format contains "image"' | first %}
{% capture imagesampleid %}{{ imagesample.objectid | default: "https://www.lib.uidaho.edu/collectionbuilder/demo-objects/mg101_b6_photographs_01.jpg" }}{% endcapture %}
{% assign pdfsample = site.data[site.metadata] | where_exp: 'item','item.format contains "pdf"' | first %}
{% capture pdfsampleid %}{{ pdfsample.objectid | default: "https://digital.lib.uidaho.edu/utils/getfile/collection/ui_ep/id/21768/filename/uiext21768.pdf" }}{% endcapture %}
{% assign videosample = site.data[site.metadata] | where_exp: 'item','item.format contains "video"' | first %}
{% capture videosampleid %}{{ videosample.objectid | default: "https://cdil.lib.uidaho.edu/storying-extinction/objects/trailcams/videos/ballcreek-cedarrub-birdonpath.mp4" }}{% endcapture %}
{% assign audiosample = site.data[site.metadata] | where_exp: 'item','item.format contains "audio"' | first %}
{% capture audiosampleid %}{{ audiosample.objectid | default: "https://www.lib.uidaho.edu/digital/mp3s/Clouds.mp3" }}{% endcapture %}


## About the Stillwell collection and this website

The Richard Stillwell Collection consists of ~ 1200 photographic negatives, organized by location.

This digital exhibition would not have been possible without the work of: Jacob Wheeler ’20, Phoebe Park ’21, Sophie Evans ’21, John Blazejewski and Julia Gearhart. 

A special thanks to the tremendous cataloguing work of Virginia French, the personal insight, knowledge and encouragement of Dr. William Childs, and to Dr. Camilla McKay for examining the collection and identifying the handwriting of Agnes Newhall Stillwell.  

For inquiries please email: resphotos@princeton.edu
