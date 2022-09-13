# Lernbericht_LA1100

Rebecca Willi

## Einleitung

Ich habe im Lernatelier den Auftrag bekommen einen Number guesser zu erstellen.

## Was habe ich gelernt?

Ich habe gelernt was eine do-while Schleife macht.

## Beschreibung


Eine do-while Schleife wiederholt einen Vorgang solange die Ausgabe am Ende der Schleife auf die Angabe in der Oberen Klammer zutrifft. Das heisst, wenn man als Beispiel eingibt Ausgabe < als 5 wird dieser Vorgang solange wiederholt bis die Ausgabe nicht mehr kleiner als 5 ist. Beim Number guessers habe ich die do-while Schleife gebraucht, damit man weiterhin eine Zahl eingeben kann, wenn man die gesuchte Zahl noch nicht gefunden hat.Wenn die Schleife beendet ist und man die gesuchte Zahl noch nicht gefunden hat, beginnt die Schleife immer wieder von vorne.

```c#
do
    {

        Console.BackgroundColor = ConsoleColor.Red;
        Console.ForegroundColor = ConsoleColor.Cyan;
        double Geheimzahl = new Random().Next(1, 100);
        Console.WriteLine("Tippen sie eine Zahl zwischen 1 und 100.");
        string Zahl1 = Console.ReadLine();
        double Zahl = Convert.ToDouble(Zahl1);


        if (Zahl == Geheimzahl)
        {
            Console.WriteLine("Glückwunsch du hast die Zahl erraten");
            Console.ForegroundColor = ConsoleColor.Green;

        }
        while (Zahl != Geheimzahl)
        {
            if (Zahl < Geheimzahl)
            {
                Console.WriteLine("Die Geheimzahl ist grösser als " + Zahl);
            }
            else if (Zahl > Geheimzahl)
            {

                Console.WriteLine("die Geheimzahl ist kleiner als " + Zahl);
            }
            if (Zahl > 101)
            {

                Console.WriteLine("Falsche Eingabe Bitte gebën sie nur Zahlen zwischen 1 und 100 ein");
            }

            Console.WriteLine("Zahl ist inkorrekt.Geben sie eine andere Zahl ein");
            Zahl1 = Console.ReadLine();
            Zahl = Convert.ToDouble(Zahl1);


        }

        Console.WriteLine("Gratuliere sie haben die Zahl erraten");
        Console.WriteLine("Möchten sie noch eine Runde spielen?[y|n]");
        antwort = Console.ReadLine();
    } while (antwort == "y");
```



![dowhile2](https://user-images.githubusercontent.com/110892622/189844922-8364f76f-3841-4a02-b3cf-4dc59df767b6.jpg)

## Verifikation

Programmcode: Zeigt die do-while schleife, wie ich sie programmiert habe.

Text: Erklärt die do-while Schleife.

Foto: Zeigt die Wiederholung der do-while Schleife während das Programm läuft.

# Reflektion zum Arbeitsprozess

Was lief gut: 
Für mich persönlich lief das Planen mit der Projektdokumentation gut, da ich für mich so Anhaltspunkte hatte für das spätere programmieren, wodurch ich die Zeit effizienter nutzen konnte.

Was weniger gut lief: 
Am Anfang hatte ich beim Programmieren Probleme da ich gewisse Begriffe verwechselt habe. Zudem wollte ich zu viel im Programm einfügen und hatte am Schluss keine Zeit mehr. So musste ich einige Sachen weglassen welche noch gut gewesen wären.

**VBV**:Ich sollte für das nächste mal überlegen, was ich wirklich im Programm brauche und welche Sachen ich auch weglassen kann und dann die wichtigen zuerst programmieren.
