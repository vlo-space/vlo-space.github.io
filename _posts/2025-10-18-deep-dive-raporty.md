---
title: "Deep dive: Jak VLO Space pisze raporty?"
author: "Kamil Kaczyński"
media:
- {url: "cover.jpg", title: "Wybrane strony z raportu PDR naszej drużyny"}
---

CanSat to konkurs którego znaczna część polega na drużynowym pisaniu raportów. Każdy, kto w&nbsp;kilka osób pisał dowolny dokument wie jednak, że często wiąże się to ze znaczną ilością bałaganu. 

Czy w&nbsp;szkole, czy w&nbsp;pracy, trudno zmusić współpracowników do stosowania identycznego stylu i&nbsp;rozmiaru czcionek, obrazków, tabel, diagramów oraz ich opisów. Ma to szczególne znaczenie przy pisaniu technicznych dokumentów, gdzie czytelność takich elementów jest podstawą zrozumienia tekstu.

W zeszłym roku pisaliśmy nasze raporty na platformie Google Docs. Rozwiązanie to wybraliśmy głównie dla możliwości równoległej pracy nad różnymi częściami dokumentu.

Osoby bardziej zaznajomione z&nbsp;pisaniem technicznych dokumentów znają popularne rozwiązanie stosowane w&nbsp;kręgach naukowych. LaTeX to system w&nbsp;którym zamiast pisać tekst w&nbsp;graficznym środowisku, pisze się specjalny kod, który oprócz samej zawartości opisuje również jak dokument ma wygądać.

LaTeX jest systemem w&nbsp;którym łatwiej jest utrzymać porządek w&nbsp;stylu dokumentu. Taki sposób pracy ma jednak swoje wady -&nbsp;LaTeX to program który rozwijał się przez ostatnie 41 lat, a&nbsp;co za tym idzie -&nbsp;nie jest zbyt nowoczesny czy szybki. Z&nbsp;tego powodu użytkownicy LaTeXa również często nie mają podglądu na żywo podczas pisania dokumentu.

<div class="container">
    <img src="{{page.asset_base}}{{page.slug}}/latex-code.jpg" title="Kod napisany w systemie LaTeX">
    <img src="{{page.asset_base}}{{page.slug}}/latex-vis.jpg" title="Wygenerowany dokument w systemie LaTeX">
</div>

Drugim problemem jest przystępność -&nbsp;osobom z&nbsp;doświadczeniem programistycznym względnie łatwo jest zrozumieć taki system, ale członkom drużyny odpowiadającym za inne aspekty projektu mogłoby być trudno go zaadoptować.

Frustracja wynikająca z&nbsp;tych problemów jest genezą nowego narzędzia -&nbsp;[Typst'a](https://typst.app). Ma ono być szybsze, oraz bardziej intuicyjne niż jego poprzednicy.

<div class="container">
    <img src="{{page.asset_base}}{{page.slug}}/typst-code.jpg" title="Kod napisany w systemie Typst">
    <img src="{{page.asset_base}}{{page.slug}}/typst-vis.jpg" title="Wygenerowany dokument w systemie Typst">
</div>

Gdy na początku tej edycji pokazałem Typst'a reszcie drużyny, reakcja nie była szczególne entuzjastyczna. Główną obawą była trudność nauki nowego systemu. Jednak w&nbsp;obecnym momencie projektu nawet najmniej zaznajomieni z&nbsp;softwarem członkowie dużyny potrafią z&nbsp;niego korzystać.

Korzyści ze zmiany systemu nie kończą się jednak na ujednoliceniu stylów. Dzięki Typst'owi numery figur, tabeli i&nbsp;diagramów są automatycznie aktualizowane w&nbsp;tekście, diagramy są napisane bezpośrednio w&nbsp;dokumencie, a&nbsp;nawet okładka naszego raportu została wykonana bez użycia zewnętrznych programów graficznych.

Choć Typst zdecydowanie nie jest systemem dla wszystkich, dla nas okazał się on być właściwym rozwiązaniem, które znacznie poprawiło jakość prezentacji naszego raportu. W&nbsp;ramach konkrusu CanSat aspekty techniczne pojawiają się nie tylko przy projektowaniu i&nbsp;wykonywaniu samej sondy, ale również przy rzeczach, które wydają się być względnie mało znaczące.

