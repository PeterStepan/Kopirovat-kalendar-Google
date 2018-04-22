# Kopirovat-kalendar-Google

Google script, který kopíruje tabulku pracovních služeb podle určeného jména do formátu pro import do Google Kalendáře. Obsahuje už i funkci, která kalendář sama importuje do zvoleného Google kalendáře. Nově obsahuje i funkci, která zabraňuje duplicitám. Lze si vybrat, zda má kalendář ignorovat ostatní události v daném dni (nutno ručně smazat případné změněné směny), nebo jestli má tolerovat pouze jednu událost za den (což zabraňuje jakýmkoliv duplicitám, ale je nutné mít pro směny samostatný kalendář).

Tady starý výpočet  buňky, která z kalendáře služeb vytváří řádky: =IF(AND(weekday(B3;2)>5;K3<>"Jmeno");"";IF(LEFT(TO_TEXT(C3);2)="8:";"Od osmi";IF(LEFT(TO_TEXT(C3);2)="6:";"Ranní";IF(LEFT(TO_TEXT(C3);2)="9:";"Svátek";IF(LEFT(TO_TEXT(C3);2)="12";"Od dvanácti";IF(LEFT(TO_TEXT(C3);2)="14";"Odpolední";"chyba"))))))
