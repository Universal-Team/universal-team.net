---
title: pkmn-chest
image: "/assets/images/icons/pkmn-chest.png"
color: "#BF0300"
repo: Universal-Team/pkmn-chest
redirect_from:
  - pkmn-chest
  - pokemon-chest
---

<style>
.gallery { width: 512px }
.gallery .gallery-thumbnails img {
  width: 64px;
  margin: 3px 10px 10px 0;
  padding: 0;
  transition: 0.2s;
}
.gallery .gallery-thumbnails img:hover {
  box-shadow: #BF0300 2px 2px 4px;
  cursor: pointer;
}
#preview {
  display:block;
  margin:0 auto;
}
</style>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script>
  $(document).ready(function() {
    $.getJSON('https://api.github.com/repos/Universal-Team/pkmn-chest/tags').done(function(json) {
      var release = json[0];
      var version = release.name;

      var ndsURL = 'https://github.com/Universal-Team/pkmn-chest/releases/download/'+version+'/pkmn-chest.nds'
      var ciaURL = 'https://github.com/Universal-Team/pkmn-chest/releases/download/'+version+'/pkmn-chest.cia'
      var releaseURL = 'https://github.com/Universal-Team/pkmn-chest/releases/tag/'+version

      $('#ndsDownload').attr('href', ndsURL);
      $('#ciaDownload').attr('href', ciaURL);
      $('#ndsDownload').attr('class', 'btn');
      $('#ciaDownload').attr('class', 'btn');
      $('#latestVersion').html(version)
      $('#latestVersion').attr('href', releaseURL);
    });
  });
</script>

# Pokémon Chest
> A Pokémon Bank for 4th and 5th generation Pokémon games for the Nintendo DS(i).

Pokémon Chest is an app for the DS(i) that can store and edit Pokémon in the DS Pokémon games.
It's current features include:
- Loading save files from DSi SD, Flashcard SD, and retail cartridges
- Storing up to 50<sup>(Flashcards)</sup> or 500<sup>(DSi/3DS)</sup> boxes of Pokémon per chest with support for multiple chests
- Editing most Pokémon, trainer, and other save data
- Injecting pk4/pk5 files from SD
- Dumping Pokémon to pk4/pk5 files
- Translated to English, French, German, Italian, Japanese, Korean\*, Lithuanian\*\*, Portuguese, Russian\*\*, and Spanish
    - \*(the Korean translation is not complete)
    - \*\*(some character graphics are currently missing)

## Download
[Download .nds](){: .btn .hidden #ndsDownload}
[Download .cia](){: .btn .hidden #ciaDownload}
[Release Page](https://github.com/Universal-Team/pkmn-chest/releases/latest){: .btn}

Latest version is: [latest](https://github.com/Universal-Team/pkmn-chest/releases/latest){: #latestVersion}

[Dowload nightly .nds](https://github.com/Universal-Team/extras/raw/master/builds/pkmn-chest/pkmn-chest.nds){: .btn}
[Dowload nightly .cia](https://github.com/Universal-Team/extras/raw/master/builds/pkmn-chest/pkmn-chest.cia){: .btn}

## Screenshots
<div class="gallery">
  <div class="preview">
    <img id="preview" src="/assets/images/pkmn-chest/topMenu1.png" alt="Preview image" height="194" width="258"/>
  </div>
  <div class="gallery-thumbnails" style="margin:0 auto;text-align:center;width:512px;">
    <img onclick="document.getElementById('preview').src = document.getElementById('img0').src;" id="img0" src="/assets/images/pkmn-chest/topMenu1.png" alt="Top Menu (Top Screen)"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img1').src;" id="img1" src="/assets/images/pkmn-chest/topMenu2.png" alt="Top Menu (Bottom Screen)"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img2').src;" id="img2" src="/assets/images/pkmn-chest/box1.png" alt="Box (Top Screen)"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img3').src;" id="img3" src="/assets/images/pkmn-chest/box2.png" alt="Box (Bottom Screen)"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img4').src;" id="img4" src="/assets/images/pkmn-chest/wallpaper.png" alt="Wallpaper"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img5').src;" id="img5" src="/assets/images/pkmn-chest/xMenu.png" alt="X Menu"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img6').src;" id="img6" src="/assets/images/pkmn-chest/options.gif" alt="Options"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img7').src;" id="img7" src="/assets/images/pkmn-chest/party.png" alt="Party"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img8').src;" id="img8" src="/assets/images/pkmn-chest/summary.png" alt="Summary"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('img9').src;" id="img9" src="/assets/images/pkmn-chest/species.png" alt="Species"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('imgA').src;" id="imgA" src="/assets/images/pkmn-chest/natures.png" alt="Natures"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('imgB').src;" id="imgB" src="/assets/images/pkmn-chest/balls.png" alt="Balls"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('imgC').src;" id="imgC" src="/assets/images/pkmn-chest/forms.png" alt="Forms"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('imgD').src;" id="imgD" src="/assets/images/pkmn-chest/moves.png" alt="Moves"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('imgE').src;" id="imgE" src="/assets/images/pkmn-chest/stats.png" alt="Stats"/>
    <img onclick="document.getElementById('preview').src = document.getElementById('imgF').src;" id="imgF" src="/assets/images/pkmn-chest/origin.png" alt="Origin"/>
  </div>
</div>

## Contact
The best way to talk to us is to join our Discord:

[![Discord](https://discordapp.com/api/guilds/568119817320792074/widget.png?style=banner2)](https://discord.gg/KDJCfGF)

If you want to report a bug you can do so [here](https://github.com/Universal-Team/pkmn-chest/issues/new/choose).

## Credits
### Main Developers
- [Epicpkmn11](https://github.com/Epicpkmn11): GUI code, porting PKSM's save and bank management code
### Translators
- [antoine62](https://github.com/antoine62): French
- [Chips](https://github.com/Ch1p5): Portuguese, some Spanish and French
- [David Pires](https://github.com/DavidPires): Portuguese
- [edo9300](https://github.com/edo9300): Italian
- [Epicpkmn11](https://github.com/Epicpkmn11): English and Japanese
- [Extocine](https://twitter.com/@ExtocineN): Russian
- [lemonnade0](https://steamcommunity.com/profiles/76561198276444028): Lithuanian
- [NightYoshi370](https://github.com/NightYoshi370/): French
- [VoltZ](https://github.com/SuperSaiyajinVoltZ): German
### Others
- [devkitPro](https://github.com/devkitPro), [WinterMute](https://github.com/WinterMute): devkitARM, libnds, and libfat
- [edo9300](https://github.com/edo9300): [ndsi-savedumper](https://github.com/edo9300/ndsi-savedumper)'s gamecard save dumping and injecting code
- [Flagbrew](https://github.com/FlagBrew): [PKSM](https://github.com/FlagBrew/PKSM)'s save and bank management code
- [RocketRobz](https://github.com/RocketRobz): Adding flashcard and SD being used together and code from [TWiLight Menu++](https://github.com/DS-Homebrew/TWiLightMenu)
- [TotallyNotGuy](https://github.com/TotallyNotGuy): Finding & making graphics and the Pokémon Center generation 4 song
- [VoltZ](https://github.com/SuperSaiyajinVoltZ): Idea to make a Pokémon Bank for the DS(i)
### Music
- [Pokémon Center (Gen 1)](https://modarchive.org/module.php?181718), [Elm's Lab](https://modarchive.org/module.php?181711), [Oak's Lab](https://modarchive.org/module.php?181717), [Game Corner](https://modarchive.org/module.php?181756), and [Twinleaf Town](https://modarchive.org/module.php?178770).
