Detta är Möbius hemsida som skapades 2023.

För att uppdatera hemsidan så behöver man inte gå in och pilla på serverdatorn. Det du behöver göra är att klona ner detta repo till din dator:


```
git clone https://github.com/Moebius-Techare/moebius-hemsida
```

Kika in i den mappen. Sen behöver du lägga till serverdatorn som ett externt repo genom följade kommando:

```
git remote add web ssh://tech@ip/home/tech/hemsida
```

Där man ersätter 'ip' med den ip som hittas på *hostup* som hostar hemsidan.
Sen behöver man köra:

```
git push web +master:refs/heads/master
```

När man vill att servern ska få det som ligger på girrehurren.

(Jag använde mig av denna guide: <https://toroid.org/git-website-howto>)

Hemsidan fungerar som följande:

I `content` ligger markdown-filer som genereras till html via kommandot `hugo`. Det finns svenska och engelska filer, det syns på `.sv.md` och `.en.md`. 

Man kan genom att köra `./gen.sh` göra alla grejer automatiskt, kanske inte bästa ur ett säkerhetspespektiv men men...
