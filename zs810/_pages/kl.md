---
layout: page
title: About
permalink: /kl/
---
1. sudo vi /usr/share/X11/xkb/symbols/zi /usr/share/X11/xkb/rules/base.lst /usr/share/X11/xkb/rules/evdev.xml
2. setxkbmap zi

1. ADertyuiop\[\]_ qwERXYUIOP{}\|
2. asdNghHkl;' QSWfGJjKL:" 
3. zTcvbnm,./ ZxCVBFM<>?
/usr/share/X11/xkb/symbols
/usr/share/X11/xkb/rules/evdev.xml
    /etc/default/keyboard
    /usr/share/x11/xkb
    xev -event keyboard
    setxkbmap -layout us
    
    cinnamon-settings keyboard

    <TLDE> for the grave accent/tilde key

    <BKSL> for the backslash/bar key

    <AB01>, <AB02> and so on for Z, X … keys

    <AC01>, <AC02> and so on for A, S … keys

    <AD01>, <AD02> and so on for Q, W … keys

    <AE01>, <AE02> and so on for 1, 2 … keys
/usr/share/X11/xkb can be divided in 3 groups accordingly to their aim:

    files to graphically display the keyboard layout
    files to configure the key mapping and the keyboard layout
    files to enable the configuration

├── geometry      # this is group 1├── keycodes      # this is group 2

├── rules         # this is group 3├── symbols       # this is group 2
https://medium.com/@damko/a-simple-humble-but-comprehensive-guide-to-xkb-for-linux-6f1ad5e13450

https://askubuntu.com/questions/482678/how-to-add-a-new-keyboard-layout-custom-keyboard-layout-definition
===================/usr/share/X11/xkb/rules/evdev.xml
<layout>
<configItem>
<name>bt</name>
<!-- Keyboard indicator for Dzongkha layouts -->
<shortDescription>dz</shortDescription>
<description>Dzongkha</description>
<languageList>
<iso639Id>dzo</iso639Id>
</languageList>
</configItem>
</layout>
=============
<layout>
<configItem>
<name>zi</name>
<!-- Keyboard indicator for zinglishzava810 layouts -->
<shortDescription>zi</shortDescription>
<description>zinglishzava810</description>
<languageList>
<iso639Id>zi</iso639Id>
<iso639Id>hin</iso639Id>
<iso639Id>nep</iso639Id>
<iso639Id>urd</iso639Id>
<iso639Id>ben</iso639Id>
<iso639Id>sat</iso639Id>
<iso639Id>eng</iso639Id>
<iso639Id>bos</iso639Id>
<iso639Id>hbs</iso639Id>
<iso639Id>hrv</iso639Id>
<iso639Id>ind</iso639Id>
<iso639Id>msa</iso639Id>
<iso639Id>min</iso639Id>
<iso639Id>ace</iso639Id>
<iso639Id>bjn</iso639Id>
<iso639Id>tsg</iso639Id>
<iso639Id>mfa</iso639Id>
</languageList>
<countryList>
  <iso3166Id>JP</iso3166Id>
  <iso3166Id>AR</iso3166Id>
  <iso3166Id>BO</iso3166Id>
  <iso3166Id>CL</iso3166Id>
  <iso3166Id>CO</iso3166Id>
  <iso3166Id>CR</iso3166Id>
  <iso3166Id>CU</iso3166Id>
  <iso3166Id>DO</iso3166Id>
  <iso3166Id>EC</iso3166Id>
  <iso3166Id>GT</iso3166Id>
  <iso3166Id>HN</iso3166Id>
  <iso3166Id>HT</iso3166Id>
  <iso3166Id>MX</iso3166Id>
  <iso3166Id>NI</iso3166Id>
  <iso3166Id>PA</iso3166Id>
  <iso3166Id>PE</iso3166Id>
  <iso3166Id>PR</iso3166Id>
  <iso3166Id>PY</iso3166Id>
  <iso3166Id>SV</iso3166Id>
  <iso3166Id>US</iso3166Id>
  <iso3166Id>UY</iso3166Id>
  <iso3166Id>VE</iso3166Id>
</countryList>
</configItem>
</layout>
    ===========/usr/share/X11/xkb/symbols/au
    default  partial alphanumeric_keys
xkb_symbols "basic" {
    include "us(basic)"

    name[Group1]= "English (Australian)";
};
    ================
=================