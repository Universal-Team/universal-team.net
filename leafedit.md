---
color: "#04b324"
repo: Universal-Team/LeafEdit
redirect_from:
  - leafedit
---

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script>
  $(document).ready(function() {
    $.getJSON('https://api.github.com/repos/Universal-Team/LeafEdit/tags').done(function(json) {
      var release = json[0];
      var version = release.name;

      var n3dsxURL = 'https://github.com/Universal-Team/LeafEdit/releases/download/'+version+'/LeafEdit.3dsx'
      var ciaURL = 'https://github.com/Universal-Team/LeafEdit/releases/download/'+version+'/LeafEdit.cia'
      var releaseURL = 'https://github.com/Universal-Team/LeafEdit/releases/tag/'+version

      $('#n3dsxDownload').attr('href', n3dsxURL);
      $('#ciaDownload').attr('href', ciaURL);
      $('#n3dsxDownload').attr('class', 'btn');
      $('#ciaDownload').attr('class', 'btn');
      $('#latestVersion').html(version)
      $('#latestVersion').attr('href', releaseURL);
    });
  });
</script>

# LeafEdit

> A Work in progress Animal Crossing: New Leaf Save Manager and Editor for the Nintendo 3DS.

LeafEdit is a work in progress Animal Crossing: New Leaf Save Manager and Editor for the Nintendo 3DS!


## Wiki
A Wiki for LeafEdit is planned. 


## Download
Here you can find the Download Links to LeafEdit. You can also get the latest Universal-Manager Nightly to download LeafEdit from it. ;)

Latest version is: [latest](https://github.com/Universal-Team/LeafEdit/releases/latest){: #latestVersion}

[Download .3dsx](){: .btn .hidden #n3dsxDownload}
[Download .cia](){: .btn .hidden #ciaDownload}
[Release Page](https://github.com/Universal-Team/LeafEdit/releases/latest){: .btn}

[Dowload nightly .3dsx](https://github.com/Universal-Team/extras/raw/master/builds/LeafEdit/LeafEdit.3dsx){: .btn}
[Dowload nightly .cia](https://github.com/Universal-Team/extras/raw/master/builds/LeafEdit/LeafEdit.cia){: .btn}


## Screenshots
Screenshots are coming soon!


## Contact
The best way to talk to us is to join our Discord:

[![Discord](https://discordapp.com/api/guilds/568119817320792074/widget.png?style=banner2)](https://discord.gg/KDJCfGF)

If you want to report a bug you can do so [here](https://github.com/Universal-Team/LeafEdit/issues/new/choose).