## Oppgaven
Vi har et oppgave som handler om Javascript IF statement og For loops. Det er fem oppgaver.

## Oppgave 1
Skriv et JavaScript-program for å konvertere temperaturer til og fra Celsius, Fahrenheit. Du trenger to blokker for å se resultatet.

## Løsning
---

var celcius = parseInt(prompt("skriv inn temperatur i celcius"))
var fahrenheit = celcius*1.8+32

document.write(celcius + "C er "+fahrenheit+"F")
document.write(fahrenheit + "F er "+celcius+"C")

---

## Eksempel Output
32C er 89.6F
89.6F er 32C

## Oppgave 2
Skriv et JavaScript-program for å få forskjellen mellom et gitt tall og 10. Hvis tallet er større enn 10 returner det dobbelte av den absolutte forskjellen.

## Løsning
---

var number = parseInt(prompt("skriv et tall"))

if (number > 10) {
    document.write((number-10)*2)
}
else if (number < 10) {
    document.write(10-number)
}
else {
    document.write(number-number)
}

---
## Eksempel Output

IF statement: ((22-10) * 2 = 24)

ELSE IF statement: (10-7 = 3)

ELSE statement: (10-10 = 0)

## Oppgave 3
Skriv et JavaScript-program for å beregne summen av de to gitte tallene. Hvis de to verdiene er like, returnerer de tredoblet summen.

## Løsning
---

var number1 = parseInt(prompt("skriv et tall"))
var number2 = parseInt(prompt("skriv et tall"))

if (number1 > number2 || number1 < number2) {
    document.write(number1+number2)
}
else {
    document.write((number1+number2)*3)
}

---

## Eksempel Output
IF statement: (5+20 = 25)

ELSE statement: ((7+7)*3 = 42)

## Oppgave 4
Skriv et JavaScript-program for å sjekke to gitte tall og returner true hvis ett av tallene er 50 eller hvis summen deres er 50. Ellers resultatet blir false.

## Løsning
---

var number1 = parseInt(prompt("skriv et tall"))
var number2 = parseInt(prompt("skriv et tall"))

if (number1 == 50 && number2 == 50) {
    document.write("begge tall er 50")
}
else if (number1 == 50 || number2 == 50) {
    document.write("en av tallene er 50")
}
else if (number1 + number2 == 50) {
    document.write("summen av tallene er 50)
}
else (false)

---

## Eksempel Output

Hvis jeg skriver 50 og 50, blir eksempel output: (begge tall er 50)

Hvis jeg skriver 40 og 50, blir eksempel output: (en av tallene er 50)

Hvis jeg skriver 40 og 40, blir eksempel output ingenting.

Hvis jeg skriver 30 og 20, blir eksempel output: (summen av tallene er 50)

## Oppgave 5
Skriv et JavaScript-program for å lage følgende mønster ved å bruke nested for-loop

## Løsning
---

var x, y, chr;

for (x = 1; x <= 6; x++) {
    for (y = 1; y < x; y++) {
        chr = chr + ("*");
    }
    console.log(chr);
    chr = '';
}

for (x = 1; x <= 6; x++) {
    for (y = 6; y > x; y--) {
        chr = chr + ("*");
    }
    console.log(chr);
    chr = '';
}

---

