# international-list

International List consists **mostly of static cosmetic filters**. English and few German websites are included. As regards tracking filters, they have been partly copied from other privacy filter lists.

The list is **intended for simple users** with a set-and-forget approach. Copy the raw URL to your content-filtering software's custom filter list (see chapter 2.B below for more info). If you have any suggestions or issues to report, please do it [here](https://github.com/betterwebleon/international-list/issues) or write an [e-mail](mailto:betterweb.leon@outlook.com).

***What is the difference between this list and other ad blocking filter lists?***

International List is a **complementary list** to basic ad blocking filter lists (for more info see chapter 2 below). It blocks various subscription and social pop-ups as well as doubled social buttons. *For example:* EasyList filter list sometimes blocks adverts only. International List often removes the frame where advert was placed initially. The complete ad frame removal often leaves more space for useful content. This list is therefore not meant only for aesthetics but also for practical reasons to keep the page neat and rather clear.

***What is the difference between this list and other advanced privacy filter lists?***

International List is sort of a **very light (mostly cosmetic)** version of Fanboy Annoyances List. This means it does not block most of the social content. *For example:* if there are social buttons on top and bottom of a webpage, this filter list will remove only social buttons on the top. The others on the bottom remain in order to keep the website functional in terms of social networks.

*So a basic rule here is: first content, then other unobtrusive social crap.*

-------------
###1. Recommended browser
**[Mozilla Firefox](https://www.mozilla.org/firefox/new/)**

*Why?* Because it can be customized in order to improve browsing speed, privacy, user interface, etc.

*How?* Type this in your address (URL) bar:<br>
<code>about:config</code>

Hit enter and confirm a Firefox warning message. You will see the settings panel.<br>
Then find the following preference names by copy-pasting each one to the "*Search*" bar.

**--- In order to increase PRIVACY ---**<br>
Double-click on each preference name and change its value to:

|   | Preference name                                               | Value |
|---|:--------------------------------------------------------------|:-----:|
|1. | beacon.enabled                                                | false |
|2. | browser.safebrowsing.downloads.enabled                        | false |
|3. | browser.safebrowsing.enabled                                  | false |
|4. | browser.safebrowsing.malware.enabled                          | false |
|5. | services.sync.prefs.sync.browser.safebrowsing.enabled         | false |
|6. | services.sync.prefs.sync.browser.safebrowsing.malware.enabled | false |
|7. | geo.enabled                                                   | false |
|8. | layout.css.visited_links_enabled                              | false |
|9. | network.http.sendSecureXSiteReferrer                          | false |
|10.| media.peerconnection.enabled                                  | false |
|11.| media.peerconnection.turn.disable                             |  true |
|12.| privacy.trackingprotection.enabled                            |  true |

**--- In order to increase SPEED ---**<br>
Double-click on each preference name and change its value to:

|   | Preference name                           | Value |
|---|:------------------------------------------|:-----:|
|13.| browser.cache.use_new_backend             |   1   |
|14.| full-screen-api.transition-duration.enter |  0 0  |
|15.| full-screen-api.transition-duration.leave |  0 0  |
|16.| full-screen-api.warning.timeout           |   0   |
|17.| image.mem.max_decoded_image_kb            | 51200 |
|18.| javascript.options.mem.high_water_mark    |   30  |
|19.| javascript.options.mem.max                | 51200 |
|20.| memory.free_dirty_pages                   |  true |
|21.| network.http.keep-alive.timeout           |   60  |
|22.| network.http.pipelining                   |  true |
|23.| network.http.pipelining.aggressive        |  true |
|24.| network.http.pipelining.maxrequests       |   8   |
|25.| network.http.pipelining.ssl               |  true |
|26.| network.http.proxy.pipelining             |  true |
|27.| network.http.request.max-start-delay      |   3   |
|28.| network.websocket.delay-failed-reconnects | false |
|29.| security.dialog_enable_delay              |   0   |

**--- Additional tweaks for BATTERY SAVING and/or LOW-PERFORMANCE COMPUTERS ---**<br>
Double-click on each preference name and change its value to:

|   | Preference name                      | Value |
|---|:-------------------------------------|:-----:|
|30.|browser.download.animateNotifications | false |
|31.|browser.fullscreen.animate            | false |
|32.|browser.panorama.animate_zoom         | false |
|33.|browser.sessionhistory.max_entries    |  15   |
|34.|browser.sessionstore.max_tabs_undo    |   8   |
|35.|browser.tabs.animate                  | false |


- At paragraphs ***14.*** and ***15.*** there are indeed two values (zeroes).
- After you enable the *Firefox Tracking Protection* (at paragraph ***12.***), Facebook/Twitter videos or Facebook widgets and comments **will not load** on some websites.<br>**If you want to see them**, just click on the "shield" icon while on website (the icon is shown in browser's address bar - left to the URL) and then click the button "*Disable protection for this session*" in pop-up panel. The browser will save your setting for corresponding domain name, so you will not have to block it again next time you visit any website from that domain name. Whenever Firefox tracking protection is disabled, the "shield" icon is red-crossed (while such websites are opened).

#####ALSO IMPORTANT:
######a) To save battery and increase safety [ask to activate Flash]
Type this in your address bar:<br>
<code>about:addons</code><br>
Hit enter and click on **Plugins** on the left panel. Then find **Shockwave Flash** on the right side.<br>
Set it to: ***Ask to Activate***.

When necessary (to enable videos, etc.) you will still be able to choose *Allow and Remember*<br>
([**see this picture on how to enable Flash by default on specific websites**](http://cdn3.jasonsamuel.com/wp-content/uploads/2014/07/3.jpg)).

######b) To optimize scrolling [animation speed]
If you are facing choppy and lagging scrolling in Firefox, increase the animation speed.<br>
Set the following value (in *about:config*):<br>
<code>layout.frame_rate.precise</code> ---> **true**

**Note:** If your scrolling performance is already okay, it may get worse after changing the upper value. In that case, reset the value to default.

######c) To optimize graphics performance [hardware acceleration]
If your graphics card (GPU) is not too slow, enable hardware acceleration. Type this in your address bar:<br>
<code>about:preferences#advanced</code><br>
Hit enter. In *General* tab enable this option: ***Use hardware acceleration when available***<br>
([**see this picture**](http://www.clonefileschecker.com/blog/wp-content/uploads/2015/10/Disabling-Hardware-Acceleration-in-Mozilla-Firefox.png)).

**Notes:**

1. To test the effect of enabled/disabled hardware acceleration, you need to **restart the browser**.<br>
2. **Test both options** (with enabled as well as disabled value) on slower computers to see the difference!<br>If Firefox lags more while hardware acceleration is enabled, disable the setting.<br>

######d) Miscellaneous
- If you want to *disable* built-in feature ***Firefox Hello***, set the following value (in *about:config*):<br>
<code>loop.enabled</code> ---> **false**
- If you want to *disable* built-in feature ***Pocket*** (not an addon), set the following value (in *about:config*):<br><code>browser.pocket.enabled</code> ---> **false**
- If you have **very slow disk**, reduce the size of disk cache. Set the following value (in *about:config*):<br><code>browser.cache.offline.capacity</code> ---> **250000**<br>The latter setting applies only to some very old computers (10+ years), since modern drives are usually fast enough.

*After you finish tweaking, simply close the tab with Firefox settings.*

###2. Recommended content-filtering software
**uBlock Origin**

*Why?* Because it is efficient, lightweight, simple and free. For Firefox, you can **[get it here](https://addons.mozilla.org/en/firefox/addon/ublock-origin/)** by clicking the green button:<br>*<code>Add to Firefox</code>*. It is better than any other alternative content-blocking solution. It uses much less resources from inefficient addon *AdBlock Plus* as well, as is evident from [this comparison](https://github.com/gorhill/uBlock/wiki/uBlock-vs.-ABP:-efficiency-compared) and also from [this comprehensive test](https://www.raymond.cc/blog/10-ad-blocking-extensions-tested-for-best-performance/view-all/).

####2.a) Recommended complementary filter lists

Following lists can be turned on by *ticking* them in uBlock Origin ["3rd-party filters" tab]:
- uBlock filters
- uBlock filters – Badware risks
- uBlock filters – Privacy
- uBlock filters – Unbreak
- Adblock Warning Removal List
- EasyList
- EasyPrivacy
- Fanboy's Enhanced Tracking List
- Malware domains
- Spam404

**Many of them (including potential regional lists for your country) should already be enabled**. Enable the rest and then click on the upper right button *<code>Apply changes</code>*. After that click the button *<code>Update now</code>* on the top left. Wait for a few moments until the button turns gray.

####2.b) Recommended additional complementary filter lists

There are also many additional (custom) lists. They can be added manually, by copying the following four URLs and pasting them to the "Custom" text area in uBlock Origin. The text area can be found at the bottom of pane ["3rd-party filters" tab].

<code>https://<i></i>easylist-downloads.adblockplus.org/adwarefilters.txt</code><br>
<code>https://<i></i>raw.githubusercontent.com/metaphoricgiraffe/behind-the-scenes-filters/master/filters.txt</code><br>
<code>https://<i></i>raw.githubusercontent.com/betterwebleon/international-list/master/filters.txt</code><br>
<code>https://<i></i>raw.githubusercontent.com/metaphoricgiraffe/tracking-filters/master/trackingfilters.txt</code><br>

It is recommended to add all the URL's to uBlock Origin in order to maximize filtering scope.<br>
After you paste link(s), first click on the *<code>Parse</code>* button below the text area. Then click on *<code>Apply changes</code>* button in the upper right corner. After that click on *<code>Update now</code>* button on the top left.

###3. Various recommended add-ons for Mozilla Firefox

The following add-ons can be installed optionally. However every (simple) user will find add-ons no. **5.**, **6**, **8.**, **9.**, **10.**, **12.**, and **14.** very useful, because they optimize browsing significantly and do not require much time to set them up.

1. [**Classic Theme Restorer**](https://addons.mozilla.org/en/firefox/addon/classicthemerestorer/)
2. [**Click&Clean**](https://addons.mozilla.org/en/firefox/addon/clickclean/)
3. [**Download Panel Tweaks**](https://addons.mozilla.org/en/firefox/addon/download-panel-tweaks/)
4. [**FindBar Tweak**](https://addons.mozilla.org/en/firefox/addon/findbar-tweak/)
5. [**Google search link fix**](https://addons.mozilla.org/en/firefox/addon/google-search-link-fix/)
6. [**I don't care about cookies**](https://addons.mozilla.org/en/firefox/addon/i-dont-care-about-cookies/)
7. [**Pocket**](https://mega.nz/#!T5RjHZyb!yXz5Wj-x7lWdRKbcCaMQ0_lZfpI828spmIm_sOEX5Ng)
8. [**Pure URL**](https://addons.mozilla.org/en/firefox/addon/pure-url/) \*
9. [**uBlock Origin**](https://addons.mozilla.org/en/firefox/addon/ublock-origin/)
10. [**Undo Close Tab Replacement**](https://addons.mozilla.org/en/firefox/addon/undo-close-tab-replacement/)
11. [**UnMHT**](https://addons.mozilla.org/en/firefox/addon/unmht/)
12. [**Webmail Ad Blocker**](https://addons.mozilla.org/en/firefox/addon/webmail-ad-blocker/)
13. [**X-notifier**](https://addons.mozilla.org/en/firefox/addon/xnotifier/)
14. [**YouTube High Definition**](https://addons.mozilla.org/en/firefox/addon/youtube-high-definition/)
15. [**ZenMate Security, Privacy & Unblock VPN**](https://addons.mozilla.org/en/firefox/addon/zenmate-security-privacy-vpn/)

\* If you encounter a problem of some blank websites (very rarely), use less rigorous addon instead of *Pure URL*:<br>
[**au-revoir-utm**](https://addons.mozilla.org/en/firefox/addon/au-revoir-utm/)

###4. Hosts file
Another very important and useful tweak is the file named "*hosts*". It is highly recommended to set it up **together with all aforementioned tweaks**. According to [StevenBlack](https://github.com/StevenBlack/hosts/blob/master/readme.md), *hosts* is a plain-text file used by all operating systems to map hostnames to IP addresses. The *hosts* is not bound to any browser, so it should work all the time irrespective of the browser or program.

In other words, *hosts* works on a system level and takes care of all the junk before it even "reaches" a browser. It blocks the whole website and therefore protects user from getting into contact with dangerous websites, full of malware. Further, it greatly improves browsing speed and privacy by blocking access to various known ad servers and data collecting systems. StevenBlack's version of *hosts* file has been amalgamated with various sources. You can download the file **[here](https://github.com/StevenBlack/hosts/archive/master.zip)** (you will find it within downloaded zip file, in the "*hosts-master*" map). Then:

- in **Windows**, you  place it to the folder <code>C:\Windows\System32\Drivers\etc</code>
- in **Mac OS X, iOS, Linux or Android** you place it to the folder <code>/etc/hosts</code>

After you are done, the easiest way is to restart the computer. Or you can also do it faster:

- in ***Windows***, open the Command Prompt window (cmd.exe) as an Administrator. Then run:<br><code>ipconfig /flushdns</code>
- in ***Mac OS X***, open the Terminal and run:<br><code>sudo dscacheutil -flushcache;sudo killall -HUP mDNSResponder</code>
- in ***Linux Debian/Ubuntu***, open the Terminal and run with root privileges:<br><code>sudo /etc/rc.d/init.d/nscd restart</code>
- in ***Linux with systemd***, open the Terminal and run with root privileges:<br><code>sudo systemctl restart network.service</code>
- in ***Fedora Linux*** or ***Arch Linux/Manjaro***, open the Terminal and run with root privileges:<br><code>sudo systemctl restart NetworkManager.service</code>

Close the window and restart your browser, if it has been opened. That's all.<br>Enjoy your browsing! :)

-------------
###License
This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org>

HAVE A NICE DAY. (*This wish is not part of the license anymore. You can however treat it as a special annex to the license.*)
