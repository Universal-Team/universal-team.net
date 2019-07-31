---
color: "#bf0300"
repo: Universal-Team/pkmn-chest
redirect_from:
	- pkmn-chest
	- pokemon-chest
---

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script>
	$(document).ready(function() {
			$.getJSON('https://api.github.com/repos/Universal-Team/pkmn-chest/tags').done(function(json) {
				var release = json[0];
				var version = release.name;
				if(version) {
					var ndsURL = 'https://github.com/Universal-Team/pkmn-chest/releases/download/'+version+'/pkmn-chest.nds'
					var ciaURL = 'https://github.com/Universal-Team/pkmn-chest/releases/download/'+version+'/pkmn-chest.cia'
					$('#ndsDownload').attr('href', ndsURL);
					$('#ciaDownload').attr('href', ciaURL);
					$('#ndsDownload').attr('display', 'inline-block');
					$('#ciaDownload').attr('display', 'inline-block');
				}
			});
	});
</script>

# Pokémon Chest
> A Pokémon Bank for 4th and 5th generation Pokémon games for the Nintendo DS(i).

Pokémon Chest is an app for the DS(i) that can store and edit Pokémon in the DS Pokémon games.
It's current features include:
- Loading save files from DSi SD, Flashcard SD, and retail cartridges
- Storing up to 500 boxes of Pokémon per chest with support for multiple chests
- Editing most of a Pokémon's data
- Injecting pk4/pk5 files from SD
- Dumping Pokémon to pk4/pk5 files
- Translated to English, French, German, Italian, Japanese, Russian, and Spanish

## Download
[Download .nds](){: .btn .hidden #ndsDownload}
[Download .cia](){: .btn .hidden #ciaDownload}
[Release Page](https://github.com/Universal-Team/pkmn-chest/releases/latest){: .btn}

[Dowload nightly .nds](https://github.com/Universal-Team/extras/raw/master/builds/pkmn-chest/pkmn-chest.nds){: .btn}
[Dowload nightly .cia](https://github.com/Universal-Team/extras/raw/master/builds/pkmn-chest/pkmn-chest.cia){: .btn}

## Screenshots
![Top Menu](assets/images/pkmn-chest/topMenu.png) ![Box](assets/images/pkmn-chest/box.png)

![X Menu](assets/images/pkmn-chest/xMenu.png) ![Options](assets/images/pkmn-chest/options.gif)

![Summary](assets/images/pkmn-chest/summary.png) ![Party](assets/images/pkmn-chest/party.png)

![Natures](assets/images/pkmn-chest/natures.png) ![stats](assets/images/pkmn-chest/stats.png)

## Contact
The best way to talk to us is to join our Discord:

[![Discord](https://discordapp.com/api/guilds/568119817320792074/widget.png?style=banner2)](https://discord.gg/KDJCfGF)

If you want to report a bug you can do so [here](https://github.com/Universal-Team/pkmn-chest/issues/new/choose).

## Credits
### Main Developers
- [Epicpkmn11](https://github.com/Epicpkmn11): GUI code, porting PKSM's save and bank management code
### Translators
- [antoine62](https://github.com/antoine62): French
- [edo9300](https://github.com/edo9300): Italian
- [Epicpkmn11](https://github.com/Epicpkmn11): English and Japanese
- [Extocine](https://twitter.com/@ExtocineN): Russian
- [VoltZ](https://github.com/SuperSaiyajinVoltZ): German
### Others
- [devkitPro](https://github.com/devkitPro), [WinterMute](https://github.com/WinterMute): devkitARM, libnds, and libfat.
- [edo9300](https://github.com/edo9300): [ndsi-savedumper](https://github.com/edo9300/ndsi-savedumper)'s gamecard save dumping and injecting code
- [Flagbrew](https://github.com/FlagBrew): [PKSM](https://github.com/FlagBrew/PKSM)'s save and bank management code
- [RocketRobz](https://github.com/RocketRobz): Adding flashcard and SD being used together and code from [TWiLight Menu++](https://github.com/DS-Homebrew/TWiLightMenu)
- [TotallyNotGuy](https://github.com/TotallyNotGuy): Finding & making graphics and the Pokémon Center generation 4 & 5 songs
- [VoltZ](https://github.com/SuperSaiyajinVoltZ): Idea to make a Pokémon Bank for the DS(i)
### Music
- [Pokémon Center (Gen 1)](https://modarchive.org/index.php?request=view_by_moduleid&query=181718), [Elm's Lab](https://modarchive.org/index.php?request=view_by_moduleid&query=181711), [Oak's Lab](https://modarchive.org/index.php?request=view_by_moduleid&query=181717), and [Game Corner](https://modarchive.org/index.php?request=view_by_moduleid&query=181756).
