### @hideIteration false
### @flyoutOnly true
# Oefening 1 - Agent testen
```blocks
player.onChat("oef1", function () {
    CodeCosmos.startingPosition()
    agent.move(FORWARD, 6)
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 3)
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 5)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 10)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 10)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 10)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 3)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 1)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(RIGHT_TURN)
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 6)
    CodeCosmos.goToNextLevel()
})
```

```template
player.onChat("jump", function () {

})
```

## Stap 1
### Verander jump naar level2
Verander de naam van de chatopdracht van het blokje ``||Player:bij chatopdracht "jump"||`` naar ``||Player:bij chatopdracht "level2"||``.
 ``` blocks
player.onChat("level2", function () {
});
```

## Stap 2
### Zet Agent klaar
Sleep het blok ``||Agent:zetKlaar||`` in het blok ``||Player:bij chatopdracht "level1"||``
``` blocks
player.onChat("level1", function () {
    CodeCosmos.startingPosition()
});
```

## Stap 3
### Beweeg Agent
Zorg ervoor dat jouw Agent kan doorwandelen tot op het gouden blokje door het pad met de grijze blokjes te volgen. 
Gebruik daarvoor het blok ``||Agent:Agent beweegt vooruit met ...||``.
Verander zeker het aantal stappen dat de Agent moet zetten!
``` blocks
player.onChat("level1", function () {
    CodeCosmos.startingPosition()
    agent.move(FORWARD, 1)
});
```

## Stap 4
### Controleer level
Laat de agent controleren of hij naar het volgende level mag. 
Plaats het blokje 'ga naar volgend level' bij de code. 
Er zal pas iets gebeuren als je een chatcommando uitvoert. 
``` blocks
player.onChat("level1", function () {
    CodeCosmos.startingPosition()
    agent.move(FORWARD, 6)
    CodeCosmos.goToNextLevel()
});
```

## Stap 5
### Voer code uit
Je code is nu klaar om te testen. Hier is wat je nu moet doen om de code uit te voeren.
- Druk op de **groene startknop**
- Open het chatvenster door op de **T**-toets te drukken
- Typ het commando '**level1**' dat je daarnet hebt aangemaakt
- Druk op **enter of het pijltje rechtsonder** om het commando uit te voeren!