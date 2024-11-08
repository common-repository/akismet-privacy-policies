=== Akismet Privacy Policies ===
Contributors: inpsyde, Bueltge
Tags: akismet, privacy, spam
License: GPLv2 or later
Requires PHP: 5.6
Requires at least: 3.0
Tested up to: 5.4
Stable tag: 2.0.1

Ergänzt das Kommentarformular um datenschutzrechtliche Hinweise bei Nutzung des Plugins Akismet.

== Description ==
Der Einsatz des Anti-Spam-Plugins Akismet ist in Deutschland aus datenschutzrechtlichen Aspekten sehr bedenklich, da personenbezogene Daten auf Servern in den USA gespeichert werden.

Um keine Angriffsfläche für Abmahnungen zu bieten, muss man die Benutzer vor dem Kommentieren auf das Speichern dieser Daten hinweisen. Dies übernimmt das Plugin.

= Erstellt durch Inpsyde =
Das Team der [Inpsyde](https://inpsyde.com) entwickelt im Web und WordPress seit 2006.

= Spenden? =
Du möchtest etwas spenden - wir bevorzugen ein positives Review, nicht mehr.

== Installation ==
1. Plugin herunterladen, entpacken, in den Ordner `wp-content/plugins/` laden und aktivieren. Oder direkt über den Adminbereich und 'Plugins' - 'Installieren' das Plugin suchen und installieren.
2. Das Plugin sollte nun automatisch unter dem Kommentarfeld den Hinweistext anzeigen. Falls nicht, muss im Theme (z.B. comments.php) manuell folgender Code innerhalb des Kommentar-Formulares, innerhalb `<form>...</form>` - da wo der Hinweis erscheinen soll, eingefügt werden:

    `<?php do_action( 'akismet_privacy_policies' ); ?>`

Der Aufruf muss an der Stelle des Templates statt finden, wo die Ausgabe erscheinen soll.

== Frequently Asked Questions ==
= Wo finde ich weitere Informationen zum Thema Datenschutz und Akismet? =

Rechtsanwalt Thomas Schwenke klärt in einem Artikel auf: [Usability VS Datenschutz – Datenschutzrechtliche Einwilligung ohne Opt-In?](http://drschwenke.de/usability-vs-datenschutz-datenschutzrechtliche-einwilligung-ohne-opt-in/)

= Plugin Dokumentation =
* [Hook-Documentation](https://github.com/inpsyde/Akismet-Privacy-Policies/wiki/Hook-Documentation)

== Screenshots ==
1. So sieht das Plugin im Einsatz aus.
2. Die optionalen Einstellungen im Backend von WordPress

== Changelog ==
= 2.0.1 =
* Fix loading of mo-file if is not exist.

= 2.0.0 =
* Multilinguale Version: Datenschutz- und Fehlerhinweis können für verschiedene Sprachen (momentan de_DE und en_US) getrennt abgespeichert werden und werden entsprechend den Spracheinstellungen der jeweiligen Wordpress-Installation beim Verfassen eines Kommentares angezeigt.
* Änderung Aufruf der inernen Hilfe.

= 1.1.2 =
* Link zum Datenschutzhintergrund ergänzt
* Source-Codex Anpassungen

= 1.1.1 =
* Prüfung auf Sprache der WordPress Installation, nur bei `de_DE` als Sprachschlüssel, werden die Hinweise ergänzt

= 1.1.0 =
* Weitere Hinweistexte und Mustertext für Datenschutzerklärung

= 1.0.0 =
* Release first version


