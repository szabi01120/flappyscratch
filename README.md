# flappyscratch
A projektben megcsináltam a játék normális működésének érdekében:
- a gravitációt
- a pontszám mérőt (erre egy nagyon egyszerű megoldást alkalmaztam, ha eltűnik a pipe sprite, mindig hozzáad a változóhoz 1-et - ugyanis innen lehet tudni, hogy a karakterünk nem ütközött neki a pipenak (collision) -, ha vége a játéknak akkor mindig kinullázza.)
- a karakter a space billentyűvel tud felfelé ugrálni (az az opció is kizárásra került, hogy a space folyamatos nyomvatartásával folyamatosan ugráljon felfelé)
- ha collision (ütközés) történik, a játék EndPhase-be kapcsol, ahol minden script leáll és egy costume jelenik meg, amire ki van írva a 'Vége a játéknak!' felirat. A zöld zászló újbóli megnyomásával a játék újraindul.
- ha a karakterünket nem mozgatjuk és leesik, akkor a játék szintén az EndPhase-be lép, ahol minden a korábban említett üzemmódba lép, vagyis leáll a játék.
- a pipe-ok 1 másodpercenént klónozzák magukat, és a helyük is változik. Itt az X koordinátát fixáltam, az Y koordinátát pedig random generálja a rendszer egy általam megadott intervallumon.
- a játékban hallani egy zenét, ami kikapcsol, amint véget ér számunkra a játék.
