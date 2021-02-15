# Netzwerk VfB Codebuch #
Codebuch Stand 2021-02-15<br>
erstellt von Eileen Wagner (ew043@hdm-stuttgart.de)

## Inhalt
- netzwerkvfb_NetzwerkVFB_Edgelist.csv (Edgelist)
- netzwerkvfb_NetzwerkVFB_Nodelist.csv (Nodelist)
- netzwerkvfb_CodebuchVFB.csv (Codierung der Datensätze)


# Edgelist

Grundregel: Die Edgelist darf pro Spalte immer nur einen Wert enthalten. Bis auf die ID idealerweise numerisch codiert (als Zahl). Fehlende Werte werden mit NA gekennzeichnet (bei der Erhebung einfach weglassen)

**from**

definiert die natürliche Person, von der eine Mitgliedschaft ausgeht. Entspricht ID in der Nodelist. Keine Sonderzeichen, nur ein Wort (z.B. TH)            

**to**

definiert alle aktiven Mitgliedschaften einer Person. Entspricht ID in der Nodelist. Keine Sonderzeichen, etc. (z.B. DBA)

**time**

definiert das Jahr, in dem die Person einer Mitgliedschaft beigetreten ist, wird als natürliche Zahl angegeben (z.B. 2010). Bei abgebrochenen Mitgliedschaften, zählt das Jahr,in der eine neue Mitgliedschaft begonnen wurde.

**duration**

gibt die Dauer an, in der eine Person für eine bestimmte Position zuständig war, wird als Skalierung angegeben. 

1 = bis 1 Jahr 
2 = zwei bis sechs Jahre
3 = mehr als sechs Jahre
4 = Mitgliedschaft besteht noch


# Nodelist

Grundregel: die IDs der Nodelist müssen mit den IDs der Edgelist komplett übereinstimmen. Ausprägungen der Attribute in der Regel numerisch definieren. Fehlende Werte werden mit NA gekennzeichnet (bei der Erhebung einfach weglassen) 

**id**

eindeutige Codierung des Knoten, wird als nominale Abkürzung angegeben (z.B. Thomas Hitzlsperger = TH)         

**name**

Vollständiger Name des Knotens (z.B. VfB Stuttgart 1893 AG)

**type**

Unterscheidung zwischen Person und Organisation, wird als Skalierung angegeben

0 = Person
1 = Organisation 

**age**

gibt das Alter der natürlichen Person an, wird als Skalierung angegeben

1 = 26 bis 39 
2 = 40 bis 59 
3 = über 60 

**education**

gibt den Bildungsstand der natürlichen Person an, wird als Skalierung angegeben

1 = Hauptschule 
2 = Mittlere Reife 
3 = Fachhochschulreife 
4 = Abitur 
5 = Studium 
6 = Promotion      

**football**

gibt an, ob die natürliche Person Fußballspieler oder Trainer war bzw. ist, wird als Skalierung angegeben

1 = kein Fußballspieler 
2 = Fußballspieler 
3 = Trainer 

**function**

definiert die Mitgliedschaft in einem Organ des VfB-Clubs an, wird als nominale Abkürzung angegeben

V = Vorstand 
AR = Aufsichtsrat 

**representation**

definiert die Funktion der natürlichen Person innerhalb der VfB-Gremien, wird als Skalierung angegeben

1 = Politik 
2 = Wirtschaft 
3 = Gewerkschaft 
4 = Umwelt 
5 = Sport 
6 = Wissenschaft 
7 = Marketing und Kommunikation 

**position**

definiert die besondere Position der natürlichen Person innerhalb des VfB-Clubs, wird als Skalierung angegeben

1 = Vorsitz 
2 = Stellvertreter 
3 = Mitglied in der VFB-Organisation 

