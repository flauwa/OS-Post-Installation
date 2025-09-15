# Fedora Workstation Post Installation [Fedora 40 - Gnome 46 (Kathmandu)]

## 1. Edit the dnf config file (sudo vi /etc/dnf/dnf.conf):
Adding these to it:

    fastestmirror=True
    max_parallel_downloads=10

## 2. Perform an initial system update:
    sudo dnf update

## 3. Drivers update:
    sudo fwupdmgr get-devices
    sudo fwupdmgr refresh --force
    sudo fwupdmgr get-updates
    sudo fwupdmgr update

## 4. Settings:
Configure settings as myself needs, especially:
- Display.
- Power.
- Appearance.
- Keyboard.
- Privacy & Security.
- System.

## 5. Configure additional repositories (Including 3rd Party):
- https://rpmfusion.org/Configuration
- 3rd Party Repositories enabled while OS Installation.

## 6. Install Multimedia plugins and related things:
- https://docs.fedoraproject.org/en-US/quick-docs/installing-plugins-for-playing-movies-and-music/
- https://docs.fedoraproject.org/en-US/quick-docs/openh264/

Optional:
- Install VLC.

## 7. Install Gnome Tweaks and Gnome Extensions:
All extensions saved at my Firefox Bookmark Toolbar but I put my list here for anyone who sees this:

- https://extensions.gnome.org/extension/3088/extension-list/
- https://extensions.gnome.org/extension/1460/vitals/ (Vitals is superior to System Monitor, I pick the second one).
- https://extensions.gnome.org/extension/6807/system-monitor/
- https://extensions.gnome.org//extension/615/appindicator-support/
- https://extensions.gnome.org/extension/5446/quick-settings-tweaker/
- https://extensions.gnome.org/extension/1401/bluetooth-quick-connect/
- https://extensions.gnome.org/extension/18/native-window-placement/
- https://extensions.gnome.org/extension/779/clipboard-indicator/
- https://extensions.gnome.org/extension/4470/media-controls/
- https://extensions.gnome.org/extension/6242/emoji-copy/
- https://extensions.gnome.org/extension/5090/space-bar/
- https://extensions.gnome.org/extension/675/lunar-calendar/

Optional extensions:
- https://extensions.gnome.org/extension/307/dash-to-dock/
- https://extensions.gnome.org/extension/3193/blur-my-hell/
- https://extensions.gnome.org/extension/5500/auto-activities/
- https://extensions.gnome.org/extension/7048/rounded-window-corners-reborn/
- https://extensions.gnome.org/extension/4/panel-favorites/
- https://extensions.gnome.org/extension/2/move-clock/

## 8. My own things:
- Safe Eyes: a Free and Open Source tool for Linux users to reduce and prevent repetitive strain injury (RSI).
    - https://github.com/slgobinath/SafeEyes
    - Adding breaks:
        - Short: Fly to the moon.
        - Short: Go touch some grass.
        ---
        - Long: Go get to sleep.
        - Long: Here we go again.
        - Long: Breaking the habit.
- ibus-bamboo: a Vietnamese input method for Linux.
    - https://github.com/BambooEngine/ibus-bamboo
    - https://software.opensuse.org//download.html?project=home%3Alamlng&package=ibus-bamboo
- Spotify: an audio streaming and media service provider.
    - https://docs.fedoraproject.org/en-US/quick-docs/installing-spotify/
    - Or installing using Flathub via Software Application / Gnome Software Center.
- VSCode: a code editor redefined and optimized for building and debugging modern web and cloud applications.
    - https://code.visualstudio.com/docs/setup/linux

Optional:
- Vivaldi Browser: a fun web browser.
    - https://vivaldi.com/download/
- Zed editor: an open source, high-performance, multiplayer code editor from the creators of Atom and Tree-sitter.
    - https://zed.dev/download
- Cloudflare WARP (1.1.1.1): a free Domain Name System service.
    - https://pkg.cloudflareclient.com/
    - https://developers.cloudflare.com/warp-client/get-started/linux/
    - https://developers.cloudflare.com/cloudflare-one/faq/teams-troubleshooting/

## 9. Browser Extensions Backup:
    - Enhancer for Youtube:
    {"version":"2.0.125.1","settings":{"blur":0,"brightness":100,"contrast":100,"grayscale":0,"huerotate":0,"invert":0,"saturate":100,"sepia":0,"applyvideofilters":false,"backgroundcolor":"#000000","backgroundopacity":85,"blackbars":false,"blockautoplay":true,"blockhfrformats":false,"blockwebmformats":false,"boostvolume":false,"cinemamode":false,"cinemamodewideplayer":true,"controlbar":{"active":true,"autohide":true,"centered":true,"position":"fixed"},"controls":["reverse-playlist","volume-booster","cards-end-screens","cinema-mode","pop-up-player","speed","options"],"controlsvisible":false,"controlspeed":true,"controlspeedmousebutton":false,"controlvolume":false,"controlvolumemousebutton":false,"convertshorts":false,"customcolors":{"--dimmer-text":"#cccccc","--hover-background":"#232323","--main-background":"#111111","--main-color":"#00adee","--main-text":"#eff0f1","--second-background":"#181818","--shadow":"#000000"},"customcssrules":"","customscript":"","customtheme":false,"darktheme":false,"date":1685191436467,"defaultvolume":false,"disableautoplay":true,"executescript":false,"expanddescription":false,"filter":"none","hidecardsendscreens":true,"hidechat":false,"hidecomments":false,"hiderelated":false,"hideshorts":false,"ignoreplaylists":true,"ignorepopupplayer":true,"localecode":"en_US","localedir":"ltr","message":false,"miniplayer":true,"miniplayerposition":"_top-right","miniplayersize":"_880x495","newestcomments":false,"overridespeeds":true,"pauseforegroundtab":false,"pausevideos":false,"popuplayersize":"1280x720","qualityembeds":"hd720","qualityembedsfullscreen":"hd1080","qualityplaylists":"hd720","qualityplaylistsfullscreen":"hd1080","qualityvideos":"hd720","qualityvideosfullscreen":"hd1080","reload":false,"reversemousewheeldirection":false,"selectquality":true,"selectqualityfullscreenoff":false,"selectqualityfullscreenon":false,"speed":1,"speedvariation":0.1,"stopvideos":false,"theatermode":false,"theme":"default-dark","themevariant":"youtube-deep-dark.css","update":1711092783218,"volume":50,"volumemultiplier":3,"volumevariation":5,"wideplayer":false,"wideplayerviewport":false}}

    - UBlock Origin:
    {"timeStamp":1715976426615,"version":"1.57.2","userSettings":{"colorBlindFriendly":true,"uiAccentCustom":true,"uiAccentCustom0":"#f75782","externalLists":"https://malware-filter.gitlab.io/pup-filter/pup-filter.txt\nhttps://raw.githubusercontent.com/StevenBlack/hosts/master/hosts\nhttps://raw.githubusercontent.com/jerryn70/GoodbyeAds/master/Hosts/GoodbyeAds.txt\nhttps://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt\nhttps://www.i-dont-care-about-cookies.eu/abp/","importedLists":["https://malware-filter.gitlab.io/pup-filter/pup-filter.txt","https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts","https://raw.githubusercontent.com/jerryn70/GoodbyeAds/master/Hosts/GoodbyeAds.txt","https://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt","https://www.i-dont-care-about-cookies.eu/abp/"],"popupPanelSections":15},"selectedFilterLists":["user-filters","ublock-filters","ublock-badware","ublock-privacy","ublock-quick-fixes","ublock-unbreak","adguard-generic","adguard-mobile","easylist","adguard-spyware-url","block-lan","easyprivacy","urlhaus-1","curben-phishing","plowe-0","adguard-mobile-app-banners","adguard-other-annoyances","adguard-popup-overlays","adguard-social","adguard-widgets","easylist-chat","easylist-annoyances","fanboy-social","fanboy-thirdparty_social","ublock-annoyances","https://raw.githubusercontent.com/jerryn70/GoodbyeAds/master/Hosts/GoodbyeAds.txt","https://www.i-dont-care-about-cookies.eu/abp/","https://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt","https://malware-filter.gitlab.io/pup-filter/pup-filter.txt","https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts"],"hiddenSettings":{},"whitelist":["# edge-scheme","about-scheme","chrome-extension-scheme","chrome-scheme","moz-extension-scheme","newtab.edge-scheme","opera-scheme","vivaldi-scheme","www.facebook.com","www.microsoft.com","wyciwyg-scheme"],"dynamicFilteringString":"behind-the-scene * * noop\nbehind-the-scene * inline-script noop\nbehind-the-scene * 1p-script noop\nbehind-the-scene * 3p-script noop\nbehind-the-scene * 3p-frame noop\nbehind-the-scene * image noop\nbehind-the-scene * 3p noop\n* vo.aicdn.com * noop\n* ajax.googleapis.com * noop\n* js.appboycdn.com * noop\n* ajax.aspnetcdn.com * noop\n* materialdesignicons.b-cdn.net * noop\n* libs.baidu.com * noop\n* lib.baomitu.com * noop\n* apps.bdimg.com * noop\n* cdn.bootcdn.net * noop\n* cdn.bootcss.com * noop\n* maxcdn.bootstrapcdn.com * noop\n* netdna.bootstrapcdn.com * noop\n* stackpath.bootstrapcdn.com * noop\n* ajax.cloudflare.com * noop\n* cdnjs.cloudflare.com * noop\n* use.fontawesome.com.cdn.cloudflare.net * noop\n* cdn.embed.ly.cdn.cloudflare.net * noop\n* cdn.jsdelivr.net.cdn.cloudflare.net * noop\n* ajax.loli.net.cdn.cloudflare.net * noop\n* cdnjs.loli.net.cdn.cloudflare.net * noop\n* fonts.loli.net.cdn.cloudflare.net * noop\n* code.createjs.com * noop\n* cdn.datatables.net * noop\n* cdn.embed.ly * noop\n* use.fontawesome.com * noop\n* sdn.inbond.gslb.geekzu.org * noop\n* sdn.geekzu.org * noop\n* gitcdn.github.io * noop\n* gstaticadssl.l.google.com * noop\n* mat1.gtimg.com * noop\n* cds.s5x3j6q5.hwcdn.net * noop\n* apps.bdimg.jomodns.com * noop\n* code.jquery.com * noop\n* cdn.jsdelivr.net * noop\n* akamai-webcdn.kgstatic.net * noop\n* lib.sinaapp.com * noop\n* ajax.loli.net * noop\n* cdnjs.loli.net * noop\n* fonts.loli.net * noop\n* cdn.bootcss.com.maoyundns.com * noop\n* cdn.bootcdn.net.maoyundns.com * noop\n* cdn.materialdesignicons.com * noop\n* cdn.mathjax.org * noop\n* ajax.microsoft.com * noop\n* mscomajax.vo.msecnd.net * noop\n* akamai-webcdn.kgstatic.net.edgesuite.net * noop\n* dualstack.osff.map.fastly.net * noop\n* pagecdn.io * noop\n* cdn.plyr.io * noop\n* lib.baomitu.com.qh-cdn.com * noop\n* iduwdjf.qiniudns.com * noop\n* mat1.gtimg.com.tegsea.tc.qq.com * noop\n* cdn.ravenjs.com * noop\n* mathjax.rstudio.com * noop\n* developer.n.shifen.com * noop\n* lb.sae.sina.com.cn * noop\n* cdn.staticfile.org * noop\n* unpkg.com * noop\n* upcdn.b0.upaiyun.com * noop\n* gateway.cname.ustclug.org * noop\n* ajax.proxy.ustclug.org * noop\n* yandex.st * noop\n* yastatic.net * noop\n* vjs.zencdn.net * noop","urlFilteringString":"","hostnameSwitchesString":"no-large-media: behind-the-scene false\nno-csp-reports: * true","userFilters":""}
