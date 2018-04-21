# Kopirovat-kalendar-Google

Google script, který kopíruje tabulku pracovních služeb podle určeného jména do formátu pro import do Google Kalendáře. Další krok bude, aby to do kalendáře dával sám. 

Tady starý výpočet  buňky, která z kalendáře služeb vytváří řádky: =IF(AND(weekday(B3;2)>5;K3<>"Štěpán");"";IF(LEFT(TO_TEXT(C3);2)="8:";"Od osmi";IF(LEFT(TO_TEXT(C3);2)="6:";"Ranní";IF(LEFT(TO_TEXT(C3);2)="9:";"Šéfovská";IF(LEFT(TO_TEXT(C3);2)="12";"Od dvanácti";IF(LEFT(TO_TEXT(C3);2)="14";"Odpolední";"chyba"))))))
