---
title: LeafEdit
image: "/assets/images/icons/leafedit.png"
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

## Credits
### Main Developers
- [VoltZ](https://github.com/SuperSaiyajinVoltZ): App Idea and Main Developer.
### Translators

English
- [Epicpkmn11](https://github.com/Epicpkmn11)
- [VoltZ](https://github.com/SuperSaiyajinVoltZ)

French
- [antoine62](https://github.com/antoine62)

German
- [VoltZ](https://github.com/SuperSaiyajinVoltZ)

Italian
- [edo9300](https://github.com/edo9300)

Japanese
- [Epicpkmn11](https://github.com/Epicpkmn11)

Lithuanian
- [lemonnade0](https://steamcommunity.com/profiles/76561198276444028)

Portuguese
- [Chips](https://github.com/Ch1p5)
- [David Pires](https://github.com/DavidPires)

Spanish
- [Daniyel33](https://github.com/Daniyel33)
- [YoSoy](https://twitter.com/riku200)

### Others

- [Cuyler](https://github.com/Cuyler36), [Slattz](https://github.com/Slattz), [NLTK](https://github.com/Slattz/NLTK) : For the Core part and the Acres, Items and Villager Sprites!
- [devkitPro](https://github.com/devkitPro), [Fincs](https://github.com/fincs), [Smealum](https://github.com/smealum), [Wintermute](https://github.com/WinterMute) : For devkitARM, Citro2D, Citro3D and Libctru.
- [Flagbrew](https://github.com/FlagBrew): [Checkpoint](https://github.com/FlagBrew/Checkpoint)'s Code for the Backup & Restore part for Animal Crossing: New Leaf.
- [Flagbrew](https://github.com/FlagBrew): [PKSM](https://github.com/FlagBrew/PKSM)'s Title Code, to get the Title ID for Animal Crossing : New Leaf and such.
- [Flame](https://github.com/FlameKat53): The Name Idea of LeafEdit.
- [Kodtiz3D](https://github.com/Kodtiz3D): For the Icon and the Banner.
