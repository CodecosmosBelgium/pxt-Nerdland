### @hideIteration true
### @flyoutOnly true
# Opdracht 2 - Raket lanceren
```block
player.onChat("start", function () {
    CodeCosmos.startBuild()
    CodeCosmos.buildDiningRoom()
    CodeCosmos.buildLivingRoom()
    CodeCosmos.buildStorage()
    CodeCosmos.buildTop()
})
```

```template
player.onChat("jump", function() {
    
})
```

## Raket bouwen
Bekijk het instructieblad voor de juiste volgorde!
 ``` blocks
player.onChat("lanceren", function () {
    CodeCosmos.startBuild()
});
```