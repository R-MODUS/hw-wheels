# hw-wheels

Katalog **kol pro mobilní roboty** (mecanum i další varianty) — použitelný i mimo R-MODUS.

Součást katalogu: [R-MODUS](https://github.com/R-MODUS) · kontext systému: [doc-thesis](https://github.com/R-MODUS/doc-thesis)

<p align="center">
  <img src="variants/mecanum-100mm/image/mecanum-wheel.png" alt="Mecanum kolo" width="360"/>
</p>

## Účel

Katalog mechanických kol. Toto repo **neobsahuje firmware ani ROS** — jen mechaniku, kusovník a rozhraní (hřídel / upevnění).

## Varianty

| Složka | Stav | Popis |
| --- | --- | --- |
| [`variants/mecanum-100mm`](variants/mecanum-100mm/) | aktivní | Ø 100 mm, 9 válečků, otvor hřídele Ø 6 mm |
| [`variants/simple-100mm`](variants/simple-100mm/) | rozpracováno | jednoduché kolo Ø 100 mm |

Nová varianta = nová podsložka ve `variants/` se stejným tvarem: `README.md` + `image/` + `step/`.

## Společné rozhraní

Platí pro všechny varianty, pokud konkrétní varianta neurčí jinak.

| Parametr | Požadavek / poznámka |
| --- | --- |
| Hřídel motoru | typicky Ø 6 mm (D-cut dle motoru) |
| Upevnění | svěrka hřídele / shaft interface + spojovací materiál |
| Orientace mecanum | zrcadlové páry L/R — viz dokumentace varianty |
| Montáž na rám | přes motor clamp platformy / vlastní držák |
| Elektrika / SW | žádné — čistě mechanický díl |

Referenční build R-MODUS používá `variants/mecanum-100mm` na [hw-robot-platform](https://github.com/R-MODUS/hw-robot-platform).

## Verzování

Verze se **nepíšou do souboru** v repu. Používají se **Git tagy** a GitHub Releases (např. `v1.0.0` s poznámkou, která varianta platí).

## Rychlý start

1. Vyber variantu ve `variants/` a otevři její `README.md`.
2. Natiskni / vyrob díly ze `step/` dané varianty.
3. Dodrž společné rozhraní výše.

## Související

- [hw-robot-platform](https://github.com/R-MODUS/hw-robot-platform) — referenční podvozek
- [hw-esp-4ch-motor-driver](https://github.com/R-MODUS/hw-esp-4ch-motor-driver) — řízení motorů (samostatné repo s FW)

## Licence

[MIT](LICENSE)
