# international-list

International List consists **mostly of static cosmetic filters**. English and few German websites are included. As regards tracking filters, they have been partly copied from other privacy filter lists.

**What is the difference between this list and other ad blocking filter lists?**

International List is a **complementary list** to basic ad blocking filter lists (for more info see chapter 2 below). It blocks various subscription and social pop-ups, as well as doubled social buttons. **For example:** EasyList filter list sometimes blocks adverts only. International List often removes the frame where advert was placed initially. The complete ad frame removal often leaves more space for useful content. This list is therefore not meant only for aesthetics but also for practical reasons to keep the page neat and rather clear.

**What is the difference between this list and other advanced privacy filter lists?**

International List is a **very light (mostly cosmetic)** version of Fanboy Annoyances List. This means it doesn't block all the social content. **For example:** if there are social buttons on top and bottom of a webpage, this filter list will remove only social buttons on the top. The others on the bottom remain in order to keep the website functional in terms of social networks.

*So a basic rule here is: first content, then other unobtrusive social crap.*

The list is **intended for simple users** with a set-and-forget approach. Copy the raw URL to your content-filtering software's custom filter list (see chapter 2.B below for more info). If you have any suggestions or issues to report, please do it [here](https://github.com/betterwebleon/international-list/issues) or write an [e-mail](mailto:betterweb.leon@outlook.com).

###1. Recommended content-filtering software
**uBlock Origin**

*Why?* Because it's efficient, lightweight, simple and free. For Firefox, you can [get it here](https://addons.mozilla.org/en/firefox/addon/ublock-origin/).

###2. Recommended complementary filter lists
**A) following lists can be turned on by *ticking* them in uBlock Origin ["3rd-party filters" tab]**
- uBlock filters
- uBlock filters – Badware risks
- uBlock filters – Block-then-redirect
- uBlock filters – Privacy
- uBlock filters – Unbreak
- Adblock Warning Removal List
- EasyList
- EasyPrivacy
- Fanboy's Enhanced Tracking List
- Malware domains
- Spam404

(*Many of them may already be turned on.*)

**B) various custom filter lists can be added by copying the following six URLs to the "Custom" field in uBlock Origin<br>["3rd-party filters" tab]**

1. https://easylist-downloads.adblockplus.org/adwarefilters.txt
2. https://raw.githubusercontent.com/metaphoricgiraffe/behind-the-scenes-filters/master/filters.txt
3. https://raw.github.com/r4vi/block-the-eu-cookie-shit-list/master/filterlist.txt
4. https://raw.githubusercontent.com/betterwebleon/international-list/master/filters.txt
5. https://raw.github.com/liamja/Prebake/master/obtrusive.txt
6. https://raw.githubusercontent.com/metaphoricgiraffe/tracking-filters/master/trackingfilters.txt

(*International List is under the number 4, however it is recommended to add all of them.*)

###3. Recommended browser
**Mozilla Firefox**

*Why?* Because it can be customized in order to improve browsing speed, privacy, user interface, etc.

\**How?* Type this in your address (URL) bar:

<code>about:config</code><br>


Hit enter and confirm a Firefox warning message. Then find the following preference names by copy-pasting each one to the "Search" bar. Double-click on each preference name and change its value to:

|   | PREFERENCE NAME                      | VALUE |
|---|:-------------------------------------|:-----:|
|1. | beacon.enabled                       | false |
|2. | browser.safebrowsing.malware.enabled | false |
|3. | geo.enabled                          | false |
|4. | layout.css.visited_links_enabled     | false |
|5. | network.http.sendSecureXSiteReferrer | false |
|6. | media.peerconnection.enabled         | false |
|7. | media.peerconnection.turn.disable    |  true |
|8. | privacy.trackingprotection.enabled   |  true |

**The upper settings are privacy-related only. If you want more speed and beter UI as well, keep on tweaking:**

|   | PREFERENCE NAME                           | VALUE |
|---|:------------------------------------------|:-----:|
|9. | browser.fullscreen.animate                | false |
|10.| browser.fullscreen.autohide               | false |
|11.| full-screen-api.transition-duration.enter |       |
|12.| full-screen-api.transition-duration.leave |       |
|13.| full-screen-api.warning.timeout           |   0   |
|14.| memory.free_dirty_pages                   |  true |
|15.| network.http.keep-alive.timeout           |   60  |
|16.| network.http.pipelining                   |  true |
|17.| network.http.pipelining.aggressive        |  true |
|18.| network.http.pipelining.maxrequests       |   8   |
|19.| network.http.pipelining.ssl               |  true |
|20.| network.http.proxy.pipelining             |  true |
|21.| network.http.request.max-start-delay      |   3   |
|22.| network.websocket.delay-failed-reconnects | false |

**At paragraphs *11.* and *12.* there are indeed no values. Just delete the existing values and confirm.** :)

**After you enable the Firefox Tracking Protection (at paragraph *8.*), Facebook/Twitter videos or Facebook widgets/comments will not appear on some websites.** If you want to see them, just click on the "shield" icon while on website (the icon is in address bar - left to the URL in the browser) and then click the button to disable Tracking Protection for that website. The browser will save your settings for corresponding parent domain name, so you won't have to do anything next time you visit any website from that domain name.

\* ***Take advantage of this valuable information at your own risk - if there is any. It is possible to revert the changes anytime. Be fearless, padawan!***

###4. Hosts file
Another very important and useful tweak is the file named "hosts". It is highly recommended to set it up **together** with all aforementioned tweaks. According to [StevenBlack](https://github.com/StevenBlack/hosts/blob/master/readme.md), <code>hosts</code> is a plain-text file used by all operating systems to map hostnames to IP addresses. The <code>hosts</code> is not bound to any browser, so it should work all the time irrespective of the browser or program.

In other words, <code>hosts</code> works on a system level and takes care of all the junk before it even "reaches" a browser. It blocks the whole website and therefore protects user from getting into contact with dangerous websites, full of malware. Further, it greatly improves browsing speed and privacy by blocking access to various known ad servers and data collecting systems. StevenBlack's version of <code>hosts</code> file has been amalgamated with various sources. You can download the file from [here](https://github.com/StevenBlack/hosts/archive/master.zip) (you will find it within the downloaded zip file). Then:

- in Windows, you  place it to the folder <code>C:\Windows\System32\Drivers\etc</code>
- in Mac OS X, iOS, Linux or Android you place it to the folder <code>/etc/hosts</code>

After you are done, the easiest way is to restart the computer. Or you can also do it faster:

- in **Windows**, open the Command Prompt window (cmd.exe) as an Administrator: Then run <code>ipconfig /flushdns</code>
- in **Mac OS X**, open the Terminal and run: <code>sudo dscacheutil -flushcache;sudo killall -HUP mDNSResponder</code>
- in **Linux Debian/Ubuntu**, open the Terminal and run with root privileges: <code>sudo /etc/rc.d/init.d/nscd restart</code>
- in **Linux with systemd**, open the Terminal and run with root privileges: <code>sudo systemctl restart network.service</code>
- in **Fedora Linux** or **Arch Linux/Manjaro**, open the Terminal and run with root privileges:<br><code>sudo systemctl restart NetworkManager.service</code>

Close the window and restart your browser, if it has been opened. That's all. Enjoy browsing :)

###5. License
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
