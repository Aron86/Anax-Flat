 Speedtest
===============================

<p><b>Urvalet</b>
<br>
I den här analysen har jag valt 3 av samma webbsidor som jag valde i min färganalys, och en helt ny nyhetssida.
<br>Anledningen till detta är för att få ett sammanhang där det blir som en fortsättning på föregående analys, och kanske ger det mig en djupare förståelse över hur designen påverkar hastigheten.
<br>Det är också dom hemsidorna jag besöker regelbundet, så det ger mig betydligt mer än att analysera någon hemsida jag aldrig besökt förut - tänker jag.
<br>
<br>Till min hjälp har jag använt verktyget <a href="https://developers.google.com/speed/pagespeed/">Google PageSpeed</a>
<br>Jag använder en windows 10 laptop med Google Chrome devtools för att mäta laddtiden osv. på reskpektive sida.
<br>Jag har tagit mätvärden på 3 undersidor för varje sida, och loggat snittet på 3 mätningar avrundat i hela sekunder (eftersom millisekunder inte påverkar upplevelsen märkbart). <br>
<br>Här är <a href="https://docs.google.com/spreadsheets/d/18f4sGt3aS2AbVt5eA3FQBPbSrRMiM0-SdiJCjNuvy2s/edit?usp=sharing">rådatan</a> som jag sammanställt i ett google kalkylark.
<br>
<br><b><a href="http://www.youtube.com">YouTube.com</a></b><br>
Youtube är en sida där användare kan lägga upp sina egna videor.<br>
<img src="img/youtube.jpg" alt="YouTube" width="600px">
<table style="width:100%">
  <tr>
    <th>Sida</th>
    <th>PageSpeed Desktop</th>
    <th>PageSpeed Mobile</th>
    <th>Resurser</th>
    <th>Storlek</th>
    <th>Laddningstid</th>
  </tr>
  <tr>
    <td>Youtube.com</td>
    <td>70/100</td>
    <td>54/100</td>
    <td>119</td>
    <td>1,9Mb</td>
    <td>ca 6s</td>
  </tr>
  <tr>
    <td>/feed/trending</td>
    <td>77/100</td>
    <td>46/100</td>
    <td>74</td>
    <td>818KB</td>
    <td>ca 4s</td>
  </tr>
  <tr>
    <td>/feed/subscriptions</td>
    <td>85/100</td>
    <td>85/100</td>
    <td>100</td>
    <td>850KB</td>
    <td>ca 5s</td>
  </tr>
</table>
<br>Jag noterar att mobilsidan presterar sämre enligt Google PageSpeed. Men till deras försvar så har ju Google en app för youtube (som inkluderas i google android) som det är tänkt att alla mobilanvändare ska använda, den är också väldigt populär. Så väldigt få (av youtubes totala användare) använder deras mobilhemsida. Jag vet inte hur man kan mäta appar ännu, men jag antar att deras app presterar bättre än mobilversionen av hemsidan. I övrigt har alla undersidor (desktop & mobilversionen) gemensamt att PageSpeed rekommenderar att optimisera bilder och undvika "redirects".
<br><br><b>Google PageSpeed rekommenderar följande:</b>
<br><br><b>Youtube.com: Desktop:</b> "Leverage browser caching, otimize images". <b>Mobile:</b> "Eliminate render-blocking JavaScript and CSS in above-the-fold content, Avoid landing page redirects."
<br><br><b>/feed/trending: Desktop:</b> Samma som ovan + "Eliminate render-blocking JavaScript and CSS in above-the-fold content, Avoid landing page redirects". <b>Mobile:</b> Samma som ovan + "Leverage browser caching, Optimize images".
<br><br><b>/feed/subscriptions: Desktop:</b> "Avoid landing page redirects". <b>Mobile:</b> "Eliminate render-blocking JavaScript and CSS in above-the-fold content, Prioritize visible content."
<br>
<br><b><a href="http://www.tomtop.com">TomTop.com</a></b><br>
Tomtop är en kinesisk sida som säljer lite av allt möjligt.
<br><img src="img/tomtop.jpg" alt="TomTop" width="600px">
<table style="width:100%">
  <tr>
    <th>Sida</th>
    <th>PageSpeed Desktop</th>
    <th>PageSpeed Mobile</th>
    <th>Resurser</th>
    <th>Storlek</th>
    <th>Laddningstid</th>
  </tr>
  <tr>
    <td>Tomtop.com</td>
    <td>33/100</td>
    <td>40/100</td>
    <td>340</td>
    <td>3,8Mb</td>
    <td>ca 17s</td>
  </tr>
  <tr>
    <td>/new-arrivals/</td>
    <td>55/100</td>
    <td>57/100</td>
    <td>160</td>
    <td>1,8Mb</td>
    <td>ca 11s</td>
  </tr>
  <tr>
    <td>/top-sellers/</td>
    <td>51/100</td>
    <td>57/100</td>
    <td>165</td>
    <td>2,0Mb</td>
    <td>ca 11s</td>
  </tr>
</table>
<br>Den här sidan fick väldigt dåliga betyg av Google PageSpeed.
<br>På alla desktop-sidorna så rekommenderar PageSpeed att bilderna bör optimiseras, samt "Leverage browser caching".
<br>Mobil-sidorna får samma rekomendationer som desktop, plus att man bör "Eliminate render-blocking JavaScript and CSS in above-the-fold content, Avoid landing page redirects".
<br>Men på det stora hela så tror jag att den dåliga laddningstiden beror på att alla sidor innehåller väldigt många stora ooptimiserade bilder.
<br><br><b>Google PageSpeed rekommenderar följande:</b>
<br><br><b>TomTop.com: Desktop:</b> "Leverage browser caching, otimize images". <b>Mobile:</b> Samma som desktop + "Eliminate render-blocking JavaScript and CSS in above-the-fold content, Avoid landing page redirects."
<br><br><b>/new-arrivals/: Desktop:</b> Samma som ovan. <b>Mobile:</b> Samma som desktop och samma som mobil-resultatet ovan.
<br><br><b>/top-sellers/: Desktop:</b> Samma som ovan. <b>Mobile:</b> Samma som desktop och samma som mobil-resultatet ovan.
<br>
<br><b><a href="http://www.omni.se">omni.se</a></b><br>
En Svensk nyhetssida.
<br>
<img src="img/omni.jpg" alt="omni" width="600px">
<table style="width:100%">
  <tr>
    <th>Sida</th>
    <th>PageSpeed Desktop</th>
    <th>PageSpeed Mobile</th>
    <th>Resurser</th>
    <th>Storlek</th>
    <th>Laddningstid</th>
  </tr>
  <tr>
    <td>omni.se</td>
    <td>72/100</td>
    <td>74/100</td>
    <td>107</td>
    <td>2,3Mb</td>
    <td>ca 6s</td>
  </tr>
  <tr>
    <td>/senaste</td>
    <td>72/100</td>
    <td>66/100</td>
    <td>93</td>
    <td>1,2Mb</td>
    <td>ca 4s</td>
  </tr>
  <tr>
    <td>/ekonomi</td>
    <td>79/100</td>
    <td>72/100</td>
    <td>99</td>
    <td>1,7Mb</td>
    <td>ca 5s</td>
  </tr>
</table>
<br>Omni kan förbättras genom att optimisera alla bilder, reducera serverns responstid, komprimera resurser, öka HTTP headerns utgångsdatum så att man utnyttjar cacheminnet för statiska resurser och optimera hur css koden körs, så att den inte blockar renderingen av sidan.
<br><br><b>Google PageSpeed rekommenderar följande:</b>
<br><br><b>Omni.se: Desktop:</b> "Leverage browser caching, Optimize images, Eliminate render-blocking JavaScript and CSS in above-the-fold content, Enable compression". <b>Mobile:</b> Samma som desktop.
<br><br><b>/senaste/: Desktop:</b> Samma som ovan. <b>Mobile:</b> Samma som desktop + "Reduce server response time".
<br><br><b>/ekonomi/: Desktop:</b> Samma som ovan. <b>Mobile:</b> Samma som desktop och samma som mobil-resultatet ovan.
<br>
<br><b><a href="http://www.svd.se/naringsliv">Svd.se/naringsliv</a></b><br>
En sida med nyheter om näringslivet och ekonomin.
<br>
<img src="img/svd.jpg" alt="svd" width="600px">
<table style="width:100%">
  <tr>
    <th>Sida</th>
    <th>PageSpeed Desktop</th>
    <th>PageSpeed Mobile</th>
    <th>Resurser</th>
    <th>Storlek</th>
    <th>Laddningstid</th>
  </tr>
  <tr>
    <td>svd.se/naringsliv</td>
    <td>58/100</td>
    <td>52/100</td>
    <td>184</td>
    <td>3,1Mb</td>
    <td>ca 10s</td>
  </tr>
  <tr>
    <td>/naringsliv/borsplus</td>
    <td>67/100</td>
    <td>53/100</td>
    <td>167</td>
    <td>3,2Mb</td>
    <td>ca 7s</td>
  </tr>
  <tr>
    <td>/naringsliv/motor</td>
    <td>59/100</td>
    <td>53/100</td>
    <td>174</td>
    <td>2,5Mb</td>
    <td>ca 7s</td>
  </tr>
</table>
<br>SVD näringslivs hemsida kan förbättras genom att man gör så att den använder cachen bättre, med bättre utgångsdatum i http-headern, och genom att man komprimerar några resurser och minifierar HTML-koden.
<br><br><b>Google PageSpeed rekommenderar följande:</b>
<br><br><b>svd.se/naringsliv: Desktop:</b> "Optimize images, Eliminate render-blocking JavaScript and CSS in above-the-fold content, Leverage browser caching, Enable compression, Minify HTML". <b>Mobile:</b> Samma som desktop.
<br><br><b>/naringsliv/borsplus: Desktop:</b> Samma som ovan. <b>Mobile:</b> Samma som desktop + Prioritize visible content.
<br><br><b>/naringsliv/motor: Desktop:</b> Samma som ovan. <b>Mobile:</b> Samma som desktop och samma som mobil-resultatet ovan.
<br>
<br>
<br>
<br>
<b>Sammanfattning</b>
<br>Dom absolut vanligaste förbättringsåtgärderna som faktiskt föreslås på samtliga fyra webbsidor är att optimera bilderna och att utnyttja cachelagringen i webbläsaren för statiska resurser (öka utgångsdatumen i HTTP-headern).
<br>Näst vanligaste förslaget till förbättring är att skjuta upp inläsningen av CSS och JavaScript som blockerar renderingen, eller infoga dom viktigaste delarna direkt i html-koden.
<br>
<br><b>Rangordning</b>
<br>1. YouTube.com
<br>2. Omni.se
<br>3. Svd.se/naringsliv
<br>4. TomTop.com
<br>
<br>Det var ett ganska väntat resultat eftersom jag alltid uppfattat youtube som en snabb och fräsh sida, dessutom ägs den ju av google.
<br>Rankningen av dom andra sidorna verkar ha påverkats mest av hur många och stora bilder dom har som inte är optimiserade.
<br>
<br>Min gräns för vad jag upplever som acceptabelt och långsamt (efter att ha analyserat dom här 4 sidorna) går vid ca 10 sekunder. Svd.se/naringsliv och TomTop.com var klart långsammare än dom andra. Jag är väldigt förvånad över att mitt urval presterade så dåligt och att hälften av sidorna fick så pass dåligt resultat.
<br>Jag hade inga gruppmedlemmar eftersom jag studerar på distans.
</p>
<br>
