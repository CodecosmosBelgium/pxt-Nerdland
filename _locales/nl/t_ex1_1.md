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
### Chatcommando
Je hebt verschillende blokjes die je uit de gereedschapskist moet verslepen naar het programmeerveld.
Het eerste blokje staat er al. Dit blokje zorgt ervoor dat als we straks iets typen, dat onze code wordt uitgevoerd.
Verander de naam van de chatopdracht in het blokje ``||Player:bij chatopdracht "jump"||`` naar ``||Player:bij chatopdracht "level1"||``.
 ``` blocks
player.onChat("level1", function () {
});
```

## Stap 2
### Zet Agent klaar
Nu moeten we de Agent klaarzetten. Hiervoor is er een blokje voorzien in de gereedschapskist, namelijk ``||CodeCosmos:zetKlaar||``.
Sleep het blokje ``||CodeCosmos:zetKlaar||`` in het blokje ``||Player:bij chatopdracht "level1"||``. Zorg ervoor dat de blokjes met elkaar verbonden zijn.
``` blocks
player.onChat("level1", function () {
    CodeCosmos.startingPosition()
});
```

## Stap 3
### Beweeg Agent
Zorg ervoor dat jouw Agent kan doorwandelen tot op het gouden blokje door het pad met de grijze blokjes te volgen.
Om de Agent te laten bewegen hebben we 2 verschillende blokjes: ``||Agent:agent beweegt vooruit met 1||`` en ``||Agent:agent draai links||``.
Je kan op het pijltje drukken om de richting te veranderen.
Sluit even de Code Builder om te kijken hoeveel blokjes jouw Agent vooruit moet gaan. 
Sleep het juiste blokje onder ``||CodeCosmos:zetKlaar||`` en zorg ervoor dat de Agent naar het gouden blokje wandelt.
``` blocks
player.onChat("level1", function () {
    CodeCosmos.startingPosition()
    agent.move(FORWARD, 1)
});
```

## Stap 4
### Controleer level
Laat de agent controleren of hij naar het volgende level mag.
Plaats het blokje ``||CodeCosmos:ga naar volgend level||`` bij de code.
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