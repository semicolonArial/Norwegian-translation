# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[SPILL!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Så før vi starter, hvordan ville *du* likt å lese?

`publish("show_options_bottom")`

# intro-start-2

n3: Nå, la oss begynne vår historie...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: DETTE ER ET MENNESKE

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: OG DETTE ER MENNESKETS ANGST

n: _DU_ ER ANGSTEN

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Niks. Nei, niks, jeg hører ikke etter. Skal sjekke mobilen min isteden.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: JOBBEN DIN ER Å BESKYTTE MENNESKET DITT FRA *FARE*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Gisp! Du skroller livet ditt vekk på Twitter! Igjen!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Vel, jeg lurer på hvorfor jeg ikke bare sitter meg ned og lytter til tankene mine oftere.

`hong({eyes:"neutral"});`

n: NÅ, ADVAR DEM OM EN *FARE!*

```
bb({eyes:"look"});
```

[Å nei, se på den forferdelige nyhetssaken!](#act1d_news)

[Å nei, handler det innlegget egentlig om *oss?*](#act1d_subtweet)

[Hei, en gif om en kat som drikker melk.](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh ya that's cute, I-- Huh ja det er søtt, je--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KATTER KAN IKKE FORDØYE MELK OG VI ER FORFERDELIGE FOLK FOR Å GLEDE OSS OVER DYREMISHANDLING

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



