# wordpress
Modified wordpress code, adapted to optimization on litespeed server.

W pliku konfiguracyjnym (wp-config.php) znajduje się sekcja z kluczami. Wykorzystywane są one do autoryzacji oraz enkrypcji, dlatego warto zadbać o to, aby każda instancja WordPressa, posiadała unikalne klucze. Wykorzystywanie tych samych kluczy, na wielu stronach, jest niebezpieczne.

Generator kluczy dostępny jest pod linkiem: https://api.wordpress.org/secret-key/1.1/salt/
