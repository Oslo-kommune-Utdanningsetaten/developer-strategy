# Ekstra retningslinjer for utvikling av åpen programvare

Man skal ha gode grunner for ikke å gjøre kode offentlig tilgjengelig - typisk i et public repo på GitHub, men før du gjør kode public, er det viktig at du og teamet ditt har tenkt igjennom følgende spørsmål:

1. Finnes det et scenarie der noen andre kan ha interesse av koden?
2. Greier vi å holde koden ren for data som ikke bør være åpen?
3. Har koden høy nok kvalitet, til at den tåler dagens lys?
4. Kommer vi til å vedlikeholde kode, dokumentasjon og issues?
5. Har vi tatt stilling til lisens (vilkår for bruk) av koden?

Hvis svaret på noen av disse spørsmålene er NEI, er nok ikke koden klar for public status ennå. Her er en veiledning/kommentar til disse spørsmålene:

1. Som regel er svaret på dette JA. Det finnes alltid en nysgjerrig-per som lurer på hva Oslo Kommune driver med. Kanskje en foresatt lurer på hvordan en algoritme vekter et resultet. En utvikler lurer på hvordan du har løst gruppe-synkronisering. En journalist lurer på hvilke datakilder som brukes. Og så videre. I tillegg har skattebetalerne betalt for denne koden, og de må kunne sjekke hva de har fått for pengene sine.
2. Dette er viktig enten repo er public eller private, men ekstra viktig når repo er public. Svaret på dette spørsmålet bør være JA uansett. Passord ligger typisk i en `.env`-fil og data ligger i databasen. Ingen av disse skal publiseres i et repo.
3. Hvis svaret her er NEI, er kanskje ikke koden god nok til å brukes?
4. Andres nytte av koden vil reduseres ved manglende vedlikehold. Husk at ikke bare kode, men også dokumentasjon og issues bør vedlikeholdes.
5. Det er fint å slippe å forfatte egen lisens, og det er [flere alternativer](https://en.wikipedia.org/wiki/Permissive_software_license) å velge mellom. [NAV](https://github.com/navikt) og [Oslo Kommune](https://github.com/oslokommune) bruker stort sett MIT-lisens for sin åpne kode. Dette er en lisens som både gir andre frihet og utviklerne trygghet.
