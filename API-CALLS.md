
# DABMAN i450 Remote Control

## INIT
http://192.168.11.8/init?language=de

```xml
<?xml version="1.0" encoding="UTF-8"?>
<result>
  <id>1</id>
  <version>h91420170914h</version>
  <lang>de</lang>
  <wifi_set_url>http://192.168.78.1/scan_wifi</wifi_set_url>
  <ptver>20170822</ptver>
  <hotkey_fav>1</hotkey_fav>
  <push_talk>1</push_talk>
  <leave_msg>1</leave_msg>
  <leave_msg_ios>1</leave_msg_ios>
  <M7_SUPPORT>0</M7_SUPPORT>
  <SMS_SUPPORT>1</SMS_SUPPORT>
  <MKEY_SUPPORT>1</MKEY_SUPPORT>
  <UART_CD>0</UART_CD>
  <PlayMode>1</PlayMode>
  <SWUpdate>NO</SWUpdate>
</result>
```

## hotkeylist
http://192.168.11.8/hotkeylist
```xml
<?xml version="1.0" encoding="UTF-8"?>
<menu>
  <item_total>5</item_total>
  <item_return>5</item_return>
  <item>
    <id>75_256</id>
    <status>emptyfile</status>
    <name>Leer</name>
  </item>
  <item>...</item>
</menu>
```
# List
http://192.168.11.8/list?id=1&start=1&count=15
```xml
<?xml version="1.0" encoding="UTF-8"?>
<menu>
  <item_total>9</item_total>
  <item_return>9</item_return>
  <item>
    <id>87</id>
    <status>content</status>
    <name>Lokale Station</name>
</item>
<item>
  <id>52</id>
  <status>content</status>
  <name>Internet Radio</name>
</item>
<item>
  <id>2</id><status>content</status><name>Media-Center</name></item><item><id>5</id><status>content</status><name>FM</name></item><item><id>91</id><status>content</status><name>DAB/DAB+</name></item><item><id>3</id><status>content</status><name>Informations-Center</name></item><item><id>47</id><status>content</status><name>AUX</name></item><item><id>104</id><status>content</status><name>Bluetooth</name></item><item><id>6</id><status>content</status><name>Einstellungen</name></item></menu>
```
http://192.168.11.8/list?id=91&start=1&count=500
```xml
<?xml version="1.0" encoding="UTF-8"?><menu><item_total>37</item_total><item_return>37</item_return><item><id>91_1</id><status>file</status><name>80s80s           </name></item><item><id>91_2</id><status>file</status><name>917XFM           </name></item><item><id>91_3</id><status>file</status><name>ANTENNE-SYLT     </name></item><item><id>91_4</id><status>file</status><name>Absolut relax    </name></item><item><id>91_5</id><status>file</status><name>DRadio DokDeb    </name></item><item><id>91_6</id><status>file</status><name>Dlf              </name></item><item><id>91_7</id><status>file</status><name>Dlf Kultur       </name></item><item><id>91_8</id><status>file</status><name>Dlf Nova         </name></item><item><id>91_9</id><status>file</status><name>ENERGY DIGITAL   </name></item><item><id>91_10</id><status>file</status><name>ERF Plus         </name></item><item><id>91_11</id><status>file</status><name>ERF Pop          </name></item><item><id>91_12</id><status>file</status><name>HAMBURG ZWEI     </name></item><item><id>91_13</id><status>file</status><name>HLRdigital       </name></item><item><id>91_14</id><status>file</status><name>KLASSIK RADIO    </name></item><item><id>91_15</id><status>file</status><name>MegaRadio        </name></item><item><id>91_16</id><status>file</status><name>N-JOY            </name></item><item><id>91_17</id><status>file</status><name>NDR 2            </name></item><item><id>91_18</id><status>file</status><name>NDR 90,3         </name></item><item><id>91_19</id><status>file</status><name>NDR Blue         </name></item><item><id>91_20</id><status>file</status><name>NDR Info         </name></item><item><id>91_21</id><status>file</status><name>NDR Info Spezial </name></item><item><id>91_22</id><status>file</status><name>NDR Kultur       </name></item><item><id>91_23</id><status>file</status><name>NDR Plus         </name></item><item><id>91_24</id><status>file</status><name>PELI ONE         </name></item><item><id>91_25</id><status>file</status><name>R.SH - Hamburg   </name></item><item><id>91_26</id><status>file</status><name>RADIO BOB!       </name></item><item><id>91_27</id><status>file</status><name>ROCK ANTENNE HH  </name></item><item><id>91_28</id><status>file</status><name>Radio Hamburg    </name></item><item><id>91_29</id><status>file</status><name>Radio Horeb      </name></item><item><id>91_30</id><status>file</status><name>Radio Paradiso   </name></item><item><id>91_31</id><status>file</status><name>SCHLAGERPARADIES </name></item><item><id>91_32</id><status>file</status><name>Schwarzwaldradio </name></item><item><id>91_33</id><status>file</status><name>TIDE.radio       </name></item><item><id>91_34</id><status>file</status><name>lulu.fm          </name></item><item><id>91_35</id><status>file</status><name>pure fm Hamburg  </name></item><item><id>91_36</id><status>file</status><name>radio ffn        </name></item><item><id>91_37</id><status>file</status><name>sunshine live    </name></item></menu>
```
# gochild
http://192.168.11.8/gochild?id=91
```xml
<?xml version="1.0" encoding="UTF-8"?><result><id>91</id></result>
```
# playinfo
http://192.168.11.8/playinfo
work only on wlan interface?
Wire Interface:
```xml
<?xml version="1.0" encoding="UTF-8"?><result>FAIL</result>s
```
http://192.168.11.8/DABhotkeylist
```xml
<?xml version="1.0" encoding="UTF-8"?>
<menu>
  <item_total>5</item_total>
  <item_return>5</item_return>
  <item>
    <id>137_0</id>
    <status>file</status>
    <name>NDR 2            </name>
  </item>
  <item><id>137_1</id><status>file</status><name>Radio Hamburg    </name></item><item><id>137_2</id><status>file</status><name>KLASSIK RADIO    </name></item><item><id>137_3</id><status>file</status><name>N-JOY            </name></item><item><id>137_4</id><status>emptyfile</status><name>Leer</name></item></menu>
```
http://192.168.11.8/playDABhotkey?key=1
```xml
<?xml version="1.0" encoding="UTF-8"?><result><id>137</id><rt>OK</rt></result>
```
http://192.168.11.8/LocalPlay?url=http://192.168.11.100/msg.wav&name=intercom
```xml
```
http://192.168.11.8/LocalPlay?url=http://192.168.11.100/msg.wav&save=1
```xml
```
http://192.168.11.8/play_stn?id=91_6
```xml
```
http://192.168.11.8/irdevice.xml
```xml
```
http://192.168.11.8/stop
```xml
```
http://192.168.11.8/exit
```xml
```
## Sendkey from Remote Control
http://192.168.11.8/Sendkey?key=2
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><rt>OK</rt></result>
```

not checked. Could be wrong, please check yourself.

| Key | Description |
|-----|-------------|
| 2  | UP          |
| 8  | MUTE        |
| 4  | LEFT        |
| 6  | ENTER       |
| 5  | Right |
| 9  | Vol+ |
| 3  | Down |
| 10 | Vol - |
| 28 | Mode |
| 1  | Home |
| 15 | Star |
| 168| KEY |
| 12 | Sleep |
| 11 | Alarm |
| 14 | Light |
| 32 | prev |
| 29 | play/pause |
| 31 | next |
|115 | 1 |
|116 | 2 |
|116 | 3|
|117 | 4 |
|118 | 5 |
|19  | EQ |
|106 | OFF |
| 7  |  |

http://192.168.11.8/back
```xml
```
http://192.168.11.8:8080/playlogo.jpg
works only on WLAN?
```xml
```
http://192.168.11.8/background_play_status
```xml
```
http://192.168.11.8/GetFMFAVlist
```xml
```
http://192.168.11.8/GotoFMfav?fav=5
```xml
```
http://192.168.11.8/setvol?vol=9&mute=0
```xml
```
http://192.168.11.8/GetFMStatus
```xml
```
http://192.168.11.8/GetBTStatus
```xml
```
## Search for station
http://192.168.11.8/searchstn?str=radio
-> gibt id 100 zurück
```xml
```
Search Results
http://192.168.11.8/list?id=100&start=1&count=100
```xml
```
choose station
http://192.168.11.8/play_url?id=154_2
```xml
```
