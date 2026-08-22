# phaedrus-fabulae

Phaedra (Faidra) fabulu teksti un to sintaktisko saišu (`.phr`) faili — daļa no
[Syntra](https://lingua.id.lv/) ekosistēmas (Carpe Diem / Syntra platforma
valodu apguvei ar AI).

## Struktūra

Katrs `.txt`/`.phr` pāris dalās vienā failu nosaukumā (bez paplašinājuma),
piem., `txt/De_Vulpe_et_Uva.txt` ↔ `phr/De_Vulpe_et_Uva.phr`.

## `.phr` faila formāts

Katra rinda ir viena sintaktiskās saites grupa — vārdu virkne, kur katram
vārdam pievienota tā **absolūtā pozīcija tekstā** (skaitot no 1, ieskaitot
virsrakstu):

Pozīcijas atbilst vienkāršai tokenizācijai: viss teksts (virsraksts + fabula
+ "Interpretatio Latina" virsraksts + parafrāze) sadalīts pēc burtu virknēm
(`[A-Za-z]+`), pieturzīmes un atstarpes ignorējot. Viena vārda forma var
piederēt **vairākām** grupām vienlaikus (pārklāšanās) — tas nav vienkāršs
1-pret-1 sarakstas modelis.

## Statuss

Šobrīd repozitorijā ir 3 pilnas fabulas (teksts + saites). Pilnajā Faidra
fabulu krājumā ir 44 fabulas — pārējās vēl jāpievieno.

Skatīšanās/veidošanas rīks: `Phaedrus_syntax_overlap_editor.html`
(Syntra ekosistēmā).
