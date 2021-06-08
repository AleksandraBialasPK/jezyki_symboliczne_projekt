#Gra w tysiaca
Aleksandra Białas, nr albumu: 130492
Github: https://github.com/AleksandraBialasPK/jezyki_symboliczne_projekt
Projekt z przedmiotu języki symboliczne.
Umożliwia przeprowadzenie rozgrywki popularnej gry karcianej.
Zasady gry oraz jej przebieg znajdują się pod linkiem: https://pl.wikipedia.org/wiki/Tysi%C4%85c_(gra)
Komunikację umożliwia WebSocket.
Wykorzystywany jest framework Tornado.
Każdy z graczy może dołączyć ze swojej przeglądarki.

#Wymagania

Aplikacja wymaga:
* Python 3.7 lub nowszy
* pip 10.0.x lub nowszy
* Tornado 6 lub nowszy

By zainstalować Tornado:
```
pip install -r requirements.txt
```

Uruchomienie:

Zanim uruchomisz program sprawdź:

MessageHandler.js
```
MessageHandler.host = "162.158.91.111"; // or localhost
MessageHandler.port = ":8888";
```
main.py
```
app.listen(8888)
```

Następnie:
```
python main.py
```

Otwórz w przeglądarce:
_localhost:8888_
 
Otwarcie czterech kart umożliwia grę na localhoscie, ale jeśli wybierzesz inny adres niż localhost, to powinieneś go użyć na pozostałych maszynach.

#Testy
```
python -m unittest discover -s Tests -p 'Test*.py' 
```

