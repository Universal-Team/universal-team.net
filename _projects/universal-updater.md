---
title: Universal-Updater
description: An easy to use app for installing and updating 3DS homebrew
image: /images/icons/universal-updater.png
repo: Universal-Team/Universal-Updater
downloads:
   release:
      qr: https://db.universal-team.net/assets/images/qr/universal-updater.cia.png
      files: [Universal-Updater.3dsx, Universal-Updater.cia]
   nightly:
      qr: https://db.universal-team.net/assets/images/qr/nightly/universal-updater.cia.png
      files: [Universal-Updater.3dsx, Universal-Updater.cia]
screenshots:
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/entry-info.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/download-list.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/queue-menu.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/search-menu.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/sort-menu.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/settings-menu.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/mark-menu.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/screenshot.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/release-notes.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/list-style.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/language-selection.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/store-selection.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/recommended-unistores.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/auto-update-settings.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/gui-settings.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/directory-settings.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/directory-selection.png
   - https://db.universal-team.net/assets/images/screenshots/universal-updater/credits.png
---

Universal-Updater is a homebrew application for the Nintendo 3DS with the intention to make downloading other homebrew simple and easy. No need to manually copy files or go through installation processes, as we do that for you.

Its features include:
- A store format with a concept similar to the Cydia Repositories
   - The default is <a href="https://db.universal-team.net">Universal-DB</a>
   - Want to add your own? Go to settings, find "Select Unistore", hit the + icon and type the URL or hit the QR button and scan the QR code (if they have one)
   - Some recommended UniStores are <a href="#unistores">below</a>
- Customization in sorting and display
   - All sorting keys: "Title", "Author", and "Last Updated"
   - Direction could be Ascending or Descending
   - App display could be shown in either a Grid or Rows
- Background installation so you can keep using the rest of the app while installing
- Searching and markings to make finding apps easy
- Viewing screenshots and release notes for apps
- Shortcuts for easily updating frequently updated apps when using the Homebrew Launcher
- Translations for users of many languages
   - To contribute to translations, join our <a href="https://crwd.in/universal-updater">Crowdin</a>
   - To request a new language, join our <a href="../discord.html">Discord Server</a> or contact a project manager on Crowdin

----

{% include downloads.html %}

----

{% include screenshots.html %}

----

## ![UniStore logo](/images/icons/unistore.png) UniStores
<div class="row">
	<div class="col-sm-4">
		<h2>How to add UniStores:</h2>
	</div>
	<div class="col-sm-8">
		<ol>
			<li>Tap the settings icon in the sidebar</li>
			<li>Select <code>Select UniStore</code></li>
			<li>Tap the + icon along the bottom</li>
			<li>Choose one from the list, enter a URL, or scan a UniStore's QR code</li>
		</ol>
	</div>
</div>

----

## Credits
- [SuperSaiyajinStackZ](https://github.com/SuperSaiyajinStackZ) - Lead developer, reworked quirc to C++
- [Pk11](https://github.com/Epicpkmn11) - Mockup Designer, Website Maintainer
- [NightScript](https://github.com/NightYoshi370) - Concept Creator & Planner
- [dlbeer](https://github.com/dlbeer) - Original developer of [quirc](https://github.com/dlbeer/quirc)
- [FlagBrew](https://github.com/FlagBrew): Original QR Code Scanner code
- [Icons8](https://icons8.com/): Icon Designer
- [lvandeve](https://github.com/lvandeve): For [LodePNG](https://github.com/lvandeve/lodepng)
- [PabloMK7](https://github.com/mariohackandglitch): Download Code Improvements
