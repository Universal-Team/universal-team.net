---
title: Universal-Updater
image: "/assets/images/icons/universal-updater.png"
color: "#002F50"
repo: Universal-Team/Universal-Updater
redirect_from:
  - universal-updater
---

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script>
  $(document).ready(function() {
    $.getJSON('https://api.github.com/repos/Universal-Team/Universal-Updater/tags').done(function(json) {
      var release = json[0];
      var version = release.name;

      var n3dsxURL = 'https://github.com/Universal-Team/Universal-Updater/releases/download/'+version+'/Universal-Updater.3dsx'
      var ciaURL = 'https://github.com/Universal-Team/Universal-Updater/releases/download/'+version+'/Universal-Updater.cia'
      var releaseURL = 'https://github.com/Universal-Team/Universal-Updater/releases/tag/'+version

      $('#n3dsxDownload').attr('href', n3dsxURL);
      $('#ciaDownload').attr('href', ciaURL);
      $('#n3dsxDownload').attr('class', 'btn');
      $('#ciaDownload').attr('class', 'btn');
      $('#latestVersion').html(version)
      $('#latestVersion').attr('href', releaseURL);
    });
  });
</script>

# Universal-Updater

> A universally good updater for Nintendo 3DS.

Universal-Updater is a universally good updater. A description of it coming soon!

## Wiki
You can visit Universal-Updater's Wiki for more information about Universal-Updater and it's Features:

[Wiki](https://github.com/Universal-Team/Universal-Updater/wiki){: .btn}


## Download

You can find the download Link to Universal-Updater here:

Latest version is: [latest](https://github.com/Universal-Team/Universal-Updater/releases/latest){: #latestVersion}

[Download .3dsx](){: .btn .hidden #n3dsxDownload}
[Download .cia](){: .btn .hidden #ciaDownload}
[Release Page](https://github.com/Universal-Team/Universal-Updater/releases/latest){: .btn}

[Dowload nightly .3dsx](https://github.com/Universal-Team/extras/raw/master/builds/Universal-Updater/Universal-Updater.3dsx){: .btn}
[Dowload nightly .cia](https://github.com/Universal-Team/extras/raw/master/builds/Universal-Updater/Universal-Updater.cia){: .btn}

## Contact
The best way to talk to us is to join our Discord:

[![Discord](https://discordapp.com/api/guilds/568119817320792074/widget.png?style=banner2)](https://discord.gg/KDJCfGF)

## Credits
### Main Developers

- [Epicpkmn11](https://github.com/Epicpkmn11) : Helped me by the JSON parsing stuff and a lot more!
- [VoltZ](https://github.com/SuperSaiyajinVoltZ) : Main Developer of Universal-Updater.
### Translators

English
- [VoltZ](https://github.com/SuperSaiyajinVoltZ)

French
- [antoine62](https://github.com/antoine62)

German
- [VoltZ](https://github.com/SuperSaiyajinVoltZ)

Japanese
- [Epicpkmn11](https://github.com/Epicpkmn11)

Lithuanian
- [lemonnade0](https://steamcommunity.com/profiles/76561198276444028)

Spanish
- [YoSoy](https://twitter.com/riku200)
### Others

- [devkitPro](https://github.com/devkitPro), [Fincs](https://github.com/fincs), [Smealum](https://github.com/smealum), [WinterMute](https://github.com/WinterMute) : devkitARM, Libctru, Citro2D, and Citro3D.