
# DABMAN i450 Remote Control

## Syntax for curl
```curl -H 'Authorization: Basic c3UzZzRnbzZzazc6amkzOTQ1NHh1L14=' http://<DEVICE>/<COMMAND>```
## Example (send "Enter"):
```curl -H 'Authorization: Basic c3UzZzRnbzZzazc6amkzOTQ1NHh1L14=' http://dabman/Sendkey?key=6```

or with ip

```curl -H 'Authorization: Basic c3UzZzRnbzZzazc6amkzOTQ1NHh1L14=' http://192.168.11.8/Sendkey?key=6```

# COMMANDS

## INIT
http://dabman/init?language=de

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
http://dabman/hotkeylist
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
http://dabman/list?id=1&start=1&count=15
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
http://dabman/list?id=91&start=1&count=500
```xml
<?xml version="1.0" encoding="UTF-8"?>
<menu><item_total>37</item_total><item_return>37</item_return><item><id>91_1</id><status>file</status><name>80s80s           </name></item><item><id>91_2</id><status>file</status><name>917XFM           </name></item><item><id>91_3</id><status>file</status><name>ANTENNE-SYLT     </name></item><item><id>91_4</id><status>file</status><name>Absolut relax    </name></item><item><id>91_5</id><status>file</status><name>DRadio DokDeb    </name></item><item><id>91_6</id><status>file</status><name>Dlf              </name></item><item><id>91_7</id><status>file</status><name>Dlf Kultur       </name></item><item><id>91_8</id><status>file</status><name>Dlf Nova         </name></item><item><id>91_9</id><status>file</status><name>ENERGY DIGITAL   </name></item><item><id>91_10</id><status>file</status><name>ERF Plus         </name></item><item><id>91_11</id><status>file</status><name>ERF Pop          </name></item><item><id>91_12</id><status>file</status><name>HAMBURG ZWEI     </name></item><item><id>91_13</id><status>file</status><name>HLRdigital       </name></item><item><id>91_14</id><status>file</status><name>KLASSIK RADIO    </name></item><item><id>91_15</id><status>file</status><name>MegaRadio        </name></item><item><id>91_16</id><status>file</status><name>N-JOY            </name></item><item><id>91_17</id><status>file</status><name>NDR 2            </name></item><item><id>91_18</id><status>file</status><name>NDR 90,3         </name></item><item><id>91_19</id><status>file</status><name>NDR Blue         </name></item><item><id>91_20</id><status>file</status><name>NDR Info         </name></item><item><id>91_21</id><status>file</status><name>NDR Info Spezial </name></item><item><id>91_22</id><status>file</status><name>NDR Kultur       </name></item><item><id>91_23</id><status>file</status><name>NDR Plus         </name></item><item><id>91_24</id><status>file</status><name>PELI ONE         </name></item><item><id>91_25</id><status>file</status><name>R.SH - Hamburg   </name></item><item><id>91_26</id><status>file</status><name>RADIO BOB!       </name></item><item><id>91_27</id><status>file</status><name>ROCK ANTENNE HH  </name></item><item><id>91_28</id><status>file</status><name>Radio Hamburg    </name></item><item><id>91_29</id><status>file</status><name>Radio Horeb      </name></item><item><id>91_30</id><status>file</status><name>Radio Paradiso   </name></item><item><id>91_31</id><status>file</status><name>SCHLAGERPARADIES </name></item><item><id>91_32</id><status>file</status><name>Schwarzwaldradio </name></item><item><id>91_33</id><status>file</status><name>TIDE.radio       </name></item><item><id>91_34</id><status>file</status><name>lulu.fm          </name></item><item><id>91_35</id><status>file</status><name>pure fm Hamburg  </name></item><item><id>91_36</id><status>file</status><name>radio ffn        </name></item><item><id>91_37</id><status>file</status><name>sunshine live    </name></item></menu>
```
# gochild
http://dabman/gochild?id=91
```xml
<?xml version="1.0" encoding="UTF-8"?><result><id>91</id></result>
```
# playinfo
http://dabman/playinfo
work only on wlan interface?
Wire Interface:
```xml
<?xml version="1.0" encoding="UTF-8"?><result>FAIL</result>s
```
http://dabman/DABhotkeylist
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
http://dabman/playDABhotkey?key=1
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><id>137</id><rt>OK</rt></result>
```

http://dabman/LocalPlay?url=http://192.168.11.100/msg.wav&name=intercom
seams to work only for special files/domains

```xml
```

http://dabman/LocalPlay?url=http://192.168.11.100/msg.wav&save=1
```xml
<result><rt>OK</rt></result>
```

http://dabman/play_stn?id=91_6
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><id>91_6</id><isfav>0</isfav></result>
```
http://dabman/irdevice.xml
```xml
<?xml version="1.0"?>
<root>
<device>
<friendlyName>dabman-sz</friendlyName>
</device>
</root>
```
http://dabman/stop
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result>OK</result>
```
http://dabman/exit
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result>OK</result>
```

## Sendkey from Remote Control
http://dabman/Sendkey?key=2
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

http://dabman/back
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><id>52</id></result>
```

http://dabman:8080/playlogo.jpg
works only if Radiostation has a play logo



http://dabman/background_play_status
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><sid>6</sid><playtime_left>00:00:00</playtime_left><vol>9</vol><mute>0</mute></result
```

http://dabman/GetFMFAVlist
```xml
<?xml version="1.0" encoding="UTF-8"?><menu><item_total>26</item_total><item_return>26</item_return><item><id>1</id><Freq>87.60</Freq></item><item><id>2</id><Freq>88.70</Freq></item><item><id>3</id><Freq>89.10</Freq></item><item><id>4</id><Freq>89.50</Freq></item><item><id>5</id><Freq>90.30</Freq></item><item><id>6</id><Freq>91.70</Freq></item><item><id>7</id><Freq>92.30</Freq></item><item><id>8</id><Freq>93.00</Freq></item><item><id>9</id><Freq>94.20</Freq></item><item><id>10</id><Freq>95.00</Freq></item><item><id>11</id><Freq>96.00</Freq></item><item><id>12</id><Freq>97.10</Freq></item><item><id>13</id><Freq>98.10</Freq></item><item><id>14</id><Freq>99.20</Freq></item><item><id>15</id><Freq>100.00</Freq></item><item><id>16</id><Freq>100.60</Freq></item><item><id>17</id><Freq>102.90</Freq></item><item><id>18</id><Freq>103.20</Freq></item><item><id>19</id><Freq>103.60</Freq></item><item><id>20</id><Freq>104.00</Freq></item><item><id>21</id><Freq>104.50</Freq></item><item><id>22</id><Freq>105.10</Freq></item><item><id>23</id><Freq>106.40</Freq></item><item><id>24</id><Freq>106.80</Freq></item><item><id>25</id><Freq>107.40</Freq></item><item><id>26</id><Freq>108.00</Freq></item></menu>
```
http://dabman/GotoFMfav?fav=5
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result>OK</result>
```

http://dabman/setvol?vol=9&mute=0
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><vol>9</vol><mute>0</mute></result>s
```

http://dabman/GetFMStatus
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><vol>1</vol><mute>0</mute><Signal>3</Signal><Sound>STEREO</Sound><Search>FALSE</Search><Freq>90.30</Freq><RDS> </RDS></result>
```

http://dabman/GetBTStatus
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><vol>1</vol><mute>0</mute><Status>2</Status></result>
```
## Search for station called Radio
http://dabman/searchstn?str=radio
-> returns id=100
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><id>100</id><rt>OK</rt></result>
```

curl 'http://dabman/gochild?id=100'
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result><id>100</id></result>
```

Search Results
http://dabman/list?id=100&start=1&count=100
```xml
<?xml version="1.0" encoding="UTF-8"?><menu><item_total>248</item_total><item_return>20</item_return><item><id>100_1</id><status>file</status><name>#%RD RADIO.DISCOunt</name></item><item><id>100_2</id><status>file</status><name>#POPHITS</name></item><item><id>100_3</id><status>file</status><name>#Pop Radio</name></item><item><id>100_4</id><status>file</status><name>'t Is Vloms Radio</name></item><item><id>100_5</id><status>file</status><name>'MEGA RADIO</name></item><item><id>100_6</id><status>file</status><name>(((EBM Radio)))</name></item><item><id>100_7</id><status>file</status><name>(a)ac Radio FM</name></item><item><id>100_8</id><status>file</status><name>1 Classic</name></item><item><id>100_9</id><status>file</status><name>1 HITS 50s</name></item><item><id>100_10</id><status>file</status><name>1 HITS 60s</name></item><item><id>100_11</id><status>file</status><name>1 HITS 70s</name></item><item><id>100_12</id><status>file</status><name>1 HITS 80s</name></item><item><id>100_13</id><status>file</status><name>1 HITS 90s</name></item><item><id>100_14</id><status>file</status><name>1 MASTER HIP-HOP</name></item><item><id>100_15</id><status>file</status><name>1 Music Radio</name></item><item><id>100_16</id><status>file</status><name>1 Pure EDM Radio</name></item><item><id>100_17</id><status>file</status><name>1 Radio Dance</name></item><item><id>100_18</id><status>file</status><name>1 Radio Jazz</name></item><item><id>100_19</id><status>file</status><name>1 Radio Lounge</name></item><item><id>100_20</id><status>file</status><name>1-Dance</name></item></menu>
```
choose station
http://dabman/play_url?id=154_2
```xml
<?xml version="1.0" encoding="UTF-8"?>
<result>
 <url>http://b1.mediayou.net/embedded/playURL_sleep.php?id=2&sc=N9XX_AAC</url>
</result>
```


# Other Commands not by the Android App

## Webpage
http://dabman/


http://dabman/set_dname?name=dabman-sz

http://dabman/scan_wifi

http://dabman/scan_results


## UPNP

http://dabman:52525/root_XXYY.xml

see file root_XXYY.xml

http://dabman:52525/root_XXYY_S.xml

see file root_XXYY_S.xml

http://dabman:52525/walkie_XXYY_S.xml

see file walkie_XXY_S.xml
