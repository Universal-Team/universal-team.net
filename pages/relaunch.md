---
color: "#666"
repo: Universal-Team/Relaunch
redirect_from:
  - relaunch
---

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script>
  $(document).ready(function() {
    $.getJSON('https://api.github.com/repos/Universal-Team/Relaunch/tags').done(function(json) {
      var release = json[0];
      var version = release.name;

      var zipURL = 'https://github.com/Universal-Team/Relaunch/releases/download/'+version+'/Relaunch.7z'
      var releaseURL = 'https://github.com/Universal-Team/Relaunch/releases/tag/'+version

      $('#ndsDownload').attr('href', zipURL);
      $('#zipDownload').attr('class', 'btn');
      $('#latestVersion').html(version)
      $('#latestVersion').attr('href', releaseURL);
    });
  });
</script>

# Relaunch

## Download
[Download .7z](){: .btn .hidden #zipDownload}
[Download Page](https://github.com/Universal-Team/Relaunch/releases/latest){: .btn}

## Basic Setup
1. Get some .nds homebrew. (You can get some [here](https://www.gamebrew.org/wiki/List_of_DS_homebrew_applications))
2. Start Relaunch and hold A and B.
3. Head to Options and choose your hotkey apps.
4. Start Relaunch again and hold the button corresponding to the app you want to launch.


## Advanced Usage
- You can edit the `Relaunch.ini` file and set custom paths, names, and file extensions for your files, you can also do this in the Relaunch menu.
- Hold `A` + `B` on boot in order to open the menu.
- There are prebuilt nightlies of Relaunch avaliable on [Universal-Team/extras](https://github.com/Universal-Team/extras/tree/master/builds)

## Credits
- [Flame](https://github.com/FlameKat53): The main developer of Relaunch
- [Epicpkmn11](https://github.com/Epicpkmn11): Implementing tons of minor and some major additions I couldn't get to work .-.
- [nocash](http://problemkaputt.de): Creating [Unlaunch](http://problemkaputt.de/unlaunch.htm), which this app is inspired by.
- [RocketRobz](https://github.com/RocketRobz): Creating [GodMode9i](https://github.com/RocketRobz/GodMode9i), the base of the Relaunch Menu.