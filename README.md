# CNAME based blocklist(s)

Currently a single `hosts` file containg online games blocklist.

Intended to work with Pi-hole or a similar DNS-based ad blocker.

An easy way to scrap google search results is (run in browser dev tools Console):

```
console.log([...new Set([...document.querySelectorAll("cite.tjvcx")].map(x => x.innerText).filter(n => n && n != "").map(x => x.split(" ")[0]).map(x => x.replace("http://", "0.0.0.0 ")).map(x => x.replace("https://", "0.0.0.0 ")))].join("\n"))
```
